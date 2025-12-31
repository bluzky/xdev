# Development Workflows Guide

This guide helps you navigate the 5 core workflows. Choose based on what phase you're in.

---

## 5 Core Workflows

### 1. **Project Planning** (Once, Week 0)
**When:** Before development starts
**Duration:** 2-4 hours
**What:** Define project scope, phases, timeline, success criteria
**Output:** master-plan.md (reference document for entire project)

→ **Start here:** [workflows/01-project-planning/](./workflows/01-project-planning/README.md)

---

### 2. **Weekly Planning** (Every Monday)
**When:** Start of each week
**Duration:** 1-2 hours
**What:** Break down this week's goals into 5 daily tasks
**Output:** week-X-plan.md (scope for the week)

→ **Start here:** [workflows/02-weekly-planning/](./workflows/02-weekly-planning/README.md)

---

### 3. **Daily Planning** (Every morning, 9 AM)
**When:** Start of each day
**Duration:** 15-30 minutes
**What:** Create detailed plan with acceptance criteria
**Output:** day-Y-plan.md (execution guide for today)

→ **Start here:** [workflows/03-daily-planning/](./workflows/03-daily-planning/README.md)

---

### 4. **Daily Tracking** (Throughout day + 5 PM)
**When:** During work and at end of day
**Duration:** 5 minutes updates + 10 minutes at 5 PM
**What:** Log progress, blockers, actual time spent
**Output:** progress.md updated with day's results

→ **Start here:** [workflows/04-daily-tracking/](./workflows/04-daily-tracking/README.md)

---

### 5. **Weekly Retrospective** (Friday, 4:30 PM)
**When:** End of each week
**Duration:** 1 hour
**What:** Review week results, capture learnings, adjust next week's plan
**Output:** summary.md (week analysis) + updated master-progress.md

→ **Start here:** [workflows/05-weekly-retrospective/](./workflows/05-weekly-retrospective/README.md)

---

## Quick Reference

| Workflow | When | Files | AI Role |
|----------|------|-------|---------|
| Project Planning | Week 0 | master-plan.md | Analyze requirements, suggest structure |
| Weekly Planning | Monday 9 AM | week-X-plan.md | Suggest daily breakdown, estimate time |
| Daily Planning | Every 9 AM | day-Y-plan.md | Review plan, suggest approach |
| Daily Tracking | During day + 5 PM | progress.md | Populate execution data |
| Weekly Retrospective | Friday 4:30 PM | summary.md, master-progress.md | Analyze metrics, identify patterns |

---

## Typical Weekly Cycle

```
Monday 9:00 AM
  └─ WEEKLY PLANNING → create week-X-plan.md
  └─ DAILY PLANNING → create day-1-plan.md
  └─ Development starts

Monday-Friday (Each Day)
  └─ 9:00 AM: DAILY PLANNING → create day-Y-plan.md
  └─ Throughout: DAILY TRACKING → log progress
  └─ 4:30 PM: PM reviews day-Y-plan.md execution + signs off
  └─ 5:00 PM: DAILY TRACKING → finalize day's results

Friday 4:30 PM
  └─ WEEKLY RETROSPECTIVE → create summary.md
  └─ Update master-progress.md
  └─ Adjust next week's plan
```

---

## For AI/Automation

Each workflow folder contains:
- **README.md** — Step-by-step instructions (AI can follow these)
- **template.md** — Simplified template with clear sections
- **checklist.md** — Quick reference for what to do

AI works best when:
1. You give it the README first (tells AI what workflow to follow)
2. You provide context (previous week's data, current state)
3. AI generates the document (draft or complete)
4. Human reviews and approves before committing

---

## Choosing Your Workflow

**I'm starting a brand new project**
→ Go to [Workflow 1: Project Planning](./workflows/01-project-planning/)

**It's Monday and I need to plan this week**
→ Go to [Workflow 2: Weekly Planning](./workflows/02-weekly-planning/)

**It's morning and I'm starting my day**
→ Go to [Workflow 3: Daily Planning](./workflows/03-daily-planning/)

**I'm in the middle of work and need to log progress**
→ Go to [Workflow 4: Daily Tracking](./workflows/04-daily-tracking/)

**It's Friday and I need to wrap up the week**
→ Go to [Workflow 5: Weekly Retrospective](./workflows/05-weekly-retrospective/)

---

## Key Principle

Each workflow is independent but connected:
- **Planning workflows** define what should happen (rarely change)
- **Tracking workflows** record what actually happened (update daily)
- **Retrospective workflow** connects them (learnings inform next plan)

**Simple rule:** Do the planning once, update tracking daily, retrospect weekly.
