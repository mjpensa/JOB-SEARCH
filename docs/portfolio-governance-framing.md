# Portfolio Governance Framing

When referencing prototyping work in any output (cover letters, interview prep, LinkedIn content), always lead with the governance or risk insight, not the technical build. For enablement-focused roles, also deploy the enablement framing to demonstrate hands-on tool evaluation, deployment, and adoption experience.

Lead stories for interviews and cover letters: #1 (ISDA CDM RAG) and #4 (Power Automate agent). Use #2 for versatility. Use #3 and #5 only as supporting evidence when relevant.

For enablement-focused roles, #4 (Power Automate agent) and #2 (Research-to-Deliverable) are the strongest enablement stories. #1 (ISDA CDM RAG) leads for tool evaluation framing.

---

## Project 1: ISDA CDM RAG Pipeline (LEAD STORY)

**What was built:** A semantic RAG pipeline built on the ISDA Common Domain Model, using domain-specific embeddings, a CDM Rosetta-based knowledge graph, semantic chunking, validation, reranking, and BM25 hybrid search — with Claude Code as the query interface.

**Governance framing (always lead with this):** Demonstrates firsthand understanding of retrieval failure modes, hallucination risk when context windows overflow, data lineage challenges in tracing LLM outputs to source documents, and why domain-specific embeddings matter for accuracy in regulated contexts. Directly informs model validation requirements under SR 11-7 and data governance under NIST AI RMF.

**Enablement framing:** Demonstrates the tool evaluation skill set that AI CoE and enablement roles require — evaluating retrieval architectures, testing domain-specific embeddings vs. general-purpose models, and determining what works for regulated financial data. The hands-on evaluation of chunking strategies, reranking approaches, and hybrid search directly informs use case feasibility assessments for business units.

**Use when discussing:** Model validation, data governance, hallucination risk, retrieval accuracy in regulated contexts, why generic models fail on domain-specific financial data, AI tool evaluation methodology, or use case feasibility assessment.

---

## Project 2: Research-to-Deliverable App (Gantt/PPTX/DOCX)

**What was built:** A full-stack LLM application that ingests user research and generates a synchronized roadmap (Gantt chart), branded PowerPoint presentation, and executive summary — all anchored to LLM-generated swimlanes and exportable to PPTX/DOCX.

**Governance framing:** Demonstrates understanding of AI-generated content flowing into client or board-level deliverables — accuracy validation, audit trail from source to output, and the risk of unverified LLM-generated analysis being exported into decision-making materials.

**Enablement framing:** Built a tool that automates professional deliverable generation — demonstrating understanding of what business users actually need from AI tools: reliable output formats, integration with existing workflows (PowerPoint, Word), and quality that meets professional standards. This is the kind of internal accelerator that AI CoE teams build to drive adoption.

**Use when discussing:** AI output validation, audit trails, risk of AI-generated content in decision-making deliverables, quality assurance for AI outputs, building internal AI accelerators, or understanding business user requirements for AI tools.

---

## Project 3: Autonomous Web Research Agents

**What was built:** Autonomous web research agents with data ingestion pipelines, including video transcription via OpenAI Whisper.

**Governance framing:** Demonstrates understanding of the data ingestion layer of AI systems — source data provenance, quality variability, and why governance frameworks must extend upstream of the model to the data collection pipeline. Multimodal transcription (Whisper) shows awareness of accuracy challenges across input modalities.

**Enablement framing:** Limited. Primarily demonstrates data pipeline understanding. Supporting example only.

**Use when discussing:** Data provenance, upstream data governance, source quality challenges, multimodal AI risks. Supporting example only — not a lead story.

---

## Project 4: Autonomous Power Automate Agent (LEAD STORY)

**What was built:** An autonomous Claude Code agent that takes a Power Automate design specification and builds, validates, deploys, debugs (via Dataverse error retrieval), and iterates until 100% functionality is verified across Outlook, SharePoint, Power Automate, Copilot Studio, and Azure.

**Governance framing (strongest governance story):** Demonstrates firsthand understanding of agentic AI risk — what happens when an autonomous system has write access to production enterprise infrastructure (Outlook, SharePoint, Azure), makes deployment decisions without human approval, and self-iterates. Directly illustrates why existing model risk frameworks designed for static models break down for autonomous agents, and why new controls are needed around authorization boundaries, rollback triggers, and audit logging.

**Enablement framing (strongest deployment lifecycle story):** Demonstrates end-to-end AI deployment across enterprise infrastructure — building, validating, deploying, debugging, and iterating an autonomous agent across Microsoft's enterprise stack (self-directed prototyping). Hands-on experience with the full AI deployment lifecycle, including integration with enterprise systems (Outlook, SharePoint, Azure), automated testing and validation, and debugging in real environments. Directly relevant to evaluating AI automation tools for business units.

**Use when discussing:** Agentic AI risk, autonomous system governance, authorization boundaries, why SR 11-7 needs extension for agentic systems, production deployment risk, human-in-the-loop requirements, AI deployment lifecycle, enterprise AI integration, or evaluating AI automation tools.

---

## Project 5: Resume Conversion Agent

**What was built:** An agent for autonomously converting external resumes into branded templates.

**Governance framing:** Supporting example demonstrating template compliance, output consistency, and quality assurance in AI-generated documents.

**Enablement framing:** Limited. A lightweight automation example. Supporting only.

**Use as:** A lighter supporting example only. Not a lead story.
