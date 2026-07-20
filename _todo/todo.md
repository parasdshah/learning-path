# Human Verification & Decisions — "AI Fluency at Scale"

> **Created**: 20 Jul 2026 (post link-overhaul review)
> **Purpose**: Every open item that needs a **human** — because it requires an org login, a paid-content check, a judgement call, or a business decision. Claude has already completed all the mechanical/research work it could act on (link replacement, broken-link fixes, Antigravity correction, free-%/hours/ROI reconciliation).
> **How to use**: Work top-down. P0 blocks launch. Tick the box, add your initials + date, and note the outcome.

**Legend**: 🔴 P0 = blocks launch · 🟠 P1 = needed for quality/credibility · 🔵 P2 = verification sweep · ⚪ P3 = optional

---

## 🔴 Section 1 — Must verify before launch (P0)

### 1.1 Verify all 8 Udemy courses (org login required)

The curation team has **no Udemy login**, so 0/8 are truly verified. For each: log in → open URL → confirm title, instructor, rating, enrollments, last-updated date, price, and ≥70% curriculum match → skim the 5 most recent 1–2★ reviews → record verdict in [08_udemy_verification_report.md](../_outputs/08_udemy_verification_report.md).

> ⚠️ **Slug status matters.** 3 URLs are confirmed to resolve; **5 are best-guess slugs that may 404** — if one 404s, search Udemy for the titled course and update the slug in both the track doc and report 08.

| # | Course | URL | Slug status | Verify |
|---|--------|-----|-------------|--------|
| A1 | GitHub Copilot Beginner to Pro | `/course/github-copilot/` | ✅ resolves | ☐ |
| A2 | GitHub Copilot – The Complete Guide 2026 | `/course/github-copilot-the-complete-guide/` | ✅ resolves — **but instructor "Maximilian Schwarzmüller" is unconfirmed** | ☐ |
| B1 | Using Gen AI & AI Agents in Software Automation Testing | `/course/using-gen-ai-in-software-automation-testing/` | ⚠️ **unverified guess** | ☐ |
| B2 | AI Agents, RAG & LLM Evals: DeepEval & RAGAS | `/course/ai-testing-deepeval-ragas-ollama/` | ✅ resolves (slug already corrected from a 404) | ☐ |
| B3 | GenAI & AI Agents for QA Test Automation | `/course/genai-ai-agents-qa-test-automation/` | ⚠️ **unverified guess** | ☐ |
| C1 | ChatGPT & AI Tools for Business Analysts | `/course/chatgpt-for-business-analysts/` | ⚠️ **unverified guess** | ☐ |
| D1 | LangChain & RAG: Build AI Applications | `/course/langchain-rag-ai-applications/` | ⚠️ **unverified guess** | ☐ |
| D2 | Multi-Agent AI Systems | `/course/multi-agent-ai-systems/` | ⚠️ **unverified guess** | ☐ |

- **Acceptance**: report 08 shows 8/8 with Approved / Rejected / Replace + verifier initials + date. **Owner**: L&D Team.

### 1.2 Click-test the new direct links, especially access-gated ones
- [ ] **Full link audit** — click every URL across all 4 track docs + shared KB (the maintenance plan Q1 task, run once now). **Owner**: L&D Admin.
- [ ] **HBR — "7 Factors That Drive Returns on AI Investments"** (Track C 3.2): HBR has a **metered paywall** after a few free articles/month. Confirm learners can reach it, or swap to an ungated alternative. **Owner**: Track C Champion.
- [ ] **Microsoft AI Product Manager Professional Certificate** (Track C 3.1): free only **per-course audit**; the full certificate is paid. Confirm the specific audit-free course covers feature prioritisation + stakeholder management, or point directly at that sub-course. **Owner**: Track C Champion.
- [ ] **DeepLearning.AI – ChatGPT Prompt Engineering for Devs** (Track D 2.3): page states "free **for a limited time** during platform beta." Confirm still free; if it goes paid, have a fallback ready. **Owner**: Track D Champion.

### 1.3 Provision tool access (+ Antigravity procurement note)
- [ ] Provision **GitHub Copilot** and **Claude** (Pro/Team) seats. **Owner**: IT/Procurement.
- [ ] **Antigravity is a Google / Gemini product** (corrected from the earlier "Anthropic" error). If Track A uses it, procurement/licensing runs through **Google**, not Anthropic, and it needs a Gemini-capable account. Decide whether Antigravity stays in the Tier-1 tool set or is optional. **Owner**: IT/Procurement + Track A Champion.

### 1.4 Fill in the blanks in the launch plan
- [ ] Executive summary "Action Required" table still has **[Date TBD]** and generic owners — set real dates/owners. **Owner**: L&D Programme Manager.

