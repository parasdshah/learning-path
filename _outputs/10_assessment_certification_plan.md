# Assessment & Certification Plan

> **Purpose**: Define assessment criteria, deliverables, and certification for each tier across all four tracks.

---

## Assessment Philosophy

- **No high-stakes exams** — assessments are formative and portfolio-building
- **Applied > Theoretical** — hands-on projects weighted higher than quizzes
- **Peer learning** — peer review is a required component at Tier 2+
- **Cross-functional collaboration** — Tier 3 capstone requires 4-role teams
- **Self-paced** — assessments available anytime; no scheduled exam windows

---

## Tier 1 — Foundational Assessment

### Format: Quiz + Reflection

| Component | Details |
|-----------|---------|
| **Quiz** | 20-question MCQ, randomised from question bank of 50+ |
| **Pass Score** | ≥80% (16/20 correct) |
| **Attempts** | Unlimited (questions randomise each attempt) |
| **Time Limit** | None (self-paced) |
| **Reflection** | 500-word written response |
| **Reflection Prompt** | "How AI applies to my role — specific ways I will use AI in my daily work" |
| **Reflection Review** | Self-submitted; reviewed for completeness only (not graded on content) |

### Track-Specific Quiz Topics

| Track | Quiz Topics |
|-------|------------|
| **A (Dev)** | LLM concepts, token limits, AI tool capabilities, prompt basics, when to trust/not trust AI output |
| **B (QA)** | AI/ML types, LLM behaviour, non-determinism, AI product lifecycle, why traditional testing fails |
| **C (BA)** | AI capabilities/limitations, business applications, AI ethics, project lifecycle, common misconceptions |
| **D (AI Dev)** | ML algorithms, bias/variance, neural networks, Python libraries, data preprocessing, evaluation metrics |

### Certification: **AI Foundations Badge** 🥉
- Issued upon passing quiz + submitting reflection
- Digital badge shareable on LinkedIn
- Valid indefinitely (foundational knowledge)

---

## Tier 2 — Intermediate Assessment

### Format: Mini-Project + Peer Review

| Component | Details |
|-----------|---------|
| **Mini-Project** | Role-specific hands-on project (see below) |
| **Documentation** | Written report documenting process, decisions, and outcomes |
| **Peer Review** | Review by 1 colleague who has completed or is completing the same tier |
| **Peer Review Criteria** | Completeness, quality, practical applicability |
| **Revision Cycle** | 1 revision allowed after peer feedback |

### Track-Specific Mini-Projects

#### Track A (Developers)
**Project**: Refactor an Existing Module Using AI Agents End-to-End
1. Select a real module from your codebase (50–200 lines of code)
2. Use AI agents to understand the current code
3. Plan the refactoring with AI assistance (document the plan)
4. Execute the refactoring using agentic workflows
5. Generate tests using AI
6. Generate documentation using AI
7. Create a PR with AI-assisted commit messages

**Deliverables**:
- Before/after code (Git diff)
- Workflow journal (prompts used, output quality ratings, modifications made)
- Time tracking (AI-assisted time vs estimated manual time)

#### Track B (QA Engineers)
**Project**: Create an AI Test Plan for a Non-Deterministic Feature
1. Choose an LLM-powered feature (real or hypothetical)
2. Define acceptance criteria with quantitative thresholds
3. Design test cases: happy path, edge cases, adversarial inputs
4. Define regression strategy for non-deterministic outputs
5. Implement ≥5 automated test cases using DeepEval or RAGAS

**Deliverables**:
- AI Test Plan document
- Automated test scripts with results
- Quality assessment report

#### Track C (Business Analysts)
**Project**: AI Feasibility Report with Data Readiness Assessment
1. Choose a real or hypothetical AI initiative
2. Conduct data availability and quality audit
3. Assess technical feasibility
4. Compare build vs buy options
5. Write AI-ready requirements with quantitative acceptance criteria

**Deliverables**:
- 10-page feasibility report
- Data readiness scorecard
- AI-ready requirements document
- 15-minute presentation deck

#### Track D (AI/ML Developers)
**Project**: Build and Deploy a RAG Application or AI Agent
1. Design the architecture
2. Implement with LangChain/LangGraph
3. Include vector database for knowledge retrieval
4. Add tool use / function calling
5. Deploy using FastAPI + Docker
6. Track experiments with MLflow

