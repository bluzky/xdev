# Index: Development Methodology Documentation

**Last Updated:** Dec 31, 2025
**Status:** Ready for use with AI and humans

---

## Start Here

Choose based on your situation:

### I'm using this methodology for the first time
1. Read: [WORKFLOWS.md](./WORKFLOWS.md) (5 min)
2. Print: [QUICK_REFERENCE.md](./QUICK_REFERENCE.md)
3. Choose your workflow from the 5 below

### I'm an AI helping with this project
1. Read: [AI_WORKFLOW_GUIDE.md](./AI_WORKFLOW_GUIDE.md) (understanding)
2. Get the human to tell you which workflow
3. Read the corresponding `ai-prompt.md` file
4. Generate the document

### I'm continuing an ongoing project
1. Check: What phase are we in?
2. What day is it? (Monday → Workflow 2, etc.)
3. Jump to that workflow

---

## Core Documentation

### Entry Points

| File | Purpose | Read Time |
|------|---------|-----------|
| **CLAUDE.md** | For AI: Entry point and quick links | 2 min |
| **WORKFLOWS.md** | Overview of 5 workflows | 3 min |
| **QUICK_REFERENCE.md** | Cheat sheet (print this!) | Reference |
| **AI_WORKFLOW_GUIDE.md** | How to use AI with workflows | 5 min |

### For Humans

- **[WORKFLOWS.md](./WORKFLOWS.md)** — Understand the 5 workflows
- **[QUICK_REFERENCE.md](./QUICK_REFERENCE.md)** — Keep visible while working
- Each workflow's **README.md** — Step-by-step instructions

### For AI

- **[AI_WORKFLOW_GUIDE.md](./AI_WORKFLOW_GUIDE.md)** — Understand how to work with AI
- Each workflow's **ai-prompt.md** — Detailed instructions for AI
- Each workflow's **template.md** — Expected output format

---

## The 5 Workflows

### Workflow 1: Project Planning
**When:** Week 0, project setup
**Duration:** 2-4 hours
**Output:** `master-plan.md`

**Files:**
- [README.md](./workflows/01-project-planning/README.md) — 5 steps
- [template.md](./workflows/01-project-planning/template.md) — Form to fill
- [ai-prompt.md](./workflows/01-project-planning/ai-prompt.md) — AI instructions (4.8K)

**Quick:** Define project scope, phases, timeline, success criteria

---

### Workflow 2: Weekly Planning
**When:** Every Monday 9 AM
**Duration:** 1-2 hours
**Output:** `week-X-plan.md`

**Files:**
- [README.md](./workflows/02-weekly-planning/README.md) — 4 steps
- [template.md](./workflows/02-weekly-planning/template.md) — Form to fill
- [ai-prompt.md](./workflows/02-weekly-planning/ai-prompt.md) — AI instructions (8.0K)

**Quick:** Break week into 5 days with realistic daily objectives

---

### Workflow 3: Daily Planning
**When:** Every morning 9 AM
**Duration:** 15-30 minutes
**Output:** `day-Y-plan.md`

**Files:**
- [README.md](./workflows/03-daily-planning/README.md) — 4 steps
- [template.md](./workflows/03-daily-planning/template.md) — Form to fill
- [ai-prompt.md](./workflows/03-daily-planning/ai-prompt.md) — AI instructions (12K)

**Quick:** Create 3-4 specific tasks with testable acceptance criteria

---

### Workflow 4: Daily Tracking
**When:** Throughout day + 5 PM
**Duration:** 5 min updates + 10 min summary
**Output:** `progress.md` + day plan execution section

**Files:**
- [README.md](./workflows/04-daily-tracking/README.md) — Clear logging instructions
- [template.md](./workflows/04-daily-tracking/template.md) — Form to fill
- [ai-prompt.md](./workflows/04-daily-tracking/ai-prompt.md) — AI instructions (10K)

**Quick:** Log progress, update execution notes, verify quality

---

### Workflow 5: Weekly Retrospective
**When:** Friday 4:30 PM
**Duration:** 1 hour (20 min discussion + 40 min writing)
**Output:** `summary.md` + updated `master-progress.md`

**Files:**
- [README.md](./workflows/05-weekly-retrospective/README.md) — 3 parts
- [template.md](./workflows/05-weekly-retrospective/template.md) — Form to fill
- [ai-prompt.md](./workflows/05-weekly-retrospective/ai-prompt.md) — AI instructions (17K)

**Quick:** Analyze week results, capture learnings, plan improvements

---

## File Structure

```
.
├── CLAUDE.md                    ← AI entry point
├── WORKFLOWS.md                 ← 5 workflows overview
├── QUICK_REFERENCE.md          ← Print & keep visible ⭐
├── AI_WORKFLOW_GUIDE.md        ← How to use AI
├── INDEX.md                     ← This file
│
├── workflows/
│   ├── 01-project-planning/
│   │   ├── README.md           ← Human instructions
│   │   ├── template.md         ← Blank form
│   │   └── ai-prompt.md        ← AI instructions ⭐
│   │
│   ├── 02-weekly-planning/
│   │   ├── README.md
│   │   ├── template.md
│   │   └── ai-prompt.md        ⭐
│   │
│   ├── 03-daily-planning/
│   │   ├── README.md
│   │   ├── template.md
│   │   └── ai-prompt.md        ⭐
│   │
│   ├── 04-daily-tracking/
│   │   ├── README.md
│   │   ├── template.md
│   │   └── ai-prompt.md        ⭐
│   │
│   └── 05-weekly-retrospective/
│       ├── README.md
│       ├── template.md
│       └── ai-prompt.md        ⭐
│
└── old-files/                   ← Original documentation (archived)
    ├── README.md
    ├── 00-START-HERE.md
    ├── METHODOLOGY_GUIDE.md
    ├── README_TEMPLATES.md
    ├── guides/
    └── templates/
```

