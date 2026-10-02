# AI for Software Developers: Competency Assessment
## Track A — Annual Appraisal & Technical Benchmark (Lending Engineering Team)

---

### Executive Overview

This assessment evaluates software developers on **Agentic AI-Assisted Software Development**, based directly on the 16-week training curriculum detailed in [`_outputs/02_track_a_developers.md`](file:///c:/Users/user/Projects/learning-path/_outputs/02_track_a_developers.md). 

While our engineering teams build and maintain products in the **lending domain** (loan origination, credit scoring, EMI calculators, repayment services), **this assessment focuses squarely on developer AI mastery**:
- How LLMs and code models function under the hood (tokens, context windows, probabilistic generation).
- Tool mastery across **GitHub Copilot** (Agent, Plan, and Ask modes), **Claude Code CLI**, and **Google Antigravity IDE**.
- Effective developer prompt engineering, context management (`AGENTS.md`, `CLAUDE.md`, `.agents/`), and Model Context Protocol (MCP).
- Agentic workflows (Plan → Execute → Verify, task decomposition, tool-calling loops).
- AI-assisted debugging (`/explain` → `/fix`), test generation, and critical validation of AI-generated code.
- Advanced multi-agent orchestration, custom skills (`SKILL.md`), developer security (OWASP for LLMs), and DORA productivity metrics.

This assessment serves as a formal input into developers' **Yearly Goals & Appraisals** to evaluate their adoption, efficiency, and safe engineering practices with AI coding tools.

---

### Assessment Structure & Module Mapping

The 60 questions are organized into three tiers reflecting the training progression:

| Assessment Module | Track A Curriculum | Primary AI Coding Focus | Questions | Weight |
|:---|:---|:---|:---:|:---:|
| **[Module 01](file:///c:/Users/user/Projects/learning-path/mcq_questionnaire/01_tier1_foundations_and_tools_mcq.md)** | **Tier 1: AI Foundations & Tool Setup** (Modules 1.1–1.6) | Transformer fundamentals for coders, tokens & embeddings, context window limits ("Lost in the Middle"), Copilot interaction modes (Agent/Ask/Plan), custom instructions, Claude Code CLI, Google Antigravity IDE, prompt engineering for code. | 20 | 25% |
| **[Module 02](file:///c:/Users/user/Projects/learning-path/mcq_questionnaire/02_tier2_augmented_workflows_mcq.md)** | **Tier 2: AI-Augmented Workflows** (Modules 2.1–2.6) | Agentic Plan-Execute-Verify loops, task decomposition, MCP external tool queries, progressive debugging (`/explain` → `/fix`), AI test & doc generation, `AGENTS.md` context standard, PR summaries, and critical review of AI output. | 20 | 40% |
| **[Module 03](file:///c:/Users/user/Projects/learning-path/mcq_questionnaire/03_tier3_advanced_agentic_governance_mcq.md)** | **Tier 3: Advanced Agentic & Team Practices** (Modules 3.1–3.5) | Custom agent skills (`SKILL.md`), multi-agent subagent delegation & context isolation, OWASP Top 10 for LLMs (prompt injection, package hallucination, excessive agency), DORA metrics vs. LOC vanity metrics, team standards & quality gates. | 20 | 35% |
| **Total** | **Full Track A Curriculum** | **Comprehensive AI Competency for Developers** | **60** | **100%** |

---

### Appraisal Grading & Scoring Matrix

$$\text{Final Score} = \left(\frac{\text{Tier 1 Score}}{20} \times 25\%\right) + \left(\frac{\text{Tier 2 Score}}{20} \times 40\%\right) + \left(\frac{\text{Tier 3 Score}}{20} \times 35\%\right)$$

| Score Range | Competency Level | Annual Appraisal Rating | Engineering Action |
|:---:|:---|:---|:---|
| **90% – 100%** | **AI Champion / Lead SME** | **Exceeds Expectations** | Eligible for technical leadership and mentoring. Authorized to author enterprise-wide custom agent skills. |
| **80% – 89%** | **Proficient AI Developer** | **Meets Expectations** | Official pass threshold. Certified to use agentic AI tools across production repositories autonomously. |
| **65% – 79%** | **Developing Practitioner** | **Needs Improvement** | Remediation required on weak modules. Peer review required on AI-assisted pull requests. |
| **< 65%** | **Unsatisfactory** | **Unsatisfactory** | Must re-take core Track A training modules and re-sit the evaluation. |

---

### Navigation

1. **[01_tier1_foundations_and_tools_mcq.md](file:///c:/Users/user/Projects/learning-path/mcq_questionnaire/01_tier1_foundations_and_tools_mcq.md)**: 20 Questions on AI Foundations, Copilot, Claude Code, Antigravity, and Prompting.
2. **[02_tier2_augmented_workflows_mcq.md](file:///c:/Users/user/Projects/learning-path/mcq_questionnaire/02_tier2_augmented_workflows_mcq.md)**: 20 Questions on Agentic Patterns, Debugging, Testing, `AGENTS.md`, and Code Review.
3. **[03_tier3_advanced_agentic_governance_mcq.md](file:///c:/Users/user/Projects/learning-path/mcq_questionnaire/03_tier3_advanced_agentic_governance_mcq.md)**: 20 Questions on Custom Skills (`SKILL.md`), Subagents, OWASP for LLMs, and DORA Metrics.
4. **[04_master_answer_key_and_scoring_guide.md](file:///c:/Users/user/Projects/learning-path/mcq_questionnaire/04_master_answer_key_and_scoring_guide.md)**: Master Answer Key with comprehensive explanations, distractor breakdowns, and scoring guide.
