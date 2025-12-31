# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a **development methodology template package** for weekly sprint-based software development with daily PM verification.

**Start here:** [WORKFLOWS.md](./WORKFLOWS.md) - Choose your workflow

---

## 5 Core Workflows

The methodology is organized into 5 independent workflows. Each has:
- A clear purpose (when to use it)
- Step-by-step README instructions
- Simplified templates
- Clear entry point for AI

| # | Workflow | When | Files | Time |
|---|----------|------|-------|------|
| 1 | **Project Planning** | Week 0 | master-plan.md | 2-4 hours |
| 2 | **Weekly Planning** | Monday 9 AM | week-X-plan.md | 1-2 hours |
| 3 | **Daily Planning** | Every 9 AM | day-Y-plan.md | 15-30 min |
| 4 | **Daily Tracking** | Throughout day + 5 PM | progress.md | 15 min |
| 5 | **Weekly Retrospective** | Friday 4:30 PM | summary.md | 1 hour |

**→ Navigate to:** [workflows/](./workflows/)

---

## Quick Links by Task

**I'm starting a new project**
→ [Workflow 1: Project Planning](./workflows/01-project-planning/README.md)

**It's Monday and I need to plan the week**
→ [Workflow 2: Weekly Planning](./workflows/02-weekly-planning/README.md)

**It's morning and I'm starting my day**
→ [Workflow 3: Daily Planning](./workflows/03-daily-planning/README.md)

**I'm working and need to track progress**
→ [Workflow 4: Daily Tracking](./workflows/04-daily-tracking/README.md)

**It's Friday and I need to do retrospective**
→ [Workflow 5: Weekly Retrospective](./workflows/05-weekly-retrospective/README.md)

---

## Document Structure

```
docs/plan/
├── master-plan.md              (Project roadmap - created once)
├── master-progress.md          (Project status - updated weekly)
│
├── week-1-plan.md              (Weekly scope)
├── week-1/
│   ├── progress.md             (Daily tracking log)
│   ├── summary.md              (Weekly retrospective)
│   ├── day-1-plan.md           (Daily detailed plan)
│   ├── day-2-plan.md
│   └── ...
├── week-2-plan.md
├── week-2/
│   └── ... (same structure)
└── ...
```

---

## Core Principles

1. **Plan Once, Track Daily**
   - Planning docs (master, weekly, daily) rarely change
   - Tracking docs (progress, execution) updated daily
   - Don't duplicate - reference instead

2. **Daily Verification**
   - PM reviews each day's work (not weekly)
   - Issues caught immediately
   - Definition of done is testable

3. **Feedback Loop**
   - Retrospectives capture learnings
   - Next week's plan incorporates insights
   - Continuous improvement

---

## For AI/Automation

Each workflow folder contains:
1. **README.md** — Step-by-step instructions (very clear for AI)
2. **template.md** — Simplified template with sections to fill
3. **Optional:** Examples or checklists

**How AI works best:**
1. Human provides context (previous week, current state)
2. AI reads workflow README to understand task
3. AI generates document from template
4. Human reviews and approves

---

## Key Development Phases

Projects typically follow 4 phases:
1. **Preparation** (Week 1) — Requirements, architecture, planning
2. **Build Core** (Week 2-3) — Main features implementation
3. **Integration & MVP** (Week 4-5) — Connect, test, release
4. **Polish** (Week 6+) — Refinement, edge cases, deployment

---

## Important Notes

1. **Templates are starting points** — Customize for your project needs
2. **Time estimates** — Daily breaks should total 30-40 hours/week
3. **Priorities** — Use P0 (must), P1 (should), P2 (nice) always
4. **Success criteria** — Must be specific and testable
5. **PM sign-off** — Daily verification is critical, don't skip
6. **Metrics** — Track velocity and quality indicators

---

## Success Indicators

You're using this well when:
- ✅ Each day produces testable work
- ✅ PM verifies daily (not weekly)
- ✅ Blockers caught same day
- ✅ Velocity improves week-to-week
- ✅ Retrospectives improve process
- ✅ Complete documentation trail exists

---

## Navigation

- [WORKFLOWS.md](./WORKFLOWS.md) — Workflow overview and quick reference
- [workflows/01-project-planning/](./workflows/01-project-planning/) — Project setup
- [workflows/02-weekly-planning/](./workflows/02-weekly-planning/) — Weekly scope
- [workflows/03-daily-planning/](./workflows/03-daily-planning/) — Daily plan
- [workflows/04-daily-tracking/](./workflows/04-daily-tracking/) — Progress tracking
- [workflows/05-weekly-retrospective/](./workflows/05-weekly-retrospective/) — Week review
