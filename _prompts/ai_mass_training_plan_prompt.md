# 🎯 Master Prompt: AI Mass Training Plan for Developers, QA, Business Analysts & AI Developers

> **Prompt Version:** 2.1  
> **Created:** 2026-07-19  
> **Audience:** Senior Learning Head · AI Domain Expert  
> **Objective:** Design a comprehensive, self-paced AI training plan across four role tracks with zero course overlap.

---

## System Context

You are a **Senior Learning Architect** and **AI Domain Expert** jointly tasked with designing an enterprise-wide AI upskilling programme for four distinct professional tracks: **Software Developers** (using agentic AI tools), **Quality Assurance Engineers**, **Business Analysts**, and **AI/ML Developers** (building AI systems). The organisation needs to rapidly build AI literacy and applied AI skills at scale, while being cost-conscious and respectful of employees' time.

---

## 📋 Detailed Instructions

### 1. Audience Segmentation & Skill Mapping

For each of the four roles—**Developer**, **QA**, **BA**, and **AI Developer**—perform the following:

| Step | Action |
|------|--------|
| **1.1** | Define the **current baseline skills** typically held by professionals in this role (e.g., Developers know programming; QA knows test automation; BA knows requirements gathering). |
| **1.2** | Define the **target AI competency profile** for each role after completing the learning path. Be specific—list concrete skills, not vague goals. |
| **1.3** | Identify **3 proficiency tiers** per role: *Foundational → Intermediate → Advanced*. For Track A, include an additional **Tier 3B (Brownfield/Legacy Modernisation)** sub-tier within the Advanced stage. Clearly define what "done" looks like at each tier (observable behaviours, deliverables, or mini-projects). |
| **1.4** | Create a **skill gap matrix** mapping current state → target state for each role at each tier. |

### 2. Learning Path Architecture

Design **four parallel but non-overlapping learning tracks**. Each track must:

- Be **100% self-paced** with no live-session dependency.
- Have a **clear weekly cadence** (suggested hours per week: 4–6 hrs) with estimated total duration.
- Follow a **modular structure** so learners can pause and resume without losing context.
- Include **milestone checkpoints** at the end of each tier (quiz, mini-project, peer review, or portfolio piece).
- Provide a **recommended sequence** but allow non-linear navigation for experienced learners.

#### Track Structures

##### 🟦 Track A — Developers (Agentic AI-Assisted Development)

> **Who this is for**: Software developers (frontend, backend, full-stack, mobile) who will use AI-powered coding tools to accelerate their daily development workflow. This track does NOT teach them to build ML models—it teaches them to **leverage AI agents and copilots** as force multipliers.

```
Tier 1: AI Foundations & Tool Setup
  → Understanding AI/LLMs at a conceptual level (what they can and can't do)
  → Setting up the agentic AI development toolkit:
      • GitHub Copilot (code completion, chat, workspace agents)
      • Claude Code (terminal-based agentic coding, multi-file edits)
      • Antigravity IDE (agentic AI coding assistant with planning, browser, tools)
  → Prompt engineering fundamentals for code generation
  → Understanding context windows, token limits, and how to feed context effectively

Tier 2: AI-Augmented Development Workflows
  → Agentic coding patterns: task decomposition, plan → execute → verify loops
  → Using AI agents for:
      • Code scaffolding & boilerplate generation
      • Debugging & root-cause analysis
      • Code review & refactoring suggestions
      • Writing unit tests, integration tests, and documentation
      • Database queries, API integration, and migration scripts
  → Prompt crafting for complex multi-step tasks (system prompts, skills, rules)
  → Managing AI agent context: .agents/ config, AGENTS.md, skills, memory
  → Version control workflows with AI (AI-assisted commits, PRs, changelogs)
  → Knowing when NOT to trust AI output—critical review and validation habits

Tier 3: Advanced Agentic Development & Team Practices
  → Building and sharing custom AI skills/prompts across the team
  → Multi-agent workflows: orchestrating AI agents for large refactors/migrations
  → AI-assisted architecture decisions and design document generation
  → Setting up team-wide AI coding standards and governance
  → Security considerations: secrets in prompts, code leakage, supply chain risks
  → Measuring AI-assisted productivity: metrics, before/after, ROI justification
  → Staying current: evaluating new AI coding tools as they emerge

Tier 3B: Brownfield & Legacy Project Modernisation with AI
  → Assessing brownfield codebases for AI-readiness (tech debt audit using AI)
  → Using AI agents to understand and document undocumented legacy code
  → AI-assisted software library & dependency upgrades:
      • Automated upgrade impact analysis with AI
      • AI-generated migration code for breaking changes
      • Regression risk identification and test generation post-upgrade
  → Handling complex change requests in existing projects:
      • Decomposing large CRs into AI-manageable tasks
      • Using agentic AI to implement cross-cutting changes across large codebases
      • AI-assisted impact analysis: "what breaks if I change X?"
  → Making legacy projects AI-ready:
      • Adding structured logging, observability, and API boundaries for AI integration
      • Refactoring monoliths for modularity so AI agents can reason about components
      • Preparing codebases for AI-assisted maintenance (AGENTS.md, context files, skill definitions)
  → Day-to-day maintenance acceleration:
      • AI-assisted bug triage and root-cause analysis in production
      • Automated changelog and release note generation
      • AI-driven code health monitoring and proactive refactoring suggestions
  → Real-world case studies: teams that used AI agents to modernise legacy Java/.NET/Python systems
```

