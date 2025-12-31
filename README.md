# Development Methodology Repository

Complete, production-ready system for organizing software development with AI.

**Two versions: Team-based and Solo Developer.**

---

## Start Here

### I'm a solo developer (+ AI partner)
→ [SOLO_DEV_START.md](./SOLO_DEV_START.md)

Key benefits:
- 4 simple workflows (Project → Weekly → Daily → Review)
- AI generates daily plans in 2 minutes
- 30-minute Friday reflection
- ~2 hours/week overhead
- Perfect for solo dev + AI collaboration

---

### I'm leading a team
→ [WORKFLOWS.md](./WORKFLOWS.md)

Key benefits:
- 5 comprehensive workflows with PM oversight
- Daily team verification and sign-offs
- Complete documentation and metrics
- Team retrospectives and feedback loops
- Scales for 3+ person teams

---

### I'm deciding between versions
→ [VERSION_GUIDE.md](./VERSION_GUIDE.md)

Detailed comparison of both approaches.

---

## What's Included

### Solo Version (~56K)
- 4 workflows (simplified)
- 12 files (4 workflows × 3 files each)
- Focused on solo dev + AI partnership
- Minimal overhead (~2 hours/week)

### Team Version (~108K)
- 5 workflows (comprehensive)
- 15 files (5 workflows × 3 files each)
- PM oversight and team coordination
- Complete documentation (~3-4 hours/week)

### Both versions include:
- README.md (step-by-step instructions for humans)
- template.md (simplified form to fill)
- ai-prompt.md (structured instructions for AI)

### Supporting Files
- CLAUDE.md — Entry point for AI
- INDEX.md — File index
- QUICK_REFERENCE.md — Team quick ref (print it)
- SOLO_QUICK_REF.md — Solo quick ref (print it)
- AI_WORKFLOW_GUIDE.md — How to use AI with team version

---

## Quick Start (2 Minutes)

**Solo Dev:**
1. Read [SOLO_DEV_START.md](./SOLO_DEV_START.md)
2. Choose your workflow
3. Follow the README in that workflow

**Team:**
1. Read [WORKFLOWS.md](./WORKFLOWS.md)
2. Choose your workflow
3. Follow the README in that workflow

Both are designed to be fast and friction-free.

---

## Core Workflows

### SOLO VERSION (4 Workflows)

| # | Workflow | When | Duration | Output |
|---|----------|------|----------|--------|
| 1 | Project Setup | Once | 30 min | project-plan.md |
| 2 | Weekly Plan | Monday | 30 min | week-X-plan.md |
| 3 | Daily Plan | Every 9 AM | 10 min | day-Y-plan.md |
| 4 | Weekly Review | Friday 5 PM | 30 min | summary.md |

**Total overhead:** ~2 hours/week

---

### TEAM VERSION (5 Workflows)

| # | Workflow | When | Duration | Output |
|---|----------|------|----------|--------|
| 1 | Project Planning | Week 0 | 2-4 hrs | master-plan.md |
| 2 | Weekly Planning | Monday | 1-2 hrs | week-X-plan.md |
| 3 | Daily Planning | Every 9 AM | 15-30 min | day-Y-plan.md |
| 4 | Daily Tracking | Throughout day | 15 min | progress.md updates |
| 5 | Weekly Retrospective | Friday 4:30 PM | 1 hour | summary.md |

**Total overhead:** ~3-4 hours/week

---

## Files & Organization

```
xdev/
├── SOLO_DEV_START.md          ← Start here (solo)
├── SOLO_QUICK_REF.md          ← Print this (solo)
├── WORKFLOWS.md               ← Start here (team)
├── QUICK_REFERENCE.md         ← Print this (team)
├── VERSION_GUIDE.md           ← Choose your version
├── AI_WORKFLOW_GUIDE.md       ← AI instructions (team)
├── CLAUDE.md                  ← AI entry point
├── INDEX.md                   ← Complete file index
├── README.md                  ← This file
│
├── solo/                      ← SOLO version
│   ├── 01-project-setup/      (README, template, ai-prompt)
│   ├── 02-weekly-plan/        (README, template, ai-prompt)
│   ├── 03-daily-plan/         (README, template, ai-prompt)
│   └── 04-weekly-review/      (README, template, ai-prompt)
│
├── workflows/                 ← TEAM version
│   ├── 01-project-planning/   (README, template, ai-prompt)
│   ├── 02-weekly-planning/    (README, template, ai-prompt)
│   ├── 03-daily-planning/     (README, template, ai-prompt)
│   ├── 04-daily-tracking/     (README, template, ai-prompt)
│   └── 05-weekly-retrospective/ (README, template, ai-prompt)
│
└── old-files/                 ← Original documentation (archived)
    ├── README.md
    ├── 00-START-HERE.md
    ├── METHODOLOGY_GUIDE.md
    ├── README_TEMPLATES.md
    ├── guides/
    └── templates/
```