---

## 🟠 Section 2 — Decisions needed (P1)

### 2.1 Track B is below the 60% free-by-hours target
- **Finding**: by learning-hours, Track B is **~50% free** (3 Udemy courses = ~33 of ~66 hrs). By *module count* it's ~79% free. All other tracks clear 60% by hours.
- [ ] **Decide**: (a) consolidate the two overlapping QA-automation Udemy courses — **2.2 DeepEval/RAGAS** and **3.3 GenAI & AI Agents for QA** (heavy overlap) — into one to lift free-by-hours above 60%; **or** (b) accept it and state the metric as by-module-count programme-wide. **Owner**: Track B Champion + L&D.

### 2.2 Tier 3B — no rigorous .NET / Python case study
- **Finding**: verified public modernisation case studies cover **Java + COBOL** only.
- [ ] Source an internal **.NET** and **Python** legacy-modernisation example, or run those as a live demo instead of an external link. **Owner**: Engineering / Track A Champion.

### 2.3 Track C 2.3 (AI Feasibility) — build-vs-buy depth
- **Finding**: the Google Cloud "Organizational readiness" article is strong on data/technical readiness but light on **build-vs-buy**. The module's own decision matrix already covers it.
- [ ] Confirm the matrix + article are sufficient, or add a dedicated build-vs-buy source. **Owner**: Track C Champion.

### 2.4 Track A 1.2 — substituted video
- **Finding**: the original "Fireship, ~15 min" video couldn't be confirmed; replaced with an **IBM Technology** explainer (verified live).
- [ ] Spot-check the IBM video fits the "how AI coding assistants work + limits" intent; swap if you have a preferred one. **Owner**: Track A Champion.

### 2.5 Track B 3.1 — metrics need the pair
- **Finding**: precision/recall/F1 come from **Google ML Crash Course**; **BLEU/ROUGE** from a **Microsoft Learn** companion link. No single source covers all.
- [ ] Confirm both are assigned in the LMS as one module. **Owner**: Track B Champion.

---

## 🔵 Section 3 — Verification sweep (lower risk)

### 3.1 Confirm the remaining stable links (not re-fetched during review)
Claude verified the changed links + NIST + Google pages. These long-standing links were assumed stable — click once to confirm:
- [ ] Shared KB ethics list: ACM *Stochastic Parrots* (`dl.acm.org/doi/10.1145/3442188.3445922`), arXiv *Model Cards* (`arxiv.org/abs/1810.03993`), EU AI Act (`digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai`), AI Incident Database (`incidentdatabase.ai`).
- [ ] Untouched course links: Coursera *ML Specialization* & *AI For Everyone*, Kaggle Learn, Hugging Face Learn, MLOps Zoomcamp (GitHub), Google ML fairness/responsibility pages.
- **Owner**: L&D Admin.

### 3.2 Currency risks to monitor
- [ ] **Coursera MLOps content** (Track D 1.1 ML Spec sibling + D 3.7 *ML in Production*): a Coursera notice indicated the MLOps specialization was **closing enrollment**. Confirm the individual courses are still enrollable/auditable; if not, find replacements. **Owner**: Track D Champion.
- [ ] Add all of the above to the **Q1 quarterly link audit** ([14_maintenance_plan.md](../_outputs/14_maintenance_plan.md)) so it recurs.

---

## ⚪ Section 4 — Optional / nice-to-have (P3)

- [ ] **Clickable links in the LMS**: URLs currently sit as plain text inside the course-card code blocks. If your LMS renders Markdown, convert to `[title](url)` for one-click access. **Owner**: L&D Admin.
- [ ] **Label consistency**: Tier 3B cards use `📌 Resource:` (docs/standards) while others use `📌 Course Title:`. Standardise if desired — cosmetic only.

---

## Reference — what Claude already completed (no action needed)
- Replaced **39 search-query "links"** with verified, live direct links (mostly official docs/standards).
- Fixed **8 broken/wrong direct links** (edX, 2 dead Coursera slugs, DeepLearning.AI, MS Learn, freeCodeCamp handbook, Udemy DeepEval slug, mislabeled MLOps course).
- Corrected the **Antigravity = Google (not Anthropic)** error in Track A and the Shared KB.
- Removed the leaked local file path; dropped fabricated view counts / false "Verified" stamps on edited modules.
- Reconciled **free-%** (now stated **by learning-hours**, one method) and **hours totals** across all docs; flagged Track B honestly.
- Replaced the **ROI hype** ("1,000:1", "break-even <1 week", "15% conservative", "30%+ faster") with a measurement plan; removed the "3× faster" slogans.
- Updated **platform-distribution** tables to reflect the new docs-heavy mix.