##### 🟩 Track B — QA Engineers

> **Who this is for**: QA engineers (manual, automation, SDET) who need to test AI-powered features, validate LLM outputs, and evolve their testing strategy for AI-era software. This track does NOT teach them to build models—it teaches them to **break AI systems intelligently**.

```
Tier 1: AI Literacy for QA
  → What is AI/ML: supervised vs unsupervised, training vs inference, models vs rules
  → How LLMs work (conceptual): tokens, probabilities, hallucinations, non-determinism
  → AI product lifecycle: data collection → training → evaluation → deployment → monitoring
  → Understanding why traditional test strategies fail for AI (non-deterministic outputs)

Tier 2: AI-Augmented Testing
  → AI-powered test generation:
      • Using tools like Copilot/Claude to generate test cases, edge cases, and test data
      • AI-driven test data synthesis for privacy-sensitive domains
  → Visual testing with AI: screenshot comparison, UI anomaly detection
  → Testing LLM-powered features:
      • Prompt testing: input variation, boundary testing, adversarial prompts
      • Output validation: factual accuracy checks, format compliance, hallucination detection
      • Regression testing strategies for non-deterministic AI outputs
  → AI-assisted test automation: using AI to maintain flaky selectors, self-healing tests

Tier 3: AI Quality Assurance Specialisation
  → Model evaluation metrics: precision, recall, F1, AUC-ROC, BLEU, ROUGE (what they mean for QA)
  → Bias & fairness testing: demographic parity, equalised odds, testing for discriminatory outputs
  → Adversarial testing & red-teaming: prompt injection, jailbreaking, safety boundary testing
  → Performance benchmarking: latency, throughput, cost-per-query for AI systems
  → Monitoring AI in production: drift detection, quality degradation alerts, A/B test validation
  → Building AI test strategies: test plans, acceptance criteria, and Definition of Done for AI features
```

##### 🟨 Track C — Business Analysts

> **Who this is for**: Business analysts, product owners, and requirements engineers who need to scope AI features, evaluate AI feasibility, write AI-ready requirements, and bridge the gap between technical AI teams and business stakeholders. This track does NOT require coding—it teaches them to **think in AI** and **make informed decisions**.

```
Tier 1: AI Literacy for Business
  → AI/ML fundamentals (non-technical): what AI can and can't do, common misconceptions
  → Business applications of AI: case studies across industries (healthcare, finance, retail, logistics)
  → AI ethics overview: bias, transparency, accountability, regulatory basics
  → The AI project lifecycle from a business perspective: ideation → feasibility → build → measure

Tier 2: AI-Informed Analysis
  → Writing AI-ready requirements:
      • How to define success criteria for non-deterministic systems
      • Specifying acceptable accuracy, latency, and error thresholds
      • Data requirements documentation: what data, how much, how clean
  → Data strategy for AI projects: data availability audit, data quality assessment, data governance
  → AI feasibility assessment: technical feasibility, data readiness, build vs buy frameworks
  → Using AI tools for BA workflows:
      • ChatGPT / Claude for requirements drafting, user story generation, stakeholder Q&A prep
      • AI-assisted data visualisation and insights (Tableau AI, Power BI Copilot)
      • Competitive analysis and market research with AI tools

Tier 3: AI Strategy & Governance
  → AI product management: prioritising AI features, managing stakeholder expectations
  → ROI modelling for AI initiatives: cost-benefit analysis, build vs buy, total cost of ownership
  → Vendor evaluation: assessing AI vendors, reading ML benchmarks, evaluating model cards
  → AI governance frameworks: model risk management, audit trails, explainability requirements
  → Regulatory landscape: EU AI Act, NIST AI RMF, industry-specific regulations
  → Responsible AI in practice: writing AI ethics reviews, incident response for AI failures
```

