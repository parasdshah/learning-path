# Success Metrics Dashboard Template

> **Purpose**: Define measurable KPIs, targets, and measurement methods for the AI upskilling programme.

---

## Primary KPIs

| # | KPI | Target | Measurement Method | Frequency | Owner |
|---|-----|--------|--------------------|-----------|-------|
| 1 | **Enrollment Rate** | >80% of eligible staff | LMS registration data / total eligible headcount | Monthly | L&D Team |
| 2 | **Tier 1 Completion Rate** | >90% within 4 weeks of enrollment | LMS — quiz pass + reflection submitted | Weekly | L&D Team |
| 3 | **Tier 2 Completion Rate** | >70% within 8 weeks of enrollment | LMS — mini-project submitted + peer review completed | Weekly | L&D Team |
| 4 | **Tier 3 Completion Rate** | >50% within 12 weeks of enrollment | LMS — capstone submitted + presentation delivered | Monthly | L&D Team |
| 5 | **Tier 3B Completion (Track A)** | >40% of Track A advanced learners | LMS — case study submitted + senior engineer review passed | Monthly | L&D Team |
| 6 | **Brownfield Project Time Saved** | >30% reduction in legacy task time | Pre/post survey comparing time estimates for similar tasks | Quarterly | Engineering Managers |
| 7 | **Learner Satisfaction (NPS)** | >8/10 | Post-module survey (1–10 scale) | Per tier | L&D Team |
| 8 | **On-the-Job Application** | >60% report using AI skills weekly | Quarterly survey: "How often do you use AI tools in your work?" | Quarterly | L&D Team |
| 9 | **Cross-functional Capstone Completion** | >40% of advanced learners participate | Capstone project submissions / total Tier 3 eligible learners | Quarterly | L&D Team |
| 10 | **Udemy Course Verification Rate** | 100% of recommended Udemy courses | Udemy verification report — verified count / total count | Pre-launch + Quarterly | L&D Team |

---

## Secondary KPIs

| # | KPI | Target | Measurement Method | Frequency |
|---|-----|--------|--------------------|-----------|
| 11 | **Module Completion Rate** | >85% per module | LMS — module marked complete | Weekly |
| 12 | **Average Quiz Score (Tier 1)** | >85% | LMS — quiz analytics | Weekly |
| 13 | **Peer Review Participation** | >90% of Tier 2+ learners complete at least 1 peer review | LMS — peer review submissions | Monthly |
| 14 | **Slack/Teams Channel Activity** | >50% of enrolled learners post at least once/month | Channel analytics | Monthly |
| 15 | **Monthly Showcase Attendance** | >30% of enrolled learners attend (live or recording) | Attendance tracking + view counts | Monthly |
| 16 | **Content Freshness** | 0 courses with "outdated" feedback | Learner survey analysis | Quarterly |
| 17 | **Manager Enablement Completion** | >90% of managers complete Tier 1 | LMS — manager cohort tracking | One-time |
| 18 | **Badge Issuance Rate** | In line with completion rates | Badge platform analytics | Monthly |
| 19 | **Time-to-Completion (median)** | Within ±20% of estimated duration per tier | LMS — enrollment date to completion date | Monthly |
| 20 | **Drop-off Rate per Tier** | <30% between Tier 1→2; <40% between Tier 2→3 | LMS — completion funnel analysis | Monthly |

---

## Tracking Dashboard Layout

### Dashboard Section 1: Enrollment & Progress

