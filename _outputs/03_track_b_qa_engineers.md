# Learning Track B — QA Engineers (AI Quality Assurance)

> **Track Colour**: 🟩 Green  
> **Target Audience**: QA engineers (manual, automation, SDET) who need to test AI-powered features, validate LLM outputs, and evolve their testing strategy for AI-era software.  
> **Focus**: Breaking AI systems intelligently — NOT building ML models.  
> **Duration**: 12 weeks (4–6 hrs/week) | **Total Hours**: ~66 hours  
> **Free Content**: ~50% by learning-hours ⚠️ (below the 60% target — see note in the summary table)

---

## Track Overview

```
Week 1–3   → Tier 1: AI Literacy for QA (12–18 hrs)
Week 4–8   → Tier 2: AI-Augmented Testing (20–30 hrs)
Week 9–12  → Tier 3: AI Quality Assurance Specialisation (16–24 hrs)
```

> **Navigation**: QA engineers with existing AI/ML knowledge may take the Tier 1 checkpoint quiz — score >80% to skip to Tier 2.

---

## Tier 1: AI Literacy for QA (Weeks 1–3)

### Module 1.1 — What is AI/ML: Core Concepts for QA

```
📌 Course Title: IBM AI Foundations for Everyone Specialization
🔗 Platform: Coursera
🔗 URL: https://www.coursera.org/specializations/ai-foundations-for-everyone
👤 Instructor: IBM (Rav Ahuja, others)
⏱️ Duration: ~10 hours (3 courses in specialization)
💰 Cost: Free (audit) / $49/month (certificate)
⭐ Rating: 4.7 / 5
👁️ Views / Enrollments: 300K+ enrollments
📅 Last Updated: 2025
🎯 Mapped To: Track B → Tier 1 → AI/ML Core Concepts (QA perspective)
🏷️ Tags: foundational, theory, IBM-backed, specialization
✅ Verified: Yes — public Coursera listing
🔊 Accessibility: Full subtitles, transcripts available
```

**Why this course for QA**: Unlike the developer-focused AI literacy in Track A, this IBM specialization provides a structured overview of AI types (supervised, unsupervised, RL), the AI lifecycle, and practical applications — framed for non-builder professionals who need to understand AI systems they'll test.

**Key modules to focus on:**
- What is AI? Types of AI, model training vs inference
- AI ethics and bias (QA angle: what to test for)
- AI applications and use cases (QA angle: what AI features look like)

---

### Module 1.2 — How LLMs Work: The QA Perspective

```
📌 Course Title: How Large Language Models Work (What QA Needs to Know)
🔗 Platform: YouTube
🔗 URL: https://www.youtube.com/watch?v=5sLYAQS9sWQ
👤 Instructor: IBM Technology (Martin Keen)
⏱️ Duration: ~6 minutes
💰 Cost: Free
📊 Signal: Canonical explainer of token/next-word probability — the root of non-determinism
📅 Last Updated: 2024
🎯 Mapped To: Track B → Tier 1 → LLM Concepts for QA
🏷️ Tags: theory, visual, LLM-specific, QA-framing
✅ Verified: Yes — direct video link confirmed live (Jul 2026)
🔊 Accessibility: Auto-captions available
```

**Direct companion videos (verified live):**
1. *Why Large Language Models Hallucinate* — IBM Technology: https://www.youtube.com/watch?v=cfqtFvWOfg0
2. *How Large Language Models Work* — IBM Technology (primary link above)

---

### Module 1.3 — The AI Product Lifecycle for QA

```
📌 Course Title: How Do You Build MLOps Pipelines on Google Cloud AI?
🔗 Platform: YouTube
🔗 URL: https://www.youtube.com/watch?v=F9bbNgVx0g8
👤 Instructor: Google Cloud Tech
⏱️ Duration: ~10 minutes
💰 Cost: Free
📊 Signal: Walks data→train→deploy→monitor; pair with the Google Cloud doc for test points
📅 Last Updated: Sep 2025
🎯 Mapped To: Track B → Tier 1 → AI Product Lifecycle
🏷️ Tags: lifecycle, process, testing-integration-points
✅ Verified: Yes — direct video link confirmed live (Jul 2026)
🔊 Accessibility: Auto-captions available
```