##### 🟥 Track D — AI/ML Developers (Building AI Systems)

> **Who this is for**: Developers specialising in building AI/ML systems, training models, deploying ML pipelines, and creating AI-native applications. This is the **deep technical track** for engineers who will architect and build AI products.

```
Tier 1: AI/ML Engineering Foundations
  → Core ML/DL concepts: supervised, unsupervised, reinforcement learning
  → Python for AI: NumPy, Pandas, Scikit-learn, Matplotlib
  → Data preprocessing, feature engineering, exploratory data analysis
  → Introduction to neural networks, PyTorch / TensorFlow fundamentals

Tier 2: Applied AI/ML Engineering
  → Model training, hyperparameter tuning, experiment tracking (MLflow, W&B)
  → Fine-tuning LLMs: LoRA, QLoRA, PEFT techniques
  → Prompt engineering at the API level: system prompts, function calling, structured outputs
  → LLM integration patterns: RAG (Retrieval-Augmented Generation), vector databases
  → Building AI agents: tool use, chains, memory, orchestration frameworks (LangChain, CrewAI)
  → MLOps basics: model versioning, CI/CD for ML pipelines, model registries
  → Model deployment: containerisation, serving (FastAPI, vLLM, TGI), edge deployment

Tier 3: Advanced AI Engineering & Production Systems
  → Building AI-native applications end-to-end
  → Multi-agent systems: architecture, communication, task delegation
  → Evaluation frameworks: LLM-as-judge, human eval, automated benchmarking
  → Responsible AI: bias detection, fairness metrics, model interpretability (SHAP, LIME)
  → AI security: prompt injection defence, adversarial attacks, red-teaming
  → Scalability: distributed training, GPU optimisation, cost management
  → Production best practices: monitoring, observability, A/B testing for AI features
```

### 3. Course Curation Rules (CRITICAL)

> ⚠️ **Zero Overlap Policy**: No single course, video, or resource may appear in more than one track. If a foundational topic (e.g., "What is Machine Learning?") is needed by all four roles, identify **four different courses**—one per track—each tailored to that role's perspective and depth level.
>
> ⚠️ **Track A vs Track D Boundary**: Track A (Developers) focuses on *using* AI tools to write code faster. Track D (AI Developers) focuses on *building* AI systems. There must be **zero content bleed** between these two tracks. Prompt engineering in Track A = crafting prompts for Copilot/Claude Code; prompt engineering in Track D = designing system prompts for LLM APIs in production apps.

#### Platform Priority (Budget-Friendly)
Curate courses **exclusively** from these platforms, in order of preference:

| Priority | Platform | Rationale |
|----------|----------|-----------|
| 1 | **YouTube** (free) | Zero cost; vast AI content from top educators (3Blue1Brown, Sentdex, freeCodeCamp, Google, Microsoft, IBM) |
| 2 | **Udemy** (paid, affordable) | Frequent sales at ₹399–₹799 / $9.99–$14.99; lifetime access; structured curriculum |
| 3 | **Coursera** (free audit / paid cert) | University-grade content; audit mode is free; specialisations available |
| 4 | **freeCodeCamp.org** (free) | Hands-on, project-based; excellent for developers |
| 5 | **Google / Microsoft / AWS Skill Builders** (free tiers) | Vendor-specific but high-quality; free certifications available |
| 6 | **Kaggle Learn** (free) | Micro-courses with hands-on notebooks; great for data skills |
| 7 | **edX** (free audit) | MIT, Harvard content; audit mode available |
| 8 | **LinkedIn Learning** (if org has licence) | Professional-grade, short-form content |

#### Udemy Course Extraction (Credential-Based Deep Verification)