---

## Total Content

| Type | Count | Size |
|------|-------|------|
| Root files | 4 | 25K |
| Workflow README.md | 5 | 10K |
| Workflow template.md | 5 | 8K |
| Workflow ai-prompt.md | 5 | 51K |
| **Total** | **19** | **94K** |

All files are complete, ready to use, and optimized for both human and AI collaboration.

---

## How to Use This Repository

### For Project Setup (Week 0)

1. Read [WORKFLOWS.md](./WORKFLOWS.md)
2. Go to [Workflow 1: Project Planning](./workflows/01-project-planning/README.md)
3. Follow the 5 steps
4. Output: `docs/plan/master-plan.md`

### For Ongoing Weekly Cycle

**Monday Morning:**
1. Go to [Workflow 2: Weekly Planning](./workflows/02-weekly-planning/README.md)
2. Provide context (previous week data, current state)
3. Generate or ask AI to generate `week-X-plan.md`
4. Team alignment meeting

**Every Day at 9 AM:**
1. Go to [Workflow 3: Daily Planning](./workflows/03-daily-planning/README.md)
2. Create 3-4 specific tasks with acceptance criteria
3. Generate `day-Y-plan.md`

**Every Day at 5 PM:**
1. Go to [Workflow 4: Daily Tracking](./workflows/04-daily-tracking/README.md)
2. Log actual time, completed tasks, quality results
3. Update `progress.md`
4. Get PM review and sign-off

**Friday 4:30 PM:**
1. Go to [Workflow 5: Weekly Retrospective](./workflows/05-weekly-retrospective/README.md)
2. Team retrospective discussion
3. Generate `summary.md`
4. Update `master-progress.md`

### With AI Help

1. Choose which workflow you need
2. Give AI the corresponding `ai-prompt.md` file
3. Provide your context (previous week data, current state, goals)
4. AI generates complete, ready-to-use document
5. You review and approve

See [AI_WORKFLOW_GUIDE.md](./AI_WORKFLOW_GUIDE.md) for detailed AI instructions.

---

## Quick Decision Tree

```
Q: Where do I start?
└─ NEW PROJECT
   └─ Go to Workflow 1: Project Planning

Q: What do I do Monday?
└─ WEEKLY PLANNING
   └─ Go to Workflow 2: Weekly Planning

Q: What do I do every morning?
└─ DAILY PLANNING
   └─ Go to Workflow 3: Daily Planning

Q: How do I track progress during work?
└─ DAILY TRACKING
   └─ Go to Workflow 4: Daily Tracking

Q: What do I do Friday?
└─ WEEKLY RETROSPECTIVE
   └─ Go to Workflow 5: Weekly Retrospective

Q: I want AI to help
└─ HOW TO USE AI
   └─ Read AI_WORKFLOW_GUIDE.md, then give AI the ai-prompt.md for your workflow
```

---

## Key Principles (Never Break These)

✅ **Plan Once, Track Daily**
- Plans (master, weekly, daily) rarely change
- Tracking (progress, execution) updated every day
- Don't duplicate info

✅ **Daily Verification**
- PM reviews every day, not just Friday
- Definition of done is testable and specific
- Issues caught immediately

✅ **Feedback Loop**
- Retrospectives inform next week's planning
- Velocity data drives adjustments
- Continuous improvement

✅ **Clear Entry Points**
- Each workflow stands alone
- AI can follow any workflow independently
- No confusion about what to do

---

## Success Indicators

You're using this well when:

✅ Each day produces independently testable work
✅ PM verifies daily (not weekly)
✅ Blockers caught and resolved same day
✅ Team velocity improves week-to-week
✅ Retrospectives identify concrete improvements
✅ Estimates become more accurate
✅ Complete documentation trail exists
✅ AI can generate high-quality outputs

---

## Support

**Questions about the methodology?**
- Humans: Read the README.md files
- AI: Read the ai-prompt.md files

**Need an example?**
- Each ai-prompt.md has detailed examples

**Want to customize?**
- Templates are starting points, adapt as needed
- Keep core principles (daily verification, feedback loop)

**Having issues?**
- Check QUICK_REFERENCE.md for "Red Flags"
- Check the troubleshooting in AI_WORKFLOW_GUIDE.md

---

## Files You Should Know

| File | Purpose | When |
|------|---------|------|
| [WORKFLOWS.md](./WORKFLOWS.md) | Overview | Start here |
| [QUICK_REFERENCE.md](./QUICK_REFERENCE.md) | Cheat sheet | Print it |
| [AI_WORKFLOW_GUIDE.md](./AI_WORKFLOW_GUIDE.md) | AI instructions | Using AI |
| Each `README.md` | Step-by-step | Doing the work |
| Each `template.md` | Blank form | Creating document |
| Each `ai-prompt.md` | AI prompt | Asking AI |

---

## Next Steps

1. **Today:** Read [WORKFLOWS.md](./WORKFLOWS.md) (3 min)
2. **Today:** Print [QUICK_REFERENCE.md](./QUICK_REFERENCE.md)
3. **Choose:** What workflow do you need?
4. **Do:** Follow that workflow's README.md
5. **Ready:** Start generating documents

---

**Everything you need is here. You're ready to start.**

Choose a workflow. Follow it. Generate documents. Build.

🚀