```
┌─────────────────────────────────────────────────────────────┐
│  ENROLLMENT OVERVIEW                      [Filter: Track ▼] │
│                                                             │
│  Total Enrolled: ███ / ███ (XX%)          Target: >80%      │
│                                                             │
│  Track A: ██████████ XX%    Track B: ████████ XX%           │
│  Track C: █████████ XX%     Track D: ███████ XX%            │
│                                                             │
│  ──────────────────────────────────────────────────          │
│  COMPLETION FUNNEL                                          │
│                                                             │
│  Tier 1  ▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓  XX% (target: >90%)        │
│  Tier 2  ▓▓▓▓▓▓▓▓▓▓▓▓▓▓        XX% (target: >70%)        │
│  Tier 3  ▓▓▓▓▓▓▓▓▓▓            XX% (target: >50%)        │
│  Tier 3B ▓▓▓▓▓▓▓               XX% (target: >40%)        │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

### Dashboard Section 2: Satisfaction & Quality

```
┌─────────────────────────────────────────────────────────────┐
│  LEARNER SATISFACTION                                       │
│                                                             │
│  Overall NPS:  ★★★★★★★★☆☆  8.2 / 10  (target: >8.0)      │
│                                                             │
│  By Track:                                                  │
│  Track A: 8.4  Track B: 7.9  Track C: 8.5  Track D: 8.0   │
│                                                             │
│  By Tier:                                                   │
│  Tier 1: 8.6   Tier 2: 7.8   Tier 3: 8.1                  │
│                                                             │
│  ──────────────────────────────────────────────────          │
│  CONTENT QUALITY FLAGS                                      │
│  🟢 No "outdated" complaints    🟡 2 courses flagged        │
│  🔴 1 course needs replacement                              │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

### Dashboard Section 3: On-the-Job Impact

```
┌─────────────────────────────────────────────────────────────┐
│  ON-THE-JOB APPLICATION                                     │
│                                                             │
│  "I use AI tools weekly":  XX% (target: >60%)               │
│                                                             │
│  Brownfield Time Saved:  XX% (target: >30%)                 │
│                                                             │
│  Top AI tools in daily use:                                 │
│  1. GitHub Copilot  (XX% of devs)                           │
│  2. Claude Code     (XX% of devs)                           │
│  3. ChatGPT         (XX% of all roles)                      │
│                                                             │
│  Capstone Projects Completed: XX / XX (XX%)                 │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

---

## Data Collection Schedule

| Data Source | Collection Method | Frequency | Responsible |
|------------|------------------|-----------|-------------|
| LMS Enrollment Data | Automated LMS export | Weekly | L&D Admin |
| Quiz Scores | Automated LMS analytics | Real-time | L&D Admin |
| Project Submissions | Manual LMS check | Weekly | L&D Team |
| Peer Reviews | Manual LMS check | Weekly | L&D Team |
| Post-Tier Surveys | Automated survey trigger | Per tier completion | L&D Team |
| Quarterly Deep Dive Survey | Manual survey distribution | Quarterly | L&D Team |
| Slack/Teams Analytics | Channel analytics export | Monthly | L&D Admin |
| Showcase Attendance | Manual + recording views | Monthly | L&D Admin |
| On-the-Job Application Survey | Quarterly survey | Quarterly | Engineering Managers |
| Brownfield Time-Saved Data | Pre/post project surveys | Per Tier 3B completion | Engineering Managers |
| Udemy Verification Audit | Manual login + verification | Quarterly | L&D Team |
| Badge Issuance | Badge platform analytics | Monthly | L&D Admin |

---

## Reporting Cadence

| Report | Audience | Frequency | Content |
|--------|----------|-----------|---------|
| **Weekly Pulse** | L&D Team | Weekly | Enrollments, completions, flags |
| **Monthly Dashboard** | L&D + Managers | Monthly | Full KPI dashboard, showcase report |
| **Quarterly Review** | Leadership | Quarterly | Strategic KPIs, ROI analysis, content health, recommendations |
| **Annual Report** | C-suite | Annually | Programme ROI, organisational AI maturity assessment, strategic recommendations |

---

## Alert Thresholds

| Condition | Severity | Action |
|-----------|----------|--------|
| Enrollment rate < 50% after 2 weeks | 🔴 Critical | Investigate barriers; re-communicate; involve managers |
| Tier 1 completion < 70% after 6 weeks | 🟡 Warning | Survey non-completers; check content difficulty |
| NPS < 7.0 for any module | 🔴 Critical | Immediate review; replace or restructure content |
| Any course receives "outdated" feedback from 3+ learners | 🟡 Warning | Verify course; replace if confirmed outdated |
| Drop-off > 50% between Tier 1→2 | 🟡 Warning | Investigate causes; add transitional support |
| Udemy course removed/unavailable | 🔴 Critical | Immediate replacement from fallback list |
| < 30% using AI tools weekly after Tier 2 | 🟡 Warning | Add "applied learning" workshops; involve managers |
