# Track A vs Track D — Boundary Analysis

> **Purpose**: Explicit delineation between Track A (Developers using AI tools) and Track D (AI/ML Developers building AI systems) to prevent content bleed.  
> **Risk Level**: 🔴 HIGH — These two tracks are at highest risk of overlap.

---

## Core Distinction

| Dimension | Track A (Developers) | Track D (AI/ML Developers) |
|-----------|---------------------|---------------------------|
| **End Goal** | "I use AI coding tools to ship faster with less toil" | "I can design, train, deploy, and monitor AI systems in production" |
| **Relationship to AI** | **Consumer** of AI tools | **Builder** of AI systems |
| **AI Models** | Uses pre-trained models via tools (Copilot, Claude Code) | Trains, fine-tunes, and deploys models |
| **Prompt Engineering** | Crafting prompts for coding assistants | Designing system prompts for LLM APIs in production apps |
| **AI Agents** | Uses agentic coding tools (Antigravity, Claude Code) | Builds agent systems (LangChain, CrewAI, LangGraph) |
| **Code Generation** | AI generates code for the developer to review | Developer writes code that generates/processes AI outputs |
| **Security** | Avoiding secrets in prompts, code leakage, supply chain | Defending against prompt injection, adversarial attacks |
| **Testing** | Using AI to generate tests for their code | Building evaluation frameworks for AI systems |
| **Deployment** | Ships features using AI-assisted development | Ships AI models and ML pipelines |
| **Metrics** | Developer productivity (time saved, code quality) | Model performance (accuracy, latency, cost) |

---

## Topic-by-Topic Boundary Map

### 1. AI Fundamentals

| Aspect | Track A | Track D |
|--------|---------|---------|
| **Course** | 3Blue1Brown "But what is a GPT?" (visual, conceptual) | Andrew Ng Machine Learning Specialization (mathematical, hands-on) |
| **Depth** | Conceptual: "How do tokens and context windows affect my prompts?" | Technical: "How does backpropagation update weights during training?" |
| **Outcome** | Understands AI tool capabilities/limitations | Can implement ML algorithms from scratch |

### 2. Prompt Engineering

| Aspect | Track A | Track D |
|--------|---------|---------|
| **Course** | Prompt Engineering for Coding Tools (YouTube practitioner content) | ChatGPT Prompt Engineering for Developers (Coursera, Andrew Ng + OpenAI) |
| **Context** | Prompts typed into Copilot Chat, Claude Code terminal, Antigravity IDE | System prompts in API calls (OpenAI, Anthropic), function calling schemas |
| **Examples** | "Refactor this function to use async/await and add error handling" | `{"role": "system", "content": "You are a medical triage assistant..."}` |
| **Outcome** | Gets better code suggestions from AI tools | Designs production prompt templates for LLM-powered applications |

### 3. AI Agents

| Aspect | Track A | Track D |
|--------|---------|---------|
| **Course** | GitHub Copilot courses (Agent Mode), Claude Code tutorials | AI Agents in LangGraph (freeCodeCamp), Multi-Agent Systems (Udemy) |
| **Relationship** | Uses agent features: Plan Mode, Agent Mode, `/goal` commands | Builds agent architectures: tool registration, memory, state management |
| **Configuration** | AGENTS.md, .agents/ directory, custom skills files | LangChain chains, LangGraph state graphs, CrewAI crew definitions |
| **Outcome** | "I activated Agent Mode and it autonomously fixed 3 bugs" | "I built a customer support agent with RAG, tool use, and memory" |

### 4. Context / RAG

| Aspect | Track A | Track D |
|--------|---------|---------|
| **Track A** | Feeding project context to AI tools via AGENTS.md, custom instructions, workspace indexing | N/A |
| **Track D** | N/A | Building RAG pipelines with vector databases, chunking strategies, hybrid search |
| **Overlap Risk** | None — completely different systems | None |

### 5. Multi-Agent / Multi-File Operations

| Aspect | Track A | Track D |
|--------|---------|---------|
| **Track A** | Orchestrating AI coding tools to make changes across multiple files in a codebase | N/A |
| **Track D** | N/A | Designing multi-agent architectures where multiple AI agents communicate and delegate tasks |
| **Overlap Risk** | Low — "multi-agent" means different things in each track | Low |

### 6. Security

| Aspect | Track A | Track D |
|--------|---------|---------|
| **Track A** | Don't paste API keys into AI prompts. Don't trust AI-generated dependency suggestions blindly. Review AI code for vulnerabilities. | N/A |
| **Track D** | N/A | Implement input sanitisation for prompts. Build guardrails against jailbreaking. Defend against adversarial inputs. Test for data extraction attacks. |
| **Overlap Risk** | None — different threat models entirely | None |