---

## Key Features

### Both Versions
✅ **AI-Ready Prompts** — Each workflow has detailed AI instructions
✅ **Simplified Templates** — Not bloated, exactly what you need
✅ **Clear Entry Points** — No confusion about where to start
✅ **Quality-First** — Tests pass, build clean standards
✅ **Feedback Loops** — Weekly reviews inform planning
✅ **Metric Tracking** — Velocity data drives improvements

### Solo Version Specific
✅ **Minimal Overhead** — ~2 hours/week
✅ **AI Partnership** — Not just tool, but collaborator
✅ **Quick Plans** — 10-minute daily planning
✅ **Self-Verification** — You own quality gates
✅ **No Meetings** — Solo reflection only

### Team Version Specific
✅ **PM Oversight** — Daily sign-offs
✅ **Team Coordination** — Alignment meetings
✅ **Complete Docs** — Full transparency
✅ **Scalable** — Works for 3+ developers
✅ **Comprehensive** — Nothing falls through cracks

---

## Methodology Principles

**Universal (Both Versions):**
1. **Plan Once, Track Daily** — Plans stable, tracking frequent
2. **Daily Verification** — Issues caught immediately, not Friday
3. **Clear Done Criteria** — Testable, not vague
4. **Feedback Loop** — Retrospectives drive improvements
5. **Metric Driven** — Data informs decisions

---

## How AI Fits In

### SOLO Version
AI is your partner throughout:
- **Morning (9 AM):** AI generates your day plan (2 min)
- **During day:** AI helps with code, architecture, debugging
- **Friday:** AI helps draft your weekly summary

### TEAM Version
AI as a support tool:
- **Planning:** AI helps break down scope, suggest tasks
- **Execution:** AI helps with code, problem-solving
- **Documentation:** AI helps draft summaries and retrospectives

---

## Getting Started

### Option 1: Solo Dev Path
```
1. Read: SOLO_DEV_START.md (5 min)
2. Create: project-plan.md (30 min)
3. Monday: week-1-plan.md (30 min)
4. Every day: Ask AI to generate day-Y-plan.md (2 min)
5. Start building!
```

### Option 2: Team Path
```
1. Read: WORKFLOWS.md (3 min)
2. Create: master-plan.md (2-4 hours)
3. Brief team: Methodology overview (30 min)
4. Monday: week-1-plan.md (1-2 hours)
5. Monday 10 AM: Team alignment meeting
6. Start building!
```

---

## Documentation Quality

- **Templates:** Simplified, focused, no bloat
- **Instructions:** Clear step-by-step, no jargon
- **AI Prompts:** Detailed, with examples and quality checks
- **Quick Refs:** Printable, keep visible
- **Total:** ~280K of structured documentation

---

## Success Indicators

You're using this well when:

✅ Each day produces independently testable work
✅ Issues caught daily, not Friday
✅ Velocity is predictable
✅ Estimates improve over time
✅ Team/personal velocity increases week-to-week
✅ Quality metrics improve (fewer errors)
✅ Retrospectives identify concrete improvements
✅ Documentation is complete for future reference

---

## Support

**Questions about the methodology?**
- Humans: Read the README.md in your chosen workflow
- AI: Read the ai-prompt.md in your chosen workflow

**Need examples?**
- Each ai-prompt.md includes detailed examples

**Want to customize?**
- Templates are starting points—adapt as needed
- Keep core principles (daily verification, feedback loop)

---

## Versions & History

**Latest:** v1.0 (Complete, both versions)
- Solo dev version (4 workflows, ~56K)
- Team version (5 workflows, ~108K)
- Original docs archived (old-files/)

---

## Choose Your Path

| Your Situation | Choose | Start Here |
|---|---|---|
| Solo dev + AI partner | SOLO | [SOLO_DEV_START.md](./SOLO_DEV_START.md) |
| Team of 3+ developers | TEAM | [WORKFLOWS.md](./WORKFLOWS.md) |
| Not sure | Compare | [VERSION_GUIDE.md](./VERSION_GUIDE.md) |
| Need quick ref | Both | [SOLO_QUICK_REF.md](./SOLO_QUICK_REF.md) or [QUICK_REFERENCE.md](./QUICK_REFERENCE.md) |

---

**Ready to start? Pick your version. Follow the instructions. Build great things.**

🚀
