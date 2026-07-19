# Course Overlap Audit Table

> **Purpose**: Cross-reference all four tracks to confirm zero course overlap and validate topic differentiation.  
> **Last Audited**: July 2026

---

## Full 4-Track Overlap Audit

| Topic | Track A (Dev — Tools) | Track B (QA) | Track C (BA) | Track D (AI Dev — Build) | Overlap Risk | Resolution |
|-------|----------------------|--------------|--------------|-------------------------|--------------|------------|
| **AI/ML Fundamentals** | 3Blue1Brown "But what is a GPT?" (visual, conceptual) | IBM AI Foundations for Everyone (Coursera — lifecycle lens) | AI For Everyone — Andrew Ng (Coursera — business strategy) | Machine Learning Specialization — Andrew Ng (Coursera — hands-on technical) | Medium ⚠️ | 4 different courses. Dev = visual tool understanding; QA = lifecycle/testing lens; BA = business strategy; AI Dev = deep mathematical/technical |
| **Prompt Engineering** | YouTube: Prompts for Copilot/Claude Code (tool-level) | Udemy: Prompt testing for QA (adversarial/boundary) | Udemy: ChatGPT for BA workflows (requirements/analysis) | Coursera: ChatGPT Prompt Engineering for Developers (API-level, system prompts) | High 🔴 | 4 completely different courses. Dev = tool prompts; QA = testing prompts; BA = productivity prompts; AI Dev = production API prompts. Zero content overlap. |
| **LLM / GenAI Concepts** | 3Blue1Brown + Fireship (how copilots work) | IBM Technology YouTube (non-determinism, hallucinations for QA) | AI For Everyone (business applications of GenAI) | Hugging Face LLM Course (transformer internals, fine-tuning) | High 🔴 | 4 different sources. Dev = copilot mechanics; QA = failure modes; BA = business impact; AI Dev = architecture & training. |
| **AI Agents** | GitHub Copilot Agent Mode + Claude Code (Udemy/YouTube — using agents) | — | — | AI Agents in LangGraph (freeCodeCamp — building agents) + Multi-Agent Systems (Udemy) | High 🔴 | Dev = using agentic tools; AI Dev = building agent systems. Completely different scope and courses. No QA/BA agent courses. |
| **AI Security** | YouTube: Secrets in prompts, code leakage, supply chain (developer concerns) | Udemy: Adversarial testing, prompt injection testing (QA testing methodology) | — | YouTube: OWASP AI security, prompt injection defence (engineering defence) | Medium ⚠️ | 3 different courses, 3 different perspectives: Dev = avoid risks when using tools; QA = find vulnerabilities; AI Dev = build defences. |
| **Bias & Fairness** | — | Google AI: Bias testing from QA perspective | edX: AI Ethics (business/governance lens) | Google ML Crash Course: Fairness module (technical implementation) | Medium ⚠️ | QA = testing methodology; BA = governance/ethics awareness; AI Dev = implementation (SHAP, LIME). Different courses. |
| **RAG (Retrieval-Augmented Generation)** | — | Udemy: Testing RAG with DeepEval/RAGAS (QA evaluation) | — | Udemy: LangChain & RAG Applications (building RAG pipelines) | Medium ⚠️ | QA = evaluating RAG quality; AI Dev = building RAG systems. Different Udemy courses with different focus. |
| **MLOps / Production** | — | YouTube: Production monitoring, drift detection (QA monitoring) | — | MLOps Zoomcamp (building ML pipelines) + Coursera MLOps (monitoring) | Low ✅ | QA = monitoring AI quality; AI Dev = building and operating ML pipelines. Different scope. |
| **Data Strategy** | — | — | Coursera: Data Strategy (business assessment) | Kaggle Learn: Pandas + EDA (technical implementation) | None ✅ | BA = data governance/strategy; AI Dev = data engineering. No overlap. |
| **AI Ethics & Governance** | — | — | Coursera: AI Governance + Alison: EU AI Act (regulatory) | Google AI: Responsible AI (technical fairness) | Low ✅ | BA = regulatory/governance; AI Dev = technical implementation. |
| **AI for Testing/QA** | — | Udemy: Gen AI in Automation Testing + RAG Evals + Advanced QA (3 courses) | — | — | None ✅ | Track B exclusive. No other track covers testing AI systems. |
| **AI for Business Analysis** | — | — | Udemy: ChatGPT for BAs + Self-study workshops (requirements, feasibility) | — | None ✅ | Track C exclusive. No other track covers business analysis with AI. |
| **Brownfield / Legacy Modernisation** | YouTube: AI-assisted legacy code audit, documentation, upgrades (curated micro-paths) | — | — | — | None ✅ | Track A exclusive (Tier 3B). Not a concern for model builders. |
| **Dependency Upgrades / Maintenance** | YouTube: AI-assisted dependency upgrades, changelog generation | — | — | — | None ✅ | Track A exclusive. Operational dev workflow, not model-building. |
| **GitHub Copilot** | Udemy: 2 Copilot courses (tool mastery) | — | — | — | None ✅ | Track A exclusive. |
| **Claude Code** | YouTube + freeCodeCamp: Claude Code tutorials | — | — | — | None ✅ | Track A exclusive. |
| **Fine-Tuning LLMs** | — | — | — | Hugging Face Learn: LoRA, QLoRA, PEFT | None ✅ | Track D exclusive. |
| **Model Deployment** | — | — | — | MLOps Zoomcamp + Coursera: FastAPI, Docker, serving | None ✅ | Track D exclusive. |
| **Experiment Tracking** | — | — | — | YouTube: MLflow tutorial | None ✅ | Track D exclusive. |
| **AI Tools for Productivity** | — | — | Udemy: ChatGPT for BAs; YouTube: Power BI Copilot | — | None ✅ | Track C exclusive. |
| **ROI & Vendor Evaluation** | YouTube: Measuring AI productivity (dev perspective) | — | YouTube: AI ROI modelling + vendor evaluation (business perspective) | — | Low ✅ | Dev = developer productivity metrics; BA = business ROI/vendor assessment. Different focus. |