> **Companion (where testing fits)**: Google Cloud — *MLOps: Continuous delivery and automation pipelines in ML* — https://cloud.google.com/architecture/mlops-continuous-delivery-and-automation-pipelines-in-machine-learning

**Self-Study Exercise**: Map a typical AI product lifecycle to QA activities:
| AI Lifecycle Stage | QA Activity |
|-------------------|-------------|
| Data Collection | Data quality validation, bias check |
| Training | N/A (AI Dev responsibility) |
| Evaluation | Model evaluation metric review |
| Deployment | Integration testing, latency testing |
| Monitoring | Drift detection, quality regression alerts |

---

### 🏁 Tier 1 Checkpoint
- **Quiz**: 20-question MCQ covering AI/ML concepts, LLM behaviour, non-determinism, AI lifecycle
- **Reflection**: 500-word essay on "Why traditional QA strategies fail for AI systems and what must change"
- **Pass criteria**: >80% on quiz + submitted reflection

---

## Tier 2: AI-Augmented Testing (Weeks 4–8)

### Module 2.1 — AI-Powered Test Generation

```
📌 Course Title: [2026] Using Gen AI & AI Agents in Software Automation Testing
🔗 Platform: Udemy
🔗 URL: https://www.udemy.com/course/using-gen-ai-in-software-automation-testing/
👤 Instructor: Rahul Shetty (or equivalent top-rated QA instructor)
⏱️ Duration: ~15 hours
💰 Cost: ₹499–₹799 / $9.99–$14.99 (sale price)
⭐ Rating: 4.5+ / 5 (Bestseller)
👁️ Views / Enrollments: 30K+ students (estimated)
📅 Last Updated: 2026
🎯 Mapped To: Track B → Tier 2 → AI-Powered Test Generation & AI-Assisted Automation
🏷️ Tags: hands-on, project-based, Playwright, test-automation, AI-agents
✅ Verified: ⚠️ Requires verification via Udemy login
🔊 Accessibility: Subtitles available (English)
```

**Key curriculum coverage:**
- Using Copilot and AI tools for test case generation
- Edge case and boundary condition generation with AI
- AI-driven test data synthesis
- Playwright with AI integration
- TestRigor and AI-powered automation
- Self-healing tests and flaky selector management

---

### Module 2.2 — Testing LLM-Powered Features

```
📌 Course Title: AI Agents, RAG & LLM Evals for Beginners: DeepEval & RAGAS
🔗 Platform: Udemy
🔗 URL: https://www.udemy.com/course/ai-testing-deepeval-ragas-ollama/
👤 Instructor: Karthik KK
⏱️ Duration: ~8 hours
💰 Cost: ₹499–₹799 / $9.99–$14.99 (sale price)
⭐ Rating: 4.5+ / 5 (Bestseller)
👁️ Views / Enrollments: 10K+ students (estimated)
📅 Last Updated: 2026
🎯 Mapped To: Track B → Tier 2 → LLM Output Validation, Hallucination Detection, RAG Testing
🏷️ Tags: hands-on, LLM-evaluation, DeepEval, RAGAS, QA-focused
✅ Verified: ⚠️ Requires verification via Udemy login
🔊 Accessibility: Subtitles available (English)
```

**Key curriculum coverage:**
- Testing RAG-based applications
- Hallucination detection and factual accuracy checks
- Using DeepEval and RAGAS evaluation frameworks
- Testing AI agent tool-calling capabilities
- Output format compliance validation

---

### Module 2.3 — Prompt Testing & Input Variation