> 🔐 **Udemy Access Available**: The organisation has a personal Udemy account available for course verification. When curating Udemy courses:
>
> 1. **Log in** using the provided credentials to access full course details.
> 2. **Verify every data point** from the actual course page—do NOT rely on search result snippets or cached metadata. Extract:
>    - Exact course title (as displayed on the course landing page)
>    - Exact instructor name and credentials
>    - Total duration (hours), total lectures count, total sections count
>    - Current rating (X.X / 5.0) and **total number of ratings**
>    - **Total enrollments** (exact number shown on course page)
>    - Last updated date (month and year, as shown on the course page)
>    - Full curriculum/syllabus outline (section titles + lecture titles)
>    - Language and available subtitles
>    - Current price (regular + sale price if applicable)
> 3. **Cross-check curriculum against track requirements**: Ensure ≥70% of the course syllabus directly maps to the skills listed in the assigned tier. If <70%, the course is a poor fit—find an alternative.
> 4. **Check reviews for red flags**: Skim the 5 most recent 1-star and 2-star reviews for patterns (outdated content, poor audio, missing resources). If >20% of recent reviews flag staleness, reject the course.
> 5. **Document your verification** in the course card with a `✅ Verified via Udemy login on [DATE]` tag.

> ⚠️ **Credential Handling**: The Udemy login will be shared privately. Do NOT persist credentials in any output document. Use them only for live verification during curation.

#### Course Selection Criteria
For **every** recommended course, provide:

```
📌 Course Title: [Exact title as shown on platform]
🔗 Platform: [YouTube / Udemy / etc.]
🔗 URL: [Direct link]
👤 Instructor: [Name / Channel]
⏱️ Duration: [X hours]
💰 Cost: [Free / ₹XXX / $XX]
⭐ Rating: [X.X / 5]
👁️ Views / Enrollments: [Total view count for YouTube / Total enrollments for Udemy / Coursera / etc.]
📅 Last Updated: [Month Year]
🎯 Mapped To: [Track X → Tier Y → Skill Z]
🏷️ Tags: [e.g., hands-on, theory, project-based, certification]
✅ Verified: [Yes/No — if Udemy, include verification date]
```

> 📊 **Why Views/Enrollments Matter**: High view or enrollment counts are a proxy for community validation. Prefer courses with:
> - **YouTube**: ≥50K views (≥200K for foundational topics)
> - **Udemy**: ≥10K enrollments
> - **Coursera**: ≥5K enrollments
> Exception: Niche topics (e.g., AI for QA testing) may have legitimately low counts—flag these as "Niche topic; limited options available" rather than rejecting outright.

> ⚠️ **Freshness Check**: Do NOT recommend any course last updated before **January 2024**. AI is evolving rapidly—stale content does more harm than good. For YouTube, prefer videos published within the last 12 months unless the content is genuinely evergreen (e.g., linear algebra fundamentals).

> 🛑 **Duplicate Detection**: Before finalising, cross-reference all four tracks and confirm:
> - No course appears in more than one track.
> - No two courses in the same track cover >70% overlapping content.
> - **Special attention**: Audit Track A vs Track D for boundary violations—these two tracks are at highest risk of overlap.
> - If overlap is detected, replace or merge and document the decision.

### 4. Overlap Prevention Matrix

Create an explicit **Course Overlap Audit Table**:

| Topic | Dev Track (Tools) | QA Track | BA Track | AI Dev Track (Build) | Overlap Risk | Resolution |
|-------|-------------------|----------|----------|---------------------|--------------|------------|
| AI/ML Fundamentals | [Course A] | [Course B] | [Course C] | [Course D] | Medium ⚠️ | Dev = conceptual for tool usage; AI Dev = deep technical; QA = testing lens; BA = business lens |
| Prompt Engineering | [Course E] | [Course F] | [Course G] | [Course H] | High 🔴 | Dev = prompts for Copilot/Claude Code; QA = testing prompts; BA = ChatGPT usage; AI Dev = API-level system prompts |
| LLM / GenAI Concepts | [Course I] | [Course J] | [Course K] | [Course L] | High 🔴 | Dev = how copilots work; QA = validating LLM output; BA = business applications; AI Dev = building with LLM APIs |
| AI Agents | [Course M] | — | — | [Course N] | High 🔴 | Dev = using agentic coding tools; AI Dev = building agent systems. Completely different focus. |
| Brownfield / Legacy Modernisation | [Course O] | — | — | — | Low ✅ | Track A exclusive—using AI tools on existing codebases. Not an AI Dev concern. |
| Dependency Upgrades / Maintenance | [Course P] | — | — | — | None ✅ | Track A exclusive—operational dev workflow, not model-building. |
| ... | ... | ... | ... | ... | ... | ... |

