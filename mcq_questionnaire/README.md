# Enterprise AI-Assisted Engineering Competency Assessment (India Lending: Loan Origination & Credit Rating)
## Track A: Developers — Annual Appraisal & SME Benchmark Questionnaire (BFSI India)

---

### Executive Overview & Strategic Intent

As part of the Global Technology Learning & Development framework and Enterprise Engineering Performance Standards, this assessment benchmarks software engineers on **Agentic AI-Assisted Software Engineering** within mission-critical **Indian Lending Platforms (Loan Origination Systems [LOS] & Credit Rating/Decisioning)** across banks and Non-Banking Financial Companies (NBFCs / Fintechs).

In India's hyper-scale digital lending landscape, software engineering directly powers:
- **Loan Origination Systems (LOS)**: Digital customer onboarding, India Stack integrations (Aadhaar e-KYC / Masked Aadhaar, PAN verification via NSDL/ITD, DigiLocker, CKYC/CERSAI, Account Aggregator [AA] cashflow consent flows, Video-KYC [V-KYC]).
- **Credit Rating & Bureau Integration**: Multi-bureau orchestration across RBI-licensed Credit Information Companies (CIBIL / TransUnion, Experian India, Equifax India, CRIF High Mark), CIR (Credit Information Report) parsing, trade-line DPD string analysis, and internal Credit Decisioning Engines (BRE / Scorecards).
- **Underwriting & Financial Metrics**: Indian lending metrics including Fixed Obligation to Income Ratio (**FOIR**), Loan to Value (**LTV**), GSTN data analysis (GSTR-1 / 3B invoice validation for MSME), and internal risk grading models.
- **Regulatory Mandates & Repayment**: **RBI Digital Lending Guidelines (DLG)**, mandatory **Key Fact Statement (KFS)** and Annual Percentage Rate (**APR**) disclosures, **DPDP Act 2023** (Digital Personal Data Protection), RBI Data Localisation directives, **e-NACH / NPCI UPI AutoPay** mandate registration, and **NeSL digital e-Sign**.