```
📌 Course Title: LLM Red Teaming Guide (Adversarial & Boundary Prompt Testing)
🔗 Platform: Promptfoo Docs (open source)
🔗 URL: https://www.promptfoo.dev/docs/red-team/
👤 Instructor: Promptfoo
⏱️ Duration: ~2 hours (read + run in CI)
💰 Cost: Free
📊 Signal: Hands-on adversarial input generation you can run in CI/CD (23k+ GitHub stars)
📅 Last Updated: 2026
🎯 Mapped To: Track B → Tier 2 → Prompt Testing
🏷️ Tags: prompt-testing, boundary-testing, adversarial, hands-on
✅ Verified: Yes — link confirmed live (Jul 2026)
🔊 Accessibility: Web-based
```

> **Companion (risk taxonomy)**: OWASP Top 10 for LLM Applications (2025) — https://genai.owasp.org/llm-top-10/. Promptfoo covers adversarial/boundary prompts; drive happy-path input-variation cases from your existing functional test design.

---

### Module 2.4 — Visual Testing with AI

```
📌 Course Title: Overview of Visual UI Testing (Applitools)
🔗 Platform: Applitools Docs (official)
🔗 URL: https://applitools.com/docs/eyes/getting-started/overview
👤 Instructor: Applitools
⏱️ Duration: ~1.5 hours (read + try)
💰 Cost: Free
📊 Signal: Canonical vendor; baseline-capture → screenshot-comparison → review loop
📅 Last Updated: 2025
🎯 Mapped To: Track B → Tier 2 → Visual Testing with AI
🏷️ Tags: visual-testing, UI, anomaly-detection, tools
✅ Verified: Yes — link confirmed live (Jul 2026)
🔊 Accessibility: Web-based
```

> **Free video alternative**: *Modern Functional Test Automation Through Visual AI* — Test Automation University — https://testautomationu.applitools.com/modern-functional-testing/

---

### Module 2.5 — Regression Testing for Non-Deterministic AI Outputs

```
📌 Course Title: Regression Strategies for Non-Deterministic AI (Self-Study Module)
🔗 Platform: Self-curated reading + practice
🔗 URL: N/A (internal exercise)
⏱️ Duration: ~3 hours (reading + creating regression strategy)
💰 Cost: Free
🎯 Mapped To: Track B → Tier 2 → Regression Testing for AI
🏷️ Tags: regression, non-deterministic, strategy, hands-on
```

**Key Concepts:**
- Statistical testing approaches for non-deterministic outputs
- Threshold-based pass/fail criteria (e.g., "output must be factually correct >95% of the time")
- Golden dataset testing: comparing against known-good outputs
- Human-in-the-loop validation workflows
- Snapshot testing for AI responses (range-based, not exact-match)

---

### 🏁 Tier 2 Checkpoint
- **Mini-Project**: Create an AI Test Plan for a non-deterministic feature:
  1. Choose an LLM-powered feature (chatbot, recommendation engine, content generator)
  2. Define acceptance criteria with quantitative thresholds
  3. Design test cases: happy path, edge cases, adversarial inputs
  4. Define regression strategy for non-deterministic outputs
  5. Implement at least 5 automated test cases using DeepEval or RAGAS
  6. Document findings and quality assessment
- **Peer Review**: Submit to a colleague for review

---

## Tier 3: AI Quality Assurance Specialisation (Weeks 9–12)

### Module 3.1 — Model Evaluation Metrics for QA

```
📌 Course Title: Classification Metrics — Accuracy, Precision, Recall, F1
🔗 Platform: Google ML Crash Course (official)
🔗 URL: https://developers.google.com/machine-learning/crash-course/classification/accuracy-precision-recall
👤 Instructor: Google
⏱️ Duration: ~1 hour (read + interactive)
💰 Cost: Free
📊 Signal: Authoritative & interactive for precision/recall/F1
📅 Last Updated: 2025
🎯 Mapped To: Track B → Tier 3 → Model Evaluation Metrics
🏷️ Tags: metrics, evaluation, mathematical, evergreen, official
✅ Verified: Yes — link confirmed live (Jul 2026)
🔊 Accessibility: Web-based
```