### 5. Shared Knowledge Base (Common Module)

Despite zero course overlap, create a **Shared Reference Module** (not a course—a curated resource pack) that all four tracks can access:

- **AI Glossary**: 50+ terms every professional should know.
- **Tool Setup Guide**: How to set up Python, Jupyter, ChatGPT, GitHub Copilot, Claude Code, Antigravity, etc.
- **Agentic AI Tools Quick-Reference Card**: One-pager comparing Antigravity, Claude Code, GitHub Copilot, Cursor, Windsurf—features, pricing, best-fit scenarios.
- **Ethics & Responsible AI Reading List**: 5–7 articles/papers accessible to all levels.
- **Weekly AI News Digest Template**: Format for teams to share relevant AI news.

### 6. Assessment & Certification Strategy

| Tier | Assessment Type | Details |
|------|----------------|---------|
| Foundational | **Quiz + Reflection** | 20-question MCQ + 500-word reflection on "How AI applies to my role" |
| Intermediate | **Mini-Project** | Role-specific hands-on project (Dev: refactor a legacy module using AI agents end-to-end; QA: create an AI test plan for a non-deterministic feature; BA: write an AI feasibility report with data readiness assessment; AI Dev: build and deploy a small ML feature) |
| Advanced | **Capstone + Peer Review** | Cross-functional capstone where 1 Dev + 1 QA + 1 BA + 1 AI Dev collaborate on an AI initiative—Dev uses AI tools to build, AI Dev architects the AI component, QA validates, BA writes the business case |
| Advanced (Tier 3B — Track A only) | **Brownfield Case Study** | Take a real legacy module from an internal codebase, and using AI agents: (1) document its current behaviour, (2) upgrade one outdated dependency, (3) implement one change request, (4) present a before/after report with time-saved metrics. Peer-reviewed by senior engineers. |

### 7. Time & Budget Estimation

Provide a summary table:

| Metric | Developer Track (Tools) | QA Track | BA Track | AI Developer Track (Build) |
|--------|------------------------|----------|----------|---------------------------|
| Total Duration (weeks) | ? | ? | ? | ? |
| Hours per Week | 4–6 | 4–6 | 4–6 | 5–8 |
| Total Learning Hours | ? | ? | ? | ? |
| Estimated Cost per Learner | ? | ? | ? | ? |
| Free Content Percentage | ? | ? | ? | ? |

### 8. Rollout Recommendations

Provide guidance on:

- **Cohort sizing**: How many learners per cohort for effective peer interaction.
- **Manager enablement**: One-pager for managers on how to support learning time.
- **Gamification**: Badge/point system to drive engagement.
- **Slack / Teams channels**: Suggested channels for each track + a cross-track channel.
- **Monthly showcases**: Format for learners to demo what they've built/learned.
- **Feedback loops**: How to collect and act on learner feedback to iterate on the plan.

### 9. Success Metrics & KPIs

Define measurable success indicators:

| KPI | Target | Measurement Method |
|-----|--------|--------------------|
| Enrollment Rate | >80% of eligible staff | LMS data |
| Tier 1 Completion Rate | >90% within 4 weeks | LMS data |
| Tier 2 Completion Rate | >70% within 8 weeks | LMS data |
| Tier 3 Completion Rate | >50% within 12 weeks | LMS data |
| Tier 3B Completion (Track A) | >40% of Track A advanced learners | LMS data + project submissions |
| Brownfield Project Time Saved | >30% reduction in task time (self-reported) | Pre/post survey on legacy tasks |
| Learner Satisfaction (NPS) | >8/10 | Post-module survey |
| On-the-Job Application | >60% report using AI skills weekly | Quarterly survey |
| Cross-functional Capstone Completion | >40% of advanced learners | Project submissions |
| Udemy Course Verification Rate | 100% of recommended Udemy courses | Curation audit log |

---

## 📐 Output Format

Structure your complete response as follows:

