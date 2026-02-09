# GitHub Authentication & Configuration — Claude Code Environment

## Git Remote — Local Proxy

The remote URL is **not** a direct connection to `github.com`. Instead it routes through a **local proxy**:

```
http://local_proxy@127.0.0.1:62100/git/mjpensa/JOB-SEARCH
```

A proxy running on `localhost:62100` intercepts all git operations (push, fetch, pull) and forwards them to GitHub. The proxy handles authentication transparently — credentials are embedded in the proxy layer, not in git config or environment variables. The `http.proxyAuthMethod=basic` setting tells git to use basic auth when communicating with this proxy.

## Commit Signing

Commits are signed using a custom SSH-based mechanism:

- **Signing key:** `/home/claude/.ssh/commit_signing_key.pub`
- **Signing program:** `/tmp/code-sign` (a custom wrapper, not standard `ssh-keygen`)
- `commit.gpgsign=true` — all commits are automatically signed

Relevant gitconfig:

```ini
[gpg]
    format = ssh
[gpg "ssh"]
    program = /tmp/code-sign
[commit]
    gpgsign = true
```

## Identity

- **Author:** `Claude <noreply@anthropic.com>`
- No personal GitHub credentials or tokens are exposed to the session

## No `gh` CLI

The GitHub CLI (`gh`) is **not installed** in this environment. All GitHub interaction must go through `git` commands routed via the local proxy.

## Branch-Level Access Control

The proxy enforces branch naming restrictions:

- Pushes **must** target branches matching `claude/*` with a valid session ID suffix
- Pushes to other branches (e.g., `main` directly) will be rejected with a **403**
- A GitHub Actions workflow (`.github/workflows/auto-merge-claude.yml`) automatically merges `claude/*` branches into `main` on every push

## Full Git Config Reference

### Global (`/root/.gitconfig`)

```ini
[user]
    name = Claude
    email = noreply@anthropic.com
    signingkey = /home/claude/.ssh/commit_signing_key.pub
[gpg]
    format = ssh
[gpg "ssh"]
    program = /tmp/code-sign
[commit]
    gpgsign = true
[http]
    proxyAuthMethod = basic
[core]
    checkStat = minimal
```

### Repo-level (`.git/config`)

```ini
[remote "origin"]
    url = http://local_proxy@127.0.0.1:62100/git/mjpensa/JOB-SEARCH
    fetch = +refs/heads/*:refs/remotes/origin/*
[gc]
    auto = 0
```
