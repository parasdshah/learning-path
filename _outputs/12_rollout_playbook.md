# Rollout Playbook

> **Purpose**: Operational guidance for launching, managing, and sustaining the AI upskilling programme.

---

## 1. Cohort Sizing

### Recommended Cohort Structure

| Track | Cohort Size | Rationale |
|-------|------------|-----------|
| **Track A (Dev)** | 15–25 | Developers need peer review partners; too large = diluted interaction |
| **Track B (QA)** | 10–20 | Smaller QA teams; niche content benefits from closer peer interaction |
| **Track C (BA)** | 15–25 | BAs benefit from discussion-heavy learning; manageable for peer review |
| **Track D (AI Dev)** | 10–15 | Deep technical content; smaller groups for meaningful code review |

### Cohort Formation Rules
- **Launch cohorts monthly** — don't wait for a "big bang" launch
- **Mix experience levels** within a cohort (junior + mid + senior) for peer learning
- **Keep team members together** where possible (same team → same cohort → shared context)
- **Allow cross-cohort interaction** via shared Slack/Teams channels
- **Assign a cohort lead** (a senior who's 1–2 tiers ahead) for lightweight facilitation

---

## 2. Manager Enablement

### One-Pager for Managers: "Supporting Your Team's AI Learning"

```
═══════════════════════════════════════════════════════════
📋 MANAGER'S GUIDE TO AI UPSKILLING SUPPORT
═══════════════════════════════════════════════════════════

WHY THIS MATTERS
• AI-skilled teams deliver 30%+ faster. This training makes 
  your team more productive, not less.
• This is a strategic investment with measurable ROI.

YOUR ROLE (3 things)
1. PROTECT LEARNING TIME
   → Block 4–6 hrs/week for your team (Friday afternoons recommended)
   → Do NOT schedule meetings during learning blocks
   → Treat learning time as sacrosanct as sprint commitments

2. ENABLE APPLICATION
   → Ask in 1:1s: "What AI technique did you try this week?"
   → Allow controlled experimentation with AI tools on real work
   → Celebrate learning milestones (badge completions, projects)

3. PARTICIPATE
   → Complete Tier 1 yourself (all managers, regardless of role)
   → Attend monthly showcase presentations
   → Review and sponsor capstone projects

WHAT NOT TO DO
✗ Don't cancel learning time for "urgent" work
✗ Don't measure learning by hours logged — measure by skills applied
✗ Don't compare individuals' progress — learning is self-paced
✗ Don't treat AI tools as optional — this is a required capability

SUCCESS INDICATOR
When your team naturally reaches for AI tools first, and code 
reviews include "Did you try this with Copilot/Claude Code?", 
the programme is working.
═══════════════════════════════════════════════════════════
```

---

## 3. Gamification System

### Badge & Points Framework

#### Points System

| Action | Points | Frequency |
|--------|--------|-----------|
| Complete a module | 10 pts | Per module |
| Pass Tier checkpoint (quiz ≥80%) | 50 pts | Per tier |
| Submit mini-project (Tier 2) | 100 pts | Once |
| Complete peer review (as reviewer) | 25 pts | Per review |
| Share a tip/resource in Slack | 5 pts | Daily max |
| Present at monthly showcase | 50 pts | Per presentation |
| Submit Tier 3 capstone | 200 pts | Once |
| Complete Tier 3B case study | 150 pts | Once |
| Help a colleague with AI tool issue | 10 pts | Unlimited |
| Write a blog post / internal wiki about AI experience | 50 pts | Unlimited |

#### Achievement Levels

| Level | Points Required | Title | Perk |
|-------|----------------|-------|------|
| 1 | 0–99 | AI Explorer | — |
| 2 | 100–249 | AI Apprentice | Name on programme leaderboard |
| 3 | 250–499 | AI Practitioner | AI-themed sticker pack / swag |
| 4 | 500–749 | AI Specialist | Feature in company newsletter |
| 5 | 750–999 | AI Champion | Invite to AI leadership council |
| 6 | 1000+ | AI Master | Conference attendance sponsorship |

#### Leaderboard
- **Track-specific leaderboards** (don't compare QA against AI Devs)
- **Team leaderboards** (encourages whole-team participation)
- **Weekly movers** highlight (who gained the most points this week)
- **Reset quarterly** to keep engagement fresh

---

## 4. Communication Channels

### Slack / Teams Channel Structure

| Channel | Purpose | Audience |
|---------|---------|----------|
| `#ai-learning-general` | Cross-track announcements, shared resources, AI news | Everyone |
| `#ai-track-developers` | Track A discussions, help, resource sharing | Developers |
| `#ai-track-qa` | Track B discussions, help, resource sharing | QA Engineers |
| `#ai-track-business` | Track C discussions, help, resource sharing | Business Analysts |
| `#ai-track-aidev` | Track D discussions, help, resource sharing | AI/ML Developers |
| `#ai-tools-help` | Technical help with AI tools (Copilot, Claude Code, etc.) | Everyone |
| `#ai-wins` | Share successes — "I used AI to do X and saved Y hours" | Everyone |
| `#ai-fails` | Share failures (blameless) — "AI hallucinated this..." | Everyone |
| `#ai-capstone-teams` | Capstone project coordination | Tier 3 learners |

### Channel Norms
- **Weekly prompt**: Monday morning automated post — "What AI tool/technique are you trying this week?"
- **Thursday tip**: Thursday afternoon — "Tip of the Week" from a learner or L&D team
- **No judgement in #ai-fails**: This channel is for learning from mistakes. Celebrate honesty.
- **Pin important resources**: Keep tool setup guides, glossary, and FAQ pinned

---

## 5. Monthly Showcases

### Format: "AI Show & Tell" (60 minutes)

```
Time   | Segment                           | Duration
-------|-----------------------------------|--------
0–5    | Welcome & housekeeping            | 5 min
5–15   | Showcase 1 (learner presentation) | 10 min
15–25  | Showcase 2 (learner presentation) | 10 min
25–35  | Showcase 3 (learner presentation) | 10 min
35–45  | Panel Q&A with presenters         | 10 min
45–55  | "Tool of the Month" demo          | 10 min
55–60  | Next month preview + awards       | 5 min
```

### Showcase Presentation Template
- **What I learned**: 1 slide on the concept/tool
- **What I built/tried**: Live demo or screenshots
- **What surprised me**: Honest reflection on AI strengths/weaknesses
- **What I'll do differently**: Action items for my daily work
- **Total time**: 8 minutes presentation + 2 minutes Q&A

### Schedule
- **First Thursday of every month**, 3:00–4:00 PM
- **Rotate tracks**: Month 1 = Dev, Month 2 = QA, Month 3 = BA, Month 4 = AI Dev, Month 5 = mixed
- **Record all sessions** for those who can't attend live (aligns with self-paced philosophy)

---

## 6. Feedback Loops

### Feedback Collection Points

| Timing | Method | Questions |
|--------|--------|-----------|
| **After each tier** | 5-question survey (LMS) | NPS, content quality, difficulty, time estimate accuracy, suggestions |
| **After each Udemy course** | Quick survey (3 questions) | Was it current? Was it useful? Would you recommend it? |
| **Monthly** | Pulse check (2 questions in Slack) | "Are you on track?" + "What's blocking you?" |
| **Quarterly** | Deep dive survey (15 questions) | Skill confidence, tool usage frequency, ROI perception, content gaps |
| **Post-capstone** | Structured reflection (team) | What worked, what didn't, team dynamics, recommendations |

### Feedback Action Cycle

```
Collect (surveys/Slack)
    ↓
Analyse (L&D team — biweekly)
    ↓
Prioritise (top 3 issues per quarter)
    ↓
Act (update content, adjust pacing, fix issues)
    ↓
Communicate ("You said X, we did Y")
    ↓
Repeat
```

### Key Feedback Metrics to Track
- **NPS per module**: Target ≥8/10. Anything below 7 → investigate and fix
- **Completion funnel**: Where do people drop off? (Tier 1→2 transition is critical)
- **Time estimate accuracy**: Are modules taking longer than estimated? Adjust
- **Content freshness complaints**: Any "this is outdated" feedback → immediate course replacement
- **Tool adoption**: "Are you using AI tools in daily work?" → the ultimate success metric

---

## 7. Launch Timeline

### Recommended 12-Week Launch Plan

| Week | Activity |
|------|----------|
| **Week -4** | Finalise programme materials. Verify all Udemy courses. Set up LMS. |
| **Week -3** | Configure Slack/Teams channels. Set up badge system. Create quiz banks. |
| **Week -2** | Manager enablement session (1 hour). Send programme announcement. Open registration. |
| **Week -1** | Tool access provisioning (GitHub Copilot, Claude, etc.). Welcome email with setup guide. |
| **Week 1** | 🚀 Launch! All tracks begin Tier 1 simultaneously. First cohorts start. |
| **Week 2** | Check-in: Pulse survey. Address any setup issues. |
| **Week 3** | Tier 1 checkpoint opens. First completions expected. |
| **Week 4** | Tier 2 begins for fast movers. Launch #ai-wins channel. |
| **Week 5** | First monthly showcase (Tier 1 reflections from early completers). |
| **Week 8** | Tier 2 checkpoints. Mini-project submissions begin. |
| **Week 9** | Tier 3 begins. Capstone team formation starts. |
| **Week 12** | First quarterly review. Feedback analysis. Content refresh if needed. |