**Deliverables**:
- Working deployed application (GitHub repo + deployment URL/instructions)
- Architecture decision document
- Experiment tracking logs
- API documentation

### Certification: **AI Practitioner Badge** 🥈
- Issued upon project completion + passing peer review
- Digital badge shareable on LinkedIn
- Valid for 2 years (reassessment recommended as tools evolve)

---

## Tier 3 — Advanced Assessment

### Format: Cross-Functional Capstone + Peer Review

| Component | Details |
|-----------|---------|
| **Team Formation** | 1 Dev (Track A) + 1 QA (Track B) + 1 BA (Track C) + 1 AI Dev (Track D) |
| **Project Duration** | 2–3 weeks (part-time, alongside regular work) |
| **Project Scope** | Design, build, test, and create a business case for an AI initiative |
| **Presentation** | 30-minute team presentation to a panel (managers + senior engineers) |
| **Peer Review** | Cross-functional team reviews each other's contributions |

### Capstone Project Structure

| Role | Responsibility | Deliverables |
|------|---------------|-------------|
| **BA (Track C)** | Define the AI opportunity, write requirements, build business case | Business case, AI-ready requirements, ROI model |
| **AI Dev (Track D)** | Architect and build the AI component | System architecture, working AI prototype, evaluation metrics |
| **Dev (Track A)** | Integrate the AI component into an application using AI tools | Working integration, Git history showing AI-assisted development |
| **QA (Track B)** | Validate the AI system | AI test plan, adversarial testing results, bias audit, monitoring spec |

### Evaluation Criteria

| Criterion | Weight | Description |
|-----------|--------|-------------|
| **Technical Quality** | 25% | Working system, clean code, proper architecture |
| **AI Tool Usage** | 20% | Evidence of effective AI tool/agent usage throughout |
| **Cross-Functional Collaboration** | 20% | Team communication, integration between components |
| **Documentation & Communication** | 15% | Clear docs, presentation quality, stakeholder-ready |
| **Innovation & Impact** | 10% | Creative use of AI, potential business value |
| **Risk & Governance** | 10% | Ethics consideration, security awareness, governance compliance |

### Certification: **AI Champion Badge** 🥇
- Issued upon capstone completion + passing panel review
- Digital badge shareable on LinkedIn
- Recognised as internal AI subject matter expert
- Eligible to mentor Tier 1–2 learners
- Valid for 1 year (annual re-certification via new project or continuing education)

---

## Tier 3B — Brownfield Case Study (Track A Only)

### Format: Real Legacy Module Modernisation + Senior Engineer Review

| Component | Details |
|-----------|---------|
| **Subject** | A real legacy module from the organisation's internal codebase |
| **Duration** | 2 weeks (part-time) |
| **Reviewer** | Senior engineer familiar with the legacy codebase |

### Assessment Rubric

| Criterion | Weight | Description |
|-----------|--------|-------------|
| **Documentation Quality** | 20% | AI-generated docs are accurate, comprehensive, and useful |
| **Dependency Upgrade** | 20% | Upgrade completed successfully with proper impact analysis |
| **Change Request Implementation** | 20% | CR implemented correctly with AI decomposition |
| **AI-Readiness Preparation** | 15% | AGENTS.md, context files, and skills properly configured |
| **Time-Saved Metrics** | 15% | Credible before/after comparison with evidence |
| **Lessons Learned** | 10% | Honest reflection on AI strengths and limitations observed |

### Certification: **AI Legacy Modernisation Specialist Badge** 🏗️
- Track A exclusive
- Issued upon case study completion + senior engineer approval
- Demonstrates practical AI-assisted brownfield development capability

---

## Certification Pathway Summary

```
Tier 1: AI Foundations Badge 🥉
  ↓
Tier 2: AI Practitioner Badge 🥈
  ↓
Tier 3: AI Champion Badge 🥇
  ↓ (Track A only)
Tier 3B: AI Legacy Modernisation Specialist 🏗️
```

---

## Badge Administration

| Aspect | Recommendation |
|--------|---------------|
| **Badge Platform** | Credly, Badgr, or internal LMS badge system |
| **Badge Design** | Track-coloured (Blue/Green/Yellow/Red) + tier symbol |
| **LinkedIn Integration** | Enable shareable digital credentials |
| **Internal Recognition** | Display on employee profiles, team dashboards |
| **Expiry & Renewal** | Tier 1: No expiry. Tier 2: 2 years. Tier 3: 1 year. |