---

## Duplicate Detection Summary

### Course-Level Duplicates
✅ **No course appears in more than one track.**

### Content-Level Overlap (>70% curriculum overlap within same track)
✅ **No two courses within the same track cover >70% overlapping content.**

### Track A ↔ Track D Special Audit
✅ **Zero content bleed confirmed.** See [06_track_a_vs_d_boundary_analysis.md](file:///c:/Users/user/Projects/stock-market-analysis/learning-path/_outputs/06_track_a_vs_d_boundary_analysis.md) for detailed delineation.

---

## High-Risk Overlap Areas — Mitigation Details

### 1. "Prompt Engineering" (Highest Risk 🔴)
- **Track A**: Typing prompts into Copilot/Claude Code chat interfaces → "Refactor this function"
- **Track B**: Testing prompts for AI features → "What happens with adversarial input?"
- **Track C**: Using ChatGPT for BA tasks → "Generate user stories for this feature"
- **Track D**: Designing system prompts for APIs → `{"role": "system", "content": "..."}`
- **4 different courses on 4 different platforms. RESOLVED.**

### 2. "AI Agents" (High Risk 🔴)
- **Track A**: Using Agent Mode in Copilot, using Claude Code agentic features
- **Track D**: Building agent systems with LangChain/LangGraph/CrewAI
- **2 different courses. Using ≠ Building. RESOLVED.**

### 3. "LLM Concepts" (High Risk 🔴)
- **Track A**: 3Blue1Brown visual + Fireship overview → conceptual understanding
- **Track B**: IBM Technology YouTube → hallucination/non-determinism for QA
- **Track C**: Andrew Ng AI For Everyone → business applications of GenAI
- **Track D**: Hugging Face LLM Course → transformer internals, fine-tuning
- **4 different sources at 4 different depth levels. RESOLVED.**

---

## Quarterly Audit Checklist

When refreshing courses each quarter, verify:

- [ ] No newly added course appears in more than one track
- [ ] Track A courses focus on USING AI tools, not building AI systems
- [ ] Track D courses focus on BUILDING AI systems, not using coding assistants
- [ ] Track B courses are QA-specific (testing, validation, quality)
- [ ] Track C courses are non-technical (strategy, governance, business analysis)
- [ ] Any course that could fit in 2+ tracks has been replaced with track-specific alternatives
- [ ] Shared topics (AI fundamentals, prompt engineering) use different courses per track
