# Learning Track A — Tier 3B: Brownfield & Legacy Modernisation with AI

> **Track Colour**: 🟦 Blue (Sub-tier)  
> **Target Audience**: Developers who work on existing/legacy codebases and need to use AI agents for modernisation, upgrades, and maintenance.  
> **Prerequisite**: Completion of Track A Tiers 1–3  
> **Duration**: 4 weeks (4–6 hrs/week) | **Total Hours**: ~24 hours  
> **Free Content**: 100% (no paid courses in this tier)

---

## Why Tier 3B Exists

> **This is the highest-impact tier for most enterprises**, because most development teams spend the majority of their time working on existing codebases — not greenfield projects. The skills taught here directly translate to daily productivity gains in real-world legacy maintenance, dependency upgrades, and change request implementation.

---

## Module 3B.1 — Assessing Brownfield Codebases for AI-Readiness

```
📌 Resource: Agentic AI Coding — Best-Practice Patterns for Speed with Quality
🔗 Platform: CodeScene Blog (official)
🔗 URL: https://codescene.com/blog/agentic-ai-coding-best-practice-patterns-for-speed-with-quality
👤 Author: Adam Tornhill (CodeScene founder)
⏱️ Duration: ~30 min (read + apply to your repo)
💰 Cost: Free
📊 Signal: Opens with "Pull Risk Forward: Assess AI Readiness" — code-health audit before agents
📅 Last Updated: Feb 2026
🎯 Mapped To: Track A → Tier 3B → AI-Readiness Assessment
🏷️ Tags: brownfield, tech-debt, assessment
✅ Verified: Yes — link confirmed live (Jul 2026)
🔊 Accessibility: Web-based
```

> **Supplementary (free)**: CodeScene whitepaper — *AI-Ready Code: How Code Health Determines AI Performance* — https://codescene.com/hubfs/whitepapers/AI-Ready-Code-How-Code-Health-Determines-AI-Performance.pdf

**Supplementary Reading:**
- "AI-Driven Modernization: From Concept to Practice" — industry whitepapers
- Sourcegraph blog posts on AI-assisted code understanding
- OpenHands documentation on large codebase SDK

**Self-Study Exercise**: Take an existing project you work on and create an "AI-Readiness Assessment":
1. **Codebase complexity**: Lines of code, number of modules, dependency count
2. **Documentation state**: % of code documented, existence of architecture docs
3. **Test coverage**: Current coverage %, types of tests present
4. **Tech debt indicators**: Outdated dependencies, code smells, complexity hotspots
5. **AI tool compatibility**: Can AI agents parse the code structure? Are there context files?

---

## Module 3B.2 — Using AI Agents to Document Legacy Code

```
📌 Resource: Documenting and Explaining Legacy Code with GitHub Copilot
🔗 Platform: GitHub Blog (official)
🔗 URL: https://github.blog/ai-and-ml/github-copilot/documenting-and-explaining-legacy-code-with-github-copilot-tips-and-examples/
👤 Author: GitHub (Christopher Harrison)
⏱️ Duration: ~30 min (read + practice)
💰 Cost: Free
📊 Signal: Worked example documenting undocumented legacy code via Copilot Chat
📅 Last Updated: Jan 2025
🎯 Mapped To: Track A → Tier 3B → Legacy Code Documentation
🏷️ Tags: documentation, legacy, hands-on, practical, official
✅ Verified: Yes — link confirmed live (Jul 2026)
🔊 Accessibility: Web-based
```

**Hands-On Exercise**: Pick a poorly-documented module from your codebase and use AI agents to:
1. Generate a module overview document
2. Document each public function/method (purpose, parameters, return values)
3. Generate flow diagrams or sequence diagrams
4. Identify and document implicit business rules
5. Create a dependency map

---

## Module 3B.3 — AI-Assisted Dependency Upgrades & Migration

```
📌 Resource: Modernizing Java Projects with GitHub Copilot Agent Mode (Step-by-Step)
🔗 Platform: GitHub Blog (official)
🔗 URL: https://github.blog/ai-and-ml/github-copilot/a-step-by-step-guide-to-modernizing-java-projects-with-github-copilot-agent-mode/
👤 Author: GitHub (Andrea Griffiths)
⏱️ Duration: ~1 hour (read + practice)
💰 Cost: Free
📊 Signal: Scan→assess→dependency updates→javax→jakarta refactor→CVE scan→fix/test loop
📅 Last Updated: Sep 2025
🎯 Mapped To: Track A → Tier 3B → Dependency Upgrades with AI
🏷️ Tags: dependency-management, migration, automation, official
✅ Verified: Yes — link confirmed live (Jul 2026)
🔊 Accessibility: Web-based
```