> **Companion (BLEU + ROUGE for text)**: Microsoft Learn — *Evaluation metrics* (defines BLEU and ROUGE-N/ROUGE-L with formulas) — https://learn.microsoft.com/en-us/ai/playbook/technology-guidance/generative-ai/working-with-llms/evaluation/list-of-eval-metrics. Optional visual intuition: StatQuest *Confusion Matrix* — https://youtu.be/Kdsp6soqA7o

---

### Module 3.2 — Bias & Fairness Testing

```
📌 Course Title: AI Fairness and Bias Testing: A QA Engineer's Guide
🔗 Platform: Google AI (free resource) + YouTube
🔗 URL: https://ai.google/responsibility/responsible-ai-practices/
👤 Instructor: Google AI Responsibility Team + conference speakers
⏱️ Duration: ~3 hours (reading + videos + practice)
💰 Cost: Free
⭐ Rating: N/A (vendor resource)
👁️ Views / Enrollments: N/A — vendor platform
📅 Last Updated: 2025–2026
🎯 Mapped To: Track B → Tier 3 → Bias & Fairness Testing
🏷️ Tags: bias, fairness, responsible-AI, testing-methodology
✅ Verified: Yes — official Google AI resource
🔊 Accessibility: Web-based, accessible
```

**Key Concepts:**
- Demographic parity testing
- Equalised odds assessment
- Disparate impact analysis
- Testing for discriminatory outputs in text generation
- Bias audit templates and checklists

---

### Module 3.3 — Adversarial Testing & Red-Teaming

```
📌 Course Title: GenAI & AI Agents for QA Test Automation | Copilot & Claude
🔗 Platform: Udemy
🔗 URL: https://www.udemy.com/course/genai-ai-agents-qa-test-automation/
👤 Instructor: Karthik KK (or equivalent QA-focused instructor)
⏱️ Duration: ~10 hours
💰 Cost: ₹499–₹799 / $9.99–$14.99 (sale price)
⭐ Rating: 4.4+ / 5
👁️ Views / Enrollments: 10K+ students (estimated)
📅 Last Updated: June 2026
🎯 Mapped To: Track B → Tier 3 → Adversarial Testing, Red-Teaming, AI Agent Testing
🏷️ Tags: adversarial, red-teaming, prompt-injection, safety, Claude-Code, MCP
✅ Verified: ⚠️ Requires verification via Udemy login
🔊 Accessibility: Subtitles available (English)
```

**Key curriculum coverage:**
- Prompt injection testing techniques
- Jailbreaking and safety boundary testing
- Red-teaming methodologies for AI systems
- Testing AI agent tool-calling for safety
- MCP server security testing
- Claude Code and Copilot for adversarial test automation

---

### Module 3.4 — Performance Benchmarking for AI Systems

```
📌 Course Title: LLM Inference Benchmarking — How Much Does Your LLM Inference Cost?
🔗 Platform: NVIDIA Technical Blog (official)
🔗 URL: https://developer.nvidia.com/blog/llm-inference-benchmarking-how-much-does-your-llm-inference-cost/
👤 Instructor: NVIDIA (Vinh Nguyen, Sergio Perez)
⏱️ Duration: ~1 hour (read)
💰 Cost: Free
📊 Signal: One article covering latency (TTFT/ITL), throughput (TPS/RPS) and cost per 1M tokens
📅 Last Updated: Jun 2025
🎯 Mapped To: Track B → Tier 3 → Performance Benchmarking
🏷️ Tags: performance, latency, throughput, cost, benchmarking
✅ Verified: Yes — link confirmed live (Jul 2026)
🔊 Accessibility: Web-based
```

---

### Module 3.5 — Monitoring AI in Production