Developer productivity gains from Generative AI and Agentic tools (such as **GitHub Copilot**, **Claude Code**, and **Google Antigravity**) must strictly adhere to RBI regulatory compliance, data localization, zero-trust security, exact financial calculations in Indian Rupees (INR), and borrower data sovereignty. This assessment evaluates practical, real-world mastery across the 16-week curriculum detailed in [`_outputs/02_track_a_developers.md`](file:///c:/Users/user/Projects/learning-path/_outputs/02_track_a_developers.md).

This evaluation is an official input into:
1. **Yearly Performance Goals & Appraisals**: Quantitative metric for the "Engineering Excellence & AI Productivity in India Lending Systems" goal.
2. **Technical Career Ladder Advancement**: Prerequisite for promotions to Senior Software Engineer, Technical Lead, and Principal Lending Architect.
3. **Engineering License to Practice**: Mandatory clearance to utilize Enterprise Agentic AI tooling on Tier-1 Indian Loan Origination, Bureau Parsing, and Underwriting Decisioning repositories.

---

### Curriculum & Assessment Architecture

The assessment is partitioned into three progressive tiers mirroring the learning journey:

| Assessment Module | Source Tier & Curriculum | Focus Areas in Indian Lending Systems | Questions | Weightage |
|:---|:---|:---|:---:|:---:|
| **[Module 01](file:///c:/Users/user/Projects/learning-path/mcq_questionnaire/01_tier1_foundations_and_tools_mcq.md)** | **Tier 1: Foundations & Tool Setup** (Modules 1.1–1.6) | Transformer fundamentals, capabilities/risks in Indian loan calculations (INR paise rounding, KFS APR), GitHub Copilot setup (Agent/Ask/Plan modes), Claude Code CLI in loan pipelines, Google Antigravity IDE, enterprise prompt engineering for RBI credit rules. | 20 | 25% |
| **[Module 02](file:///c:/Users/user/Projects/learning-path/mcq_questionnaire/02_tier2_augmented_workflows_mcq.md)** | **Tier 2: AI-Augmented Workflows** (Modules 2.1–2.6) | Plan-Execute-Verify loops in LOS modernization, CIBIL/Experian bureau adapter debugging, AI test generation (FOIR/LTV boundaries, Account Aggregator consent flows), `AGENTS.md` context management, version control auditability, critical validation of AI output. | 20 | 40% |
| **[Module 03](file:///c:/Users/user/Projects/learning-path/mcq_questionnaire/03_tier3_advanced_agentic_governance_mcq.md)** | **Tier 3: Advanced Agentic & Governance** (Modules 3.1–3.5) | Custom lending agent skills (`SKILL.md`), multi-agent subagent orchestration across loan services (Dedupe, Bureau, Underwriting, Disbursement), OWASP Top 10 for LLMs in Indian lending, DORA metrics & ROI measurement, enterprise AI coding standards & quality gates. | 20 | 35% |
| **Total** | **Full Track A Curriculum** | **End-to-End Enterprise Agentic Mastery** | **60** | **100%** |

---

### Indian Lending (LOS & Credit Rating) Guardrails Tested

All 60 questions are contextualized within tier-1 Indian lending platforms (e.g., Digital Personal Loans, MSME Business Loans, Home Loans, Credit Scorecards, and Bureau Decision Engines). Key domain principles embedded into question scenarios include:

1. **RBI Digital Lending Guidelines (DLG) & KFS**: Direct borrower account disbursement via IMPS/NEFT/RTGS (no LSP pooling accounts), Penny-Drop bank account validation, mandatory Key Fact Statement (KFS) computation, cooling-off period enforcement.
2. **Indian Financial Precision (INR)**: Strict use of `BigDecimal` with `RoundingMode.HALF_EVEN` for INR currency, avoiding floating-point truncation on EMI calculations, broken-period interest, and GST (18%) processing fee components.
3. **Data Sovereignty & DPDP Act 2023**: Prohibition of borrower Aadhaar numbers, PAN, CKYC KIN, bank account numbers, or Credit Bureau trade-line logs escaping into overseas LLM endpoints; compliance with RBI Data Localisation directives.
4. **Bureau Integration & Decisioning Integrity**: Deterministic parsing of CIBIL/Experian TU-format segments (`NAME`, `ID`, `PT`, `TR`), handling DPD (Days Past Due) strings (`000`, `030`, `XXX`), FOIR calculation integrity, and credit limit allocations.
5. **Idempotency & Concurrency**: Strict guarantees for loan application de-duplication, sanction letter generation, and disbursement triggers under high-concurrency festival peak loads.

---

### Appraisal Grading & Scoring Matrix

| Aggregate Score | Competency Level | Annual Appraisal Rating | L&D / Engineering Management Action |
|:---:|:---|:---|:---|
| **95% – 100%** | **Distinguished SME (Tier 3+)** | **Exceeds Expectations (Top 5%)** | Eligible for AI Champion / Lending Guild Lead. Authorized to author and approve enterprise-wide India lending agent skills. |
| **85% – 94%** | **Advanced Practitioner (Tier 2/3)** | **Exceeds Expectations** | Strong autonomous agentic developer. Recommended for high-impact LOS/BRE refactoring and architecture projects. |
| **80% – 84%** | **Competent Developer (Baseline Pass)** | **Meets Expectations** | Minimum passing threshold per Track A benchmark. Cleared for daily AI tool usage on production Indian lending repositories. |
| **65% – 79%** | **Developing / Incomplete** | **Needs Improvement** | Mandatory 4-week remediation targeting failed modules. Peer review required on 100% of AI-assisted commits in lending codebases. |
| **< 65%** | **Unsatisfactory** | **Unsatisfactory** | Temporary revocation of enterprise AI tool licenses. Must retake Track A with assigned senior BFSI lending mentor. |

---

### Assessment Navigation

1. **[01_tier1_foundations_and_tools_mcq.md](file:///c:/Users/user/Projects/learning-path/mcq_questionnaire/01_tier1_foundations_and_tools_mcq.md)**: 20 Foundational & Tool Mastery Questions in Indian Lending Systems.
2. **[02_tier2_augmented_workflows_mcq.md](file:///c:/Users/user/Projects/learning-path/mcq_questionnaire/02_tier2_augmented_workflows_mcq.md)**: 20 Advanced Workflow & Code Review Questions in Loan Origination & Bureau Engineering.
3. **[03_tier3_advanced_agentic_governance_mcq.md](file:///c:/Users/user/Projects/learning-path/mcq_questionnaire/03_tier3_advanced_agentic_governance_mcq.md)**: 20 Multi-Agent, Security & Governance Questions in Indian BFSI Lending.
4. **[04_master_answer_key_and_scoring_guide.md](file:///c:/Users/user/Projects/learning-path/mcq_questionnaire/04_master_answer_key_and_scoring_guide.md)**: Complete answer key with exhaustive technical justifications, distractor autopsies, and managerial evaluation rubric.
