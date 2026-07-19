# Skill Gap Matrix — Enterprise AI Upskilling Programme

> **Document Version**: 1.0 | **Last Updated**: July 2026  
> **Purpose**: Maps current baseline skills → target AI competency profiles for each role at each proficiency tier.

---

## 1. Role Profiles & Baseline Skills

### 🟦 Developer (Track A) — Baseline
| Skill Area | Current State |
|------------|--------------|
| Programming | Proficient in 1+ languages (Java, C#, Python, JavaScript, TypeScript) |
| Version Control | Git workflows (branching, PRs, merges) |
| Software Architecture | Understanding of design patterns, SOLID principles, microservices vs monolith |
| Testing | Writes unit tests, basic integration tests |
| DevOps | CI/CD basics, Docker/container awareness |
| Debugging | Systematic debugging using IDE tools, logs, stack traces |
| Code Review | Participates in peer code reviews |
| Documentation | Writes README files, inline comments, basic ADRs |

### 🟩 QA Engineer (Track B) — Baseline
| Skill Area | Current State |
|------------|--------------|
| Test Strategy | Creates test plans, test cases, test suites |
| Manual Testing | Exploratory testing, boundary value analysis, equivalence partitioning |
| Automation | Selenium, Playwright, Cypress, or equivalent framework |
| API Testing | Postman, REST-assured, or equivalent |
| Performance Testing | Basic load testing (JMeter, k6) |
| Defect Management | Bug reporting, triage, lifecycle management |
| CI/CD Integration | Integrating test suites into CI pipelines |
| Test Data | Creating and managing test data sets |

### 🟨 Business Analyst (Track C) — Baseline
| Skill Area | Current State |
|------------|--------------|
| Requirements | Elicitation, documentation (BRDs, FRDs, user stories) |
| Stakeholder Management | Facilitation, workshops, interviews |
| Process Modelling | BPMN, flowcharts, swimlane diagrams |
| Data Analysis | Excel/Sheets, basic SQL, pivot tables |
| Visualisation | PowerPoint, basic dashboards |
| Domain Knowledge | Industry-specific business process understanding |
| Agile/Scrum | Works within sprint ceremonies, backlog grooming |
| Communication | Bridges technical and business stakeholders |

### 🟥 AI/ML Developer (Track D) — Baseline
| Skill Area | Current State |
|------------|--------------|
| Programming | Strong Python; may know Java/C++ |
| Mathematics | Linear algebra, calculus, probability & statistics fundamentals |
| Data Handling | SQL, basic data wrangling with Pandas/NumPy |
| Software Engineering | Git, testing, basic CI/CD |
| Cloud | Basic cloud service awareness (AWS/GCP/Azure) |
| APIs | Building and consuming REST APIs |
| Problem Solving | Algorithmic thinking, data structures |
| Research | Reading technical papers, documentation |

---

## 2. Target AI Competency Profiles

### 🟦 Developer (Track A) — Target State
> *"I can build anything 3× faster with AI tools."*

| Competency | Description |
|-----------|-------------|
| AI Tool Mastery | Fluent with GitHub Copilot, Claude Code, and Antigravity IDE for daily coding |
| Prompt Engineering (Tool-Level) | Crafts effective prompts for code generation, debugging, refactoring, and documentation |
| Agentic Workflow Design | Decomposes tasks into AI-manageable chunks; uses plan→execute→verify loops |
| Context Management | Configures .agents/, AGENTS.md, skills, and memory for project-specific AI assistance |
| Critical AI Output Review | Systematically validates AI-generated code for correctness, security, and performance |
| Legacy Modernisation with AI | Uses AI agents to audit, document, upgrade dependencies, and implement changes in brownfield codebases |
| Team AI Practices | Builds shared AI skills/prompts, establishes team coding standards for AI usage |
| AI Productivity Metrics | Measures and reports ROI of AI-assisted development |

### 🟩 QA Engineer (Track B) — Target State
> *"I can break AI systems intelligently and validate non-deterministic outputs."*

| Competency | Description |
|-----------|-------------|
| AI/ML Literacy | Understands supervised/unsupervised/RL, training vs inference, model lifecycle |
| LLM Output Validation | Tests for hallucinations, factual accuracy, format compliance, non-determinism |
| AI Test Generation | Uses AI tools to generate test cases, edge cases, and synthetic test data |
| Adversarial Testing | Red-teams AI systems: prompt injection, jailbreaking, safety boundary testing |
| Bias & Fairness Testing | Tests for demographic parity, discriminatory outputs, equalised odds |
| Model Evaluation Metrics | Interprets precision, recall, F1, BLEU, ROUGE in QA context |
| AI Monitoring | Sets up drift detection, quality degradation alerts for production AI systems |
| AI Test Strategy | Creates test plans and Definition of Done for AI features |

### 🟨 Business Analyst (Track C) — Target State
> *"I think in AI, make informed decisions, and bridge technical teams with business."*

| Competency | Description |
|-----------|-------------|
| AI Literacy | Articulates what AI can/can't do; avoids common misconceptions |
| AI-Ready Requirements | Writes requirements with accuracy thresholds, latency targets, data specs |
| AI Feasibility Assessment | Evaluates technical feasibility, data readiness, build vs buy decisions |
| Data Strategy | Conducts data availability audits, quality assessments, governance reviews |
| AI-Augmented BA Workflows | Uses ChatGPT/Claude for requirements drafting, user stories, stakeholder prep |
| ROI Modelling | Builds cost-benefit analyses for AI initiatives |
| Vendor Evaluation | Reads ML benchmarks, evaluates model cards, assesses AI vendors |
| AI Governance | Understands EU AI Act, NIST AI RMF, responsible AI principles |
| Regulatory Awareness | Navigates industry-specific AI regulations |

### 🟥 AI/ML Developer (Track D) — Target State
> *"I can design, train, deploy, and monitor AI systems in production."*

| Competency | Description |
|-----------|-------------|
| ML/DL Engineering | Builds models using PyTorch/TensorFlow; handles training, tuning, evaluation |
| LLM Fine-Tuning | Applies LoRA, QLoRA, PEFT techniques on pre-trained models |
| RAG Architecture | Designs and builds RAG pipelines with vector databases |
| AI Agent Development | Builds agents with tool use, chains, memory using LangChain/CrewAI/LangGraph |
| MLOps | Manages model versioning, CI/CD for ML, experiment tracking, model registries |
| Production Deployment | Containerises and serves models (FastAPI, vLLM, TGI) |
| Evaluation Frameworks | Implements LLM-as-judge, human eval, automated benchmarking |
| Responsible AI | Applies bias detection, fairness metrics, model interpretability (SHAP, LIME) |
| AI Security | Defends against prompt injection, adversarial attacks; conducts red-teaming |
| Scale & Cost | Manages distributed training, GPU optimisation, cost management |

---

## 3. Proficiency Tier Definitions

### 🟦 Track A — Developers

#### Tier 1: Foundational (Weeks 1–3)
**"Done" looks like:**
- Can explain how LLMs work at a conceptual level (tokens, context windows, probabilistic output)
- Has installed and configured GitHub Copilot, Claude Code, and Antigravity IDE
- Can write basic prompts that generate functional code snippets
- Understands token limits and how to feed context effectively
- **Deliverable**: Completes a coding task (e.g., build a REST API endpoint) using AI tools, documenting prompts used and output quality

#### Tier 2: Intermediate (Weeks 4–8)
**"Done" looks like:**
- Uses AI agents for daily development: scaffolding, debugging, testing, documentation
- Crafts multi-step prompts for complex tasks with system prompts and skills
- Configures .agents/ directory, AGENTS.md, and custom skills for their project
- Critically reviews AI output — identifies incorrect code, security issues, performance problems
- Uses AI for Git workflows (commit messages, PR descriptions, changelogs)
- **Deliverable**: Refactors an existing module using AI agents end-to-end; documents the workflow, time saved, and issues caught

#### Tier 3: Advanced (Weeks 9–12)
**"Done" looks like:**
- Builds and shares custom AI skills/prompts across the team
- Orchestrates multi-agent workflows for large-scale changes
- Establishes team AI coding standards and governance policies
- Understands and mitigates AI security risks (secrets in prompts, code leakage)
- Measures AI-assisted productivity with concrete metrics
- **Deliverable**: Creates a team AI playbook + presents a productivity ROI analysis with before/after metrics

#### Tier 3B: Brownfield & Legacy Modernisation (Weeks 13–16)
**"Done" looks like:**
- Assesses brownfield codebases for AI-readiness (tech debt audit)
- Uses AI agents to document undocumented legacy code
- Performs AI-assisted dependency upgrades with impact analysis and migration code
- Decomposes large CRs into AI-manageable tasks across large codebases
- Prepares legacy codebases for AI-assisted maintenance (AGENTS.md, context files)
- **Deliverable**: Takes a real legacy module → documents it → upgrades one dependency → implements one CR → presents before/after report with time-saved metrics

---

### 🟩 Track B — QA Engineers

#### Tier 1: Foundational (Weeks 1–3)
**"Done" looks like:**
- Can explain supervised vs unsupervised learning, training vs inference
- Understands how LLMs work: tokens, probabilities, hallucinations, non-determinism
- Articulates why traditional test strategies fail for AI (non-deterministic outputs)
- Maps the AI product lifecycle: data → training → evaluation → deployment → monitoring
- **Deliverable**: 20-question MCQ (>80%) + 500-word reflection on "How AI changes my QA practice"

#### Tier 2: Intermediate (Weeks 4–8)
**"Done" looks like:**
- Uses AI tools to generate test cases, edge cases, and synthetic test data
- Tests LLM-powered features: prompt testing, output validation, hallucination detection
- Implements regression strategies for non-deterministic AI outputs
- Uses AI for test automation maintenance (self-healing selectors)
- **Deliverable**: Creates a comprehensive AI test plan for a non-deterministic feature (e.g., chatbot, recommendation engine)

#### Tier 3: Advanced (Weeks 9–12)
**"Done" looks like:**
- Interprets model evaluation metrics (precision, recall, F1, BLEU, ROUGE) in QA context
- Conducts bias & fairness testing with documented methodology
- Performs adversarial testing: prompt injection, jailbreaking, safety boundary testing
- Sets up production monitoring: drift detection, quality degradation alerts
- **Deliverable**: Capstone — cross-functional AI initiative validation (with Dev, BA, AI Dev)

---

### 🟨 Track C — Business Analysts

#### Tier 1: Foundational (Weeks 1–3)
**"Done" looks like:**
- Explains AI/ML in business terms without jargon
- Cites 5+ real-world AI business applications across industries
- Understands AI ethics basics: bias, transparency, accountability
- Maps the AI project lifecycle from a business perspective
- **Deliverable**: 20-question MCQ (>80%) + 500-word reflection on "How AI applies to my role"

#### Tier 2: Intermediate (Weeks 4–7)
**"Done" looks like:**
- Writes AI-ready requirements with success criteria, accuracy thresholds, data requirements
- Conducts data availability audits and quality assessments
- Performs AI feasibility assessments using build vs buy frameworks
- Uses AI tools for requirements drafting, user story generation, stakeholder prep
- **Deliverable**: AI feasibility report with data readiness assessment for a real project

#### Tier 3: Advanced (Weeks 8–10)
**"Done" looks like:**
- Builds ROI models for AI initiatives (cost-benefit, TCO analysis)
- Evaluates AI vendors by reading ML benchmarks and model cards
- Understands EU AI Act, NIST AI RMF, and industry-specific regulations
- Writes AI ethics reviews and incident response plans
- **Deliverable**: Capstone — cross-functional AI initiative business case (with Dev, QA, AI Dev)

---

### 🟥 Track D — AI/ML Developers

#### Tier 1: Foundational (Weeks 1–4)
**"Done" looks like:**
- Builds ML models using scikit-learn (classification, regression, clustering)
- Proficient with NumPy, Pandas, Matplotlib for data work
- Understands data preprocessing, feature engineering, EDA
- Builds basic neural networks with PyTorch or TensorFlow
- **Deliverable**: End-to-end ML project — data loading → EDA → model training → evaluation → prediction

#### Tier 2: Intermediate (Weeks 5–10)
**"Done" looks like:**
- Tracks experiments with MLflow/W&B; performs hyperparameter tuning
- Fine-tunes LLMs using LoRA/QLoRA/PEFT techniques
- Designs system prompts with function calling and structured outputs at the API level
- Builds RAG pipelines with vector databases
- Builds AI agents using LangChain/CrewAI/LangGraph
- Deploys models using FastAPI with containerisation
- **Deliverable**: Builds and deploys a RAG-based application or AI agent with tool use

#### Tier 3: Advanced (Weeks 11–16)
**"Done" looks like:**
- Builds AI-native applications end-to-end
- Designs multi-agent systems with proper communication and task delegation
- Implements evaluation frameworks (LLM-as-judge, automated benchmarking)
- Applies bias detection, fairness metrics, and model interpretability
- Defends against prompt injection and adversarial attacks
- Manages distributed training and GPU cost optimisation
- **Deliverable**: Capstone — cross-functional AI initiative architecture (with Dev, QA, BA)

---

## 4. Skill Gap Matrix — Current State → Target State

### 🟦 Track A — Developers

| Skill Area | Baseline (Current) | Tier 1 Target | Tier 2 Target | Tier 3 Target | Tier 3B Target | Gap Size |
|-----------|-------------------|---------------|---------------|---------------|----------------|----------|
| AI/LLM Understanding | None/minimal | Conceptual understanding | Deep practical understanding | Evaluates new AI tools | Assesses AI-readiness of codebases | Large |
| AI Tool Setup & Config | None | Copilot + Claude Code + Antigravity installed | .agents/ config, custom skills | Team-wide standards | Legacy project AI config | Large |
| Prompt Engineering (Tools) | None | Basic code-gen prompts | Complex multi-step task prompts | Custom shareable skills | Prompts for legacy understanding | Large |
| Context Management | N/A | Understands token limits | Manages context windows effectively | Optimises context across projects | Feeds legacy context to AI | Large |
| AI-Assisted Coding | None | Basic code completion | Full workflow: scaffold→debug→test→doc | Multi-agent orchestration | Legacy code analysis & modification | Large |
| Critical AI Review | Code review skills exist | Spots obvious AI errors | Systematic validation habits | Security & supply chain awareness | Risk assessment for legacy changes | Medium |
| Team AI Practices | N/A | N/A | N/A | Standards, governance, sharing | AI maintenance processes | Large |
| Legacy Modernisation | Manual processes | N/A | N/A | N/A | AI-assisted audit, upgrade, migrate | Large |

### 🟩 Track B — QA Engineers

| Skill Area | Baseline (Current) | Tier 1 Target | Tier 2 Target | Tier 3 Target | Gap Size |
|-----------|-------------------|---------------|---------------|---------------|----------|
| AI/ML Concepts | None/minimal | Core concepts understood | Applied to testing context | Deep evaluation metrics knowledge | Large |
| LLM Understanding | None | Tokens, probabilities, hallucinations | Testing LLM features | Adversarial testing, red-teaming | Large |
| AI Test Strategy | Traditional strategies | Knows why traditional fails for AI | Creates AI test plans | Full AI quality specialisation | Large |
| AI-Powered Test Gen | None | Awareness | Uses AI for test case generation | N/A (uses as standard) | Medium |
| Non-Deterministic Testing | None | Conceptual understanding | Regression strategies for AI | Production monitoring & drift detection | Large |
| Bias & Fairness Testing | None | Ethics awareness | Identifies bias vectors | Formal bias testing methodology | Large |
| Adversarial Testing | None | N/A | Basic prompt testing | Full red-teaming capability | Large |

### 🟨 Track C — Business Analysts

| Skill Area | Baseline (Current) | Tier 1 Target | Tier 2 Target | Tier 3 Target | Gap Size |
|-----------|-------------------|---------------|---------------|---------------|----------|
| AI Literacy | None/minimal | Articulates AI capabilities/limits | Applies AI thinking to analysis | Strategic AI leadership | Large |
| AI-Ready Requirements | Standard requirements | Understands difference | Writes AI-specific requirements | Reviews AI requirements critically | Large |
| Data Strategy | Basic data awareness | Conceptual | Data audits & quality assessment | Full data governance | Medium |
| AI Feasibility | N/A | Understands AI project lifecycle | Conducts feasibility assessments | Build vs buy, vendor evaluation | Large |
| AI Tools for BA | None | Awareness | Uses ChatGPT/Claude for BA tasks | AI-augmented analytics (Copilot, etc.) | Medium |
| AI Governance | None | Ethics basics | Regulatory awareness | EU AI Act, NIST RMF expertise | Large |
| ROI Modelling | Business case skills | N/A | Basic AI cost-benefit | Full TCO & ROI models | Medium |

### 🟥 Track D — AI/ML Developers

| Skill Area | Baseline (Current) | Tier 1 Target | Tier 2 Target | Tier 3 Target | Gap Size |
|-----------|-------------------|---------------|---------------|---------------|----------|
| ML/DL Foundations | Basic Python + math | Scikit-learn + PyTorch basics | Experiment tracking, tuning | End-to-end AI applications | Medium |
| LLM Engineering | None/minimal | Neural network fundamentals | Fine-tuning (LoRA/QLoRA), RAG | Multi-agent systems, evaluation | Large |
| Prompt Engineering (API) | None | N/A | System prompts, function calling | Production prompt management | Large |
| AI Agent Development | None | N/A | Builds agents (LangChain/CrewAI) | Multi-agent architecture | Large |
| MLOps | None/basic DevOps | N/A | Model versioning, CI/CD for ML | Full production monitoring | Large |
| Model Deployment | None | N/A | FastAPI, containerisation | Distributed, GPU-optimised serving | Large |
| Responsible AI | None | N/A | Awareness | Bias detection, SHAP, LIME, security | Large |
| AI Security | None | N/A | N/A | Prompt injection defence, red-teaming | Large |

---

## 5. Gap Prioritisation Summary

| Role | Largest Gaps | Quick Wins (Tier 1) | Highest Impact (Tier 2) | Strategic Value (Tier 3) |
|------|-------------|---------------------|------------------------|-------------------------|
| **Developer** | AI tool mastery, prompt engineering, context management | Tool setup + basic prompts = immediate productivity gains | AI-augmented full development workflow | Team practices + legacy modernisation |
| **QA** | AI literacy, non-deterministic testing, adversarial testing | Understanding why AI breaks traditional testing | AI test plans + LLM output validation | Bias/fairness testing + production monitoring |
| **BA** | AI literacy, AI-ready requirements, governance | Speaking the AI language + ethics awareness | Writing AI-specific requirements + feasibility | ROI modelling + regulatory compliance |
| **AI Dev** | LLM engineering, MLOps, AI agents, production systems | ML/DL fundamentals with hands-on projects | RAG + agents + deployment pipeline | Multi-agent systems + responsible AI at scale |