```
📌 Course Title: Data Drift in ML — How to Detect and Handle It
🔗 Platform: Evidently AI (open source)
🔗 URL: https://www.evidentlyai.com/ml-in-production/data-drift
👤 Instructor: Evidently AI
⏱️ Duration: ~1.5 hours (read + try the library)
💰 Cost: Free
📊 Signal: Canonical OSS monitoring source; drift detection & quality alerts without labels
📅 Last Updated: 2025
🎯 Mapped To: Track B → Tier 3 → Production AI Monitoring
🏷️ Tags: monitoring, drift-detection, production, observability
✅ Verified: Yes — link confirmed live (Jul 2026)
🔊 Accessibility: Web-based
```

---

### Module 3.6 — Building AI Test Strategies

```
📌 Course Title: AI Test Strategy: Test Plans, Acceptance Criteria, and DoD for AI Features
🔗 Platform: Self-study module (reading + template creation)
🔗 URL: N/A (internal exercise)
⏱️ Duration: ~4 hours
💰 Cost: Free
🎯 Mapped To: Track B → Tier 3 → AI Test Strategy Creation
🏷️ Tags: strategy, test-plan, definition-of-done, templates
```

**Exercise**: Create a comprehensive AI Test Strategy document including:
1. Test scope for AI features (what to test, what not to test)
2. Acceptance criteria templates for non-deterministic systems
3. Definition of Done for AI features
4. Risk-based testing prioritisation for AI components
5. Regression testing policy for model updates
6. Production monitoring and alerting strategy

---

### 🏁 Tier 3 Checkpoint
- **Capstone**: Cross-functional AI initiative (with Dev from Track A, BA from Track C, AI Dev from Track D):
  - QA role: Create comprehensive test strategy, execute adversarial testing, validate bias/fairness, set up monitoring
  - Deliverables: AI test plan, adversarial testing report, bias audit results, monitoring dashboard spec
- **Peer Review**: Cross-functional team reviews each other's contributions

---

## Course Summary Table — Track B

| Module | Course | Platform | Duration | Cost | Tier |
|--------|--------|----------|----------|------|------|
| 1.1 | IBM AI Foundations for Everyone | Coursera | 10 hr | Free (audit) | 1 |
| 1.2 | How LLMs Work (QA Perspective) | YouTube (IBM Technology) | 2 hr | Free | 1 |
| 1.3 | AI/ML Product Lifecycle for QA | YouTube (Google Cloud) | 1.5 hr | Free | 1 |
| 2.1 | Using Gen AI in Automation Testing | Udemy | 15 hr | ₹499–799 | 2 |
| 2.2 | AI Agents, RAG & LLM Evals (DeepEval) | Udemy | 8 hr | ₹499–799 | 2 |
| 2.3 | Prompt Testing / Red-Teaming for QA | Promptfoo | 2 hr | Free | 2 |
| 2.4 | Visual Testing with AI | Applitools | 1.5 hr | Free | 2 |
| 2.5 | Regression for Non-Deterministic AI | Self-study | 3 hr | Free | 2 |
| 3.1 | ML Metrics for QA | Google ML Crash Course | 2 hr | Free | 3 |
| 3.2 | Bias & Fairness Testing | Google AI + YouTube | 3 hr | Free | 3 |
| 3.3 | GenAI & AI Agents for QA (Advanced) | Udemy | 10 hr | ₹499–799 | 3 |
| 3.4 | Performance Benchmarking | NVIDIA Blog | 2 hr | Free | 3 |
| 3.5 | Production AI Monitoring | Evidently AI | 2 hr | Free | 3 |
| 3.6 | AI Test Strategy Creation | Self-study | 4 hr | Free | 3 |

**Track B Total**: ~66 hours | **Free Content**: ~50% | **Paid Content**: 3 Udemy courses (~₹1,500–2,400 / $30–45 total)

> ⚠️ **Below the 60% free-by-hours target.** The three Udemy courses account for ~33 of the ~66 hours. By *module count* the track is ~79% free (11 of 14), but by learner *time* it is ~50%. To clear 60% by hours, consolidate the two overlapping QA-automation Udemy courses (2.2 *DeepEval/RAGAS* and 3.3 *GenAI & AI Agents for QA*) into one, or add free hours.
