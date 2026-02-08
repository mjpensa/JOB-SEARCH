# Career Strategy Command Center — Setup Guide

> **⚠️ This repo contains personal information (phone, email, contact names, career details). Keep it private.**

## Project Structure

job-search/
├── CLAUDE.md                              # Core behavioral instructions (Claude Code reads this automatically)
├── .claudeignore                          # Keeps Claude Code focused on source files
├── README.md                              # This file
├── docs/                                  # Knowledge base (source of truth — don't modify without approval)
│   ├── master-resume.md                   # Complete resume in markdown
│   ├── career-narrative.md                # Strategic narrative, target roles, STAR+R stories
│   ├── portfolio-governance-framing.md    # 5 AI prototypes with governance/risk mappings
│   ├── engagement-mapping.md              # 10 consulting engagements → AI governance connections
│   ├── objection-handling.md              # 5 interview objections with approved responses
│   ├── target-criteria.md                 # Company tiers, role preferences, compensation, disqualifiers
│   ├── contacts.md                        # Networking contacts with relationship context
│   ├── regulatory-cheat-sheet.md          # SR 11-7, NIST AI RMF, EU AI Act distinctive angles [SCAFFOLD]
│   ├── lessons-learned.md                 # Running log of corrections and application outcomes
│   ├── exemplar-cover-letters.md          # Gold standard cover letters [PLACEHOLDER]
│   └── exemplar-STAR-answers.md           # Gold standard interview answers [PLACEHOLDER]
└── outputs/                               # Generated deliverables (created automatically)
    ├── jd-analysis-*.md                   # Saved JD analyses for cross-session reference
    ├── cover-letter-*.md                  # Draft cover letters
    └── networking-*.md                    # Outreach messages

## Setup

1. Place all files in a local directory maintaining the structure above
2. Open Claude Code in that directory: `claude` from the project root
3. CLAUDE.md loads automatically — all behavioral rules, commands, and file references are active

## Commands
- **ANALYZE JD** + paste a job description → structured fit assessment (saved to `outputs/` for future reference)
- **DRAFT COVER LETTER** + specify target role → tailored cover letter (auto-checks for prior JD analysis)
- **INTERVIEW PREP** + role type → questions, STAR answers, objection prep
- **NETWORKING** + name and context → outreach message draft

## How Sessions Work in Claude Code

**Key difference from Claude.ai:** Each Claude Code session starts fresh. Claude Code reads CLAUDE.md automatically but has no memory of previous sessions. GitHub serves as the persistence layer:

- **JD analyses are saved to `outputs/` and committed to GitHub** so any future session on any machine can reference them
- **Corrections are appended to `docs/lessons-learned.md` and committed** so they persist across sessions and machines
- **Cover letters and networking messages are committed** so you have full version history of every deliverable
- **Claude Code pulls before starting work and pushes after completing it** — the repo is always current

This means you can work from any machine with Claude Code and the repo cloned. All state lives in GitHub.

## Files to Complete
Three files are scaffolded but need content developed through interactive sessions:
1. `docs/regulatory-cheat-sheet.md` — Fill in your distinctive angles on each framework
2. `docs/exemplar-cover-letters.md` — Add 2-3 cover letters you're satisfied with
3. `docs/exemplar-STAR-answers.md` — Polish 3-5 interview answers through practice

## Maintaining the System
- **Corrections:** When you correct Claude Code's output, it will automatically append to `docs/lessons-learned.md`. Periodically review this file to ensure it's accurate.
- **Application outcomes:** Tell Claude Code the result (e.g., "Bank A advanced me to round 2 — the regulatory depth framing resonated"). It will log it.
- **Contacts:** Update `docs/contacts.md` as new networking contacts are identified. Tell Claude Code to add entries, or edit directly.
- **Target criteria:** Update `docs/target-criteria.md` if target companies or role preferences shift.
- **Source files:** Claude Code will not modify files in `docs/` without asking first (except lessons-learned.md). If it suggests an edit to your resume or STAR stories, review and approve before it writes.
