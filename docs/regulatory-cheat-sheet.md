# Regulatory Framework Cheat Sheet

This file captures Matthew's distinctive angles on key regulatory frameworks — not generic summaries of what the frameworks say, but his specific talking points, connections to his experience, and perspectives that differentiate him from other candidates.

---

## SR 11-7 (OCC Supervisory Guidance on Model Risk Management)

### Core relevance
SR 11-7 defines model risk management requirements for banking organizations. It was written for traditional quantitative models. The critical question for AI governance roles: how does SR 11-7 extend to AI/ML models, and where does it break down?

### Matthew's distinctive angles
[TO BE COMPLETED — develop through interactive session. Key questions to address:]
- How would you argue SR 11-7 applies to LLMs? Where does the definition of "model" include or exclude GenAI?
- What specific SR 11-7 requirements (effective challenge, documentation, outcome analysis) become harder or different with AI/ML?
- How does your RBC data lineage experience connect to SR 11-7 model input validation?
- How does your HSBC RCSA experience connect to the risk identification requirements?
- What's your view on extending SR 11-7 vs. creating new AI-specific guidance?

### JD language mapping
When JDs mention "model risk management," "effective challenge," "three lines of defense," "model validation," or "SR 11-7" — they are referencing this framework. Use terminology naturally.

---

## NIST AI Risk Management Framework (AI RMF 1.0)

### Core relevance
Four core functions: Govern, Map, Measure, Manage. Voluntary framework but increasingly referenced by US regulators and adopted as an internal standard by financial institutions.

### Matthew's distinctive angles
[TO BE COMPLETED — develop through interactive session. Key questions to address:]
- How do you map your consulting experience to each of the four functions?
  - Govern → governance framework design (Wells Fargo, MasterCard)
  - Map → risk identification and taxonomy (HSBC RCSA, MasterCard taxonomy)
  - Measure → quantification of risk (HSBC likelihood/impact, Key Bank market analysis)
  - Manage → controls implementation and change management (BofA, all engagements)
- How do you connect NIST AI RMF to SR 11-7? Where do they overlap, where do they complement?
- What insights from your prototyping work inform how you'd implement NIST AI RMF in practice?
- Where does NIST AI RMF fall short for financial services specifically?

### JD language mapping
When JDs mention "AI risk management framework," "responsible AI," "AI governance framework," or "NIST" — connect to this.

---

## EU AI Act

### Core relevance
Risk-based classification system: unacceptable, high-risk, limited risk, minimal risk. Most relevant to financial services: credit scoring, insurance pricing, and fraud detection are classified as high-risk. Compliance deadlines phased through 2027.

### Matthew's distinctive angles
[TO BE COMPLETED — develop through interactive session. Key questions to address:]
- How does the EU AI Act risk-tiering approach compare to how US banks currently classify AI use cases?
- How does your MasterCard risk taxonomy work connect to the concept of risk-tiering AI applications?
- What's your view on the EU approach vs. the US approach (voluntary frameworks vs. prescriptive regulation)?
- How would you advise a global bank that needs to comply with both EU AI Act and US guidance?

### JD language mapping
When JDs mention "EU AI Act," "AI regulation," "risk classification," "high-risk AI systems," or "regulatory compliance for AI" — connect to this.

---

## GenAI-Specific Risks (Cross-Framework)

### Key risks Matthew can speak to from firsthand experience
[TO BE COMPLETED — develop through interactive session. For each, connect to a specific prototype:]
- **Hallucination** → ISDA CDM RAG pipeline (retrieval failure modes, context window overflow)
- **Data leakage** → Power Automate agent (write access to production systems)
- **Prompt injection** → [develop angle]
- **Explainability/interpretability** → [develop angle]
- **Agentic risk / autonomous decision-making** → Power Automate agent (authorization boundaries, rollback triggers)
- **Data lineage for AI** → RBC CCAR reporting + ISDA CDM RAG
- **Model drift** → Wells Fargo data resiliency (monitoring and detection frameworks)