### 7. Testing with AI

| Aspect | Track A | Track D |
|--------|---------|---------|
| **Track A** | Using AI tools to generate unit tests, integration tests for the code the developer writes | N/A |
| **Track D** | N/A | Building evaluation frameworks (LLM-as-judge, automated benchmarking) for AI models |
| **Overlap Risk** | None — "test generation" ≠ "model evaluation" | None |

### 8. MLOps / DevOps

| Aspect | Track A | Track D |
|--------|---------|---------|
| **Track A** | Standard DevOps (CI/CD, Docker) — may use AI to help write pipeline configs | N/A |
| **Track D** | N/A | ML-specific ops: experiment tracking (MLflow), model versioning, model registries, ML pipeline CI/CD |
| **Overlap Risk** | Low — Track A DevOps is standard software; Track D is ML-specific | Low |

---

## Course Cross-Reference Audit

| Course | Track | Justification for Assignment |
|--------|-------|----------------------------|
| 3Blue1Brown "But what is a GPT?" | A only | Visual, conceptual — helps developers understand their tools |
| GitHub Copilot Beginner to Pro (Udemy) | A only | Tool mastery course — no ML engineering content |
| GitHub Copilot Complete Guide 2026 (Udemy) | A only | Advanced tool usage — agentic workflows, MCP |
| Claude Code Full Course (YouTube) | A only | Terminal-based AI coding tool — using, not building |
| Anthropic Claude Code 101 (Skilljar) | A only | Official tool training — not model building |
| Microsoft Learn: Copilot Agent Mode | A only | Building apps *with* Copilot — not building AI systems |
| Machine Learning Specialization (Coursera) | D only | Deep ML theory + math + implementation |
| Kaggle Learn Micro-Courses | D only | Hands-on Python/ML implementation |
| Hugging Face LLM Course | D only | Fine-tuning models — not using pre-built tools |
| ChatGPT Prompt Engineering for Developers (Coursera) | D only | API-level prompt design — not tool-level |
| LangChain & RAG (Udemy) | D only | Building RAG systems — not using built-in RAG |
| AI Agents in LangGraph (freeCodeCamp) | D only | Building agent architectures — not using agent tools |
| MLOps Zoomcamp | D only | ML pipeline ops — not standard DevOps |
| Full Stack LLM Bootcamp | D only | Production LLM systems — not using coding assistants |
| Multi-Agent AI Systems (Udemy) | D only | Agent system architecture — not multi-file code editing |

**Result**: ✅ Zero overlap detected between Track A and Track D course lists.

---

## Decision Rule: "Could This Course Fit in Both Tracks?"

If you encounter a course during quarterly refresh that *could* fit in either track, apply this test:

1. **Does the course teach you to USE an AI tool, or BUILD an AI system?**
   - USE → Track A
   - BUILD → Track D

2. **Does the course involve writing code that CALLS AI APIs, or code that IS ABOUT the developer's own project?**
   - Calls AI APIs → Track D
   - About the developer's project, with AI as assistant → Track A

3. **Does the course require understanding of ML theory (loss functions, gradients, attention mechanisms)?**
   - Yes → Track D
   - No → Track A

4. **If it fails all three tests (genuinely ambiguous), it belongs in NEITHER track.** Find a more specific alternative for each.

---

## Visual Boundary

```
┌──────────────────────────────────────────────────────────────┐
│                    THE AI BOUNDARY LINE                       │
│                                                              │
│  Track A (LEFT SIDE)          │  Track D (RIGHT SIDE)        │
│  ─────────────────           │  ─────────────────          │
│                               │                              │
│  Developer writes code        │  Developer writes AI code    │
│  AI tool helps them           │  AI IS the product           │
│                               │                              │
│  "Copilot, refactor this"     │  "Build a RAG pipeline"      │
│  "Claude, write tests"        │  "Fine-tune this LLM"        │
│  "Antigravity, plan this CR"  │  "Deploy this model to prod" │
│                               │                              │
│  Prompt → Code Suggestion     │  System Prompt → API Call    │
│  Agent Mode → Auto-fix        │  Agent → Tool Use Chain      │
│  AGENTS.md → Context          │  Vector DB → RAG retrieval   │
│                               │                              │
│  OUTPUT: Better software      │  OUTPUT: AI systems          │
│  METRIC: Time saved           │  METRIC: Model accuracy      │
└──────────────────────────────────────────────────────────────┘
```