> **Also verified (other stacks)**: Amazon Q Developer — *Upgrading Java versions* (https://docs.aws.amazon.com/amazonq/latest/qdeveloper-ug/code-transformation.html); OpenRewrite + Claude Code — Moderne blog *From JBoss to Jetty* (https://moderne.ai/blog/writing-openrewrite-recipes-with-ai).

**Hands-On Exercise**: Using AI agents, perform a dependency upgrade on a real project:
1. **Scan**: Use AI to identify outdated dependencies and their upgrade paths
2. **Impact Analysis**: Ask AI to predict what breaks with the upgrade (API changes, deprecations)
3. **Migration Code**: Use AI to generate migration code for breaking changes
4. **Test Generation**: Use AI to generate regression tests for the upgraded dependency
5. **Verify**: Run tests and document results

---

## Module 3B.4 — Handling Complex Change Requests with AI

```
📌 Resource: How Claude Code Works in Large Codebases — Best Practices
🔗 Platform: Anthropic (Claude blog, official)
🔗 URL: https://claude.com/blog/how-claude-code-works-in-large-codebases-best-practices-and-where-to-start
👤 Author: Anthropic
⏱️ Duration: ~30 min (read + practice)
💰 Cost: Free
📊 Signal: Million-line monorepos & legacy systems; plan-then-edit for multi-file changes
📅 Last Updated: 2026
🎯 Mapped To: Track A → Tier 3B → Complex CRs with AI
🏷️ Tags: change-management, cross-cutting, large-codebase, official
✅ Verified: Yes — link confirmed live (Jul 2026)
🔊 Accessibility: Web-based
```

**Key Concepts:**
- Decomposing large CRs into AI-manageable tasks
- Using agentic AI to implement cross-cutting changes
- AI-assisted impact analysis: "what breaks if I change X?"
- Planning and executing multi-file changes with agent supervision

**Hands-On Exercise**: Take a real change request from your backlog and:
1. Decompose it into 5+ AI-manageable sub-tasks
2. Use AI agents to perform impact analysis
3. Implement each sub-task using AI agents
4. Review and validate each change
5. Document the workflow, time spent, and quality of AI output

---

## Module 3B.5 — Making Legacy Projects AI-Ready

```
📌 Resource: AGENTS.md — Open Format for Guiding Coding Agents
🔗 Platform: agents.md (official spec)
🔗 URL: https://agents.md/
👤 Author: Agentic AI Foundation (Linux Foundation)
⏱️ Duration: ~1 hour (read + configure your repo)
💰 Cost: Free
📊 Signal: The de-facto context-file standard; nested-file precedence for monorepos
📅 Last Updated: Continuously maintained
🎯 Mapped To: Track A → Tier 3B → Making Legacy Projects AI-Ready
🏷️ Tags: legacy-modernisation, AI-readiness, configuration, official-standard
✅ Verified: Yes — link confirmed live (Jul 2026)
🔊 Accessibility: Web-based
```

**Key Activities:**
- Adding structured logging and observability points
- Creating API boundaries for AI tool integration
- Refactoring monolithic code for modularity (so AI can reason about components)
- Setting up AGENTS.md, CLAUDE.md, and context files for AI-assisted maintenance
- Creating skill definitions specific to the legacy codebase

**Hands-On Exercise**: Take a legacy module and make it "AI-ready":
1. Add an AGENTS.md file with project context, conventions, and boundaries
2. Add structured context files for key business logic areas
3. Create custom AI skills for common maintenance tasks
4. Document the module's architecture in a format AI tools can consume

---

## Module 3B.6 — Day-to-Day Maintenance Acceleration

```
📌 Resource: Building AI-Powered GitHub Issue Triage with the Copilot SDK
🔗 Platform: GitHub Blog (official)
🔗 URL: https://github.blog/ai-and-ml/github-copilot/building-ai-powered-github-issue-triage-with-the-copilot-sdk/
👤 Author: GitHub (Andrea Griffiths)
⏱️ Duration: ~1 hour (read + build)
💰 Cost: Free
📊 Signal: Builds a real AI issue-triage tool on the Copilot SDK
📅 Last Updated: 2026
🎯 Mapped To: Track A → Tier 3B → Maintenance Acceleration
🏷️ Tags: maintenance, bug-triage, official
✅ Verified: Yes — link confirmed live (Jul 2026)
🔊 Accessibility: Web-based
```

> **Supplements for the other sub-topics**: changelog/release notes → GitHub *Automatically generated release notes* (https://docs.github.com/en/repositories/releasing-projects-on-github/automatically-generated-release-notes); code-health monitoring → CodeScene (https://codescene.com/).

**Key Workflows:**
- AI-assisted bug triage and root-cause analysis in production
- Automated changelog and release note generation
- AI-driven code health monitoring and proactive refactoring suggestions

---

## Module 3B.7 — Case Studies: AI-Powered Legacy Modernisation

```
📌 Resource: Modernizing Applications in Minutes with Amazon Q Developer (Novacomp)
🔗 Platform: AWS Case Studies (official)
🔗 URL: https://aws.amazon.com/solutions/case-studies/novacomp-case-study/
👤 Author: AWS (customer case study)
⏱️ Duration: ~20 min (read)
💰 Cost: Free
📊 Signal: Quantified — Java 8→17, 10k LOC in ~50 min (vs ~3 weeks), ~60% tech-debt cut
📅 Last Updated: 2025
🎯 Mapped To: Track A → Tier 3B → Case Studies
🏷️ Tags: case-studies, real-world, quantified, enterprise
✅ Verified: Yes — link confirmed live (Jul 2026)
🔊 Accessibility: Web-based
```

**More real, verified case studies (direct links):**
- COBOL modernisation — GitHub Blog, *How GitHub Copilot and AI agents are saving legacy systems* (Oct 2025): https://github.blog/ai-and-ml/github-copilot/how-github-copilot-and-ai-agents-are-saving-legacy-systems/
- Mainframe COBOL — IBM Research, *watsonx Code Assistant for Z: the Rosetta Stone for mainframes* (Jun 2025): https://research.ibm.com/blog/watsonx-code-assistant-for-z-is-the-rosetta-stone-for-mainframes
- Reverse-engineering legacy (no source) — InfoQ, *Thoughtworks: From Black Box to Blueprint* (Sep 2025): https://www.infoq.com/news/2025/09/tw-blackbox/

> **Gap note**: verified, quantified public case studies cover **Java** and **COBOL** well. Standalone **.NET** and **Python** case studies of comparable rigour were not found — source these from an internal project or treat as a live demo rather than an external link.

---

## 🏁 Tier 3B Checkpoint — Brownfield Case Study

### Assessment: Real Legacy Module Modernisation

Take a **real legacy module** from an internal codebase and complete the following using AI agents:

| Step | Activity | Expected Output |
|------|---------|----------------|
| 1 | **Document** current behaviour | AI-generated documentation: module overview, function docs, flow diagrams, business rules |
| 2 | **Assess** AI-readiness | AI-readiness assessment with scores across 5 dimensions |
| 3 | **Upgrade** one outdated dependency | Completed upgrade with AI-generated impact analysis, migration code, and test coverage |
| 4 | **Implement** one change request | Completed CR with AI decomposition, implementation, and validation |
| 5 | **Prepare** for AI maintenance | AGENTS.md, context files, custom skills configured for the module |
| 6 | **Report** | Before/after report with time-saved metrics, quality assessment, lessons learned |

### Review Process
- **Self-assessment**: Complete a reflection on AI strengths/weaknesses observed
- **Peer review**: Senior engineer reviews the modernised code, documentation, and report
- **Time tracking**: Compare actual time with estimated manual time for each step
- **Presentation**: 20-minute presentation to team on findings and recommendations

---

## Course Summary Table — Tier 3B

| Module | Topic | Platform | Duration | Cost |
|--------|-------|----------|----------|------|
| 3B.1 | AI-Readiness Assessment | CodeScene Blog | 2 hr | Free |
| 3B.2 | Legacy Code Documentation | GitHub Blog | 2 hr | Free |
| 3B.3 | Dependency Upgrades with AI | GitHub Blog | 3 hr | Free |
| 3B.4 | Complex CRs with AI | Anthropic Blog | 2 hr | Free |
| 3B.5 | Making Legacy AI-Ready | agents.md | 3 hr | Free |
| 3B.6 | Maintenance Acceleration | GitHub Blog | 2 hr | Free |
| 3B.7 | Case Studies | AWS / GitHub / IBM | 4 hr | Free |
| — | Brownfield Case Study | Hands-on project | 6 hr | Free |

**Tier 3B Total**: ~24 hours | **Free Content**: 100%

**Track A Grand Total (Tiers 1–3B)**: ~77 hours | **Free Content**: ~71% | **Paid Content**: 2 Udemy courses (~₹1,000–1,600 / $20–30 total)