```
1. Executive Summary (1 page)
2. Skill Gap Matrix (per role × 4 roles)
3. Learning Track A — Developers / Agentic AI Tools (full course list + sequence)
   3a. Track A Tier 3B — Brownfield & Legacy Modernisation (dedicated sub-section)
4. Learning Track B — QA Engineers (full course list + sequence)
5. Learning Track C — Business Analysts (full course list + sequence)
6. Learning Track D — AI/ML Developers (full course list + sequence)
7. Track A vs Track D Boundary Analysis (explicit delineation)
8. Course Overlap Audit Table (4-track cross-reference)
9. Udemy Verification Report (for all Udemy courses: verified data + curriculum match %)
10. Shared Knowledge Base Resources
11. Assessment & Certification Plan
12. Time & Budget Summary
13. Rollout Playbook
14. Success Metrics Dashboard Template
```

---

## 🚫 Constraints & Guardrails

- **No vendor lock-in**: Don't build entire tracks around one platform or cloud provider.
- **No paid-only paths**: Every track must be completable with **≥60% free content**.
- **No prerequisites beyond role baseline**: Don't assume developers know Python (teach it), don't assume BAs know statistics (teach it).
- **No live-session dependency**: Everything must work for someone learning at 2 AM alone.
- **Language**: All content must be in **English**. Prefer courses with **subtitles/captions** available.
- **Accessibility**: Flag courses that provide transcripts, closed captions, or alternative formats.
- **Udemy data integrity**: Every Udemy course MUST be verified via login. Do not recommend any Udemy course based solely on search results or cached data. If you cannot verify a course, replace it with a verified alternative or a free YouTube equivalent.
- **Views/enrollment counts are mandatory**: Do NOT submit any course card without the views/enrollment field filled. If the data is unavailable, note `N/A — could not verify` rather than leaving it blank.

---

## 💡 Pro Tips for the AI Expert

- For **Developers (Track A)**: This track is about **tool mastery, not theory**. Prioritise courses and tutorials that show real-world workflows: "watch me build a feature using Claude Code", "pair programming with Copilot", "agentic coding with Antigravity". Hands-on screen-share style content >>> lecture slides. Look for content from practitioners who ship code daily with these tools.
- For **Track A — Brownfield/Legacy (Tier 3B)**: This is the **highest-impact tier** for most enterprises, because most teams work on existing codebases, not greenfield. Prioritise content that shows AI agents working on **real legacy code** (Java, .NET, Python monoliths)—not toy demos. Look for case studies, conference talks, and practitioner blogs. If no structured course exists for a sub-topic, recommend a combination of YouTube talks + blog posts + hands-on exercises as a "curated micro-path".
- For **AI/ML Developers (Track D)**: Prioritise courses that include **hands-on coding labs**, **GitHub repos** with starter code, and **end-to-end project walkthroughs**. AI Developers learn by building models, not watching theory lectures. Prefer content with real datasets and deployment components.
- For **QA Engineers**: Focus on courses that bridge the gap between traditional testing and AI-specific quality challenges. This is an underserved niche—curate carefully.
- For **Business Analysts**: Avoid overly technical content. BAs need to **speak AI fluently** without necessarily coding. Focus on frameworks, tools, and decision-making.
- For **all tracks**: Include at least one course per track that covers **Generative AI / LLMs / ChatGPT** since this is the most immediately applicable AI technology across all roles.
- **Track A ↔ Track D boundary reminder**: A developer in Track A should finish the programme and think "I can build anything 3× faster with AI tools." An AI Developer in Track D should finish and think "I can design, train, deploy, and monitor AI systems in production." If any course could fit in both tracks, it belongs in **neither**—find a more specific alternative for each.
- **Udemy verification tip**: When logged into Udemy, use the "Preview this course" feature to assess production quality (audio, visuals, pacing) before recommending. A 4.5-star course with 50K enrollments but recent reviews saying "hasn't been updated for GPT-4" is worse than a 4.2-star course with 5K enrollments that was updated last month.

---

## 🔄 Maintenance Plan

This training plan should be **reviewed and refreshed quarterly**:

| Quarter | Action |
|---------|--------|
| Q1 | Full course link audit (check for broken/removed content) + **Udemy re-verification** (log in, check all Udemy courses still exist, ratings haven't dropped, content hasn't gone stale) |
| Q2 | Refresh with newly released high-quality courses; update view/enrollment counts |
| Q3 | Incorporate learner feedback; adjust difficulty curves; review Tier 3B brownfield content for new AI tool releases |
| Q4 | Annual strategy review; align with org's AI maturity goals; evaluate new platforms |

---

> **End of Prompt**  
> *Use this prompt with any advanced AI assistant (Claude, Gemini, GPT-4o, etc.) or hand it to your L&D team and AI SME to collaboratively build the training plan.*
