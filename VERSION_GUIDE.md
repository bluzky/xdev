# Two Versions: Team vs Solo Dev

This repository has **two complete, independent versions** of the development methodology.

Choose based on your situation.

---

## Quick Decision

### I'm a solo developer
→ Use **SOLO** version
→ Start with [SOLO_DEV_START.md](./SOLO_DEV_START.md)

### I'm leading a team
→ Use **TEAM** version
→ Start with [WORKFLOWS.md](./WORKFLOWS.md)

### I'm using both
→ Use SOLO for personal work, TEAM for team projects
→ Files don't conflict (different directories)

---

## Side-by-Side Comparison

| Aspect | SOLO | TEAM |
|--------|------|------|
| **Workflows** | 4 simple | 5 detailed |
| **Templates** | Minimal | Comprehensive |
| **AI Role** | Coding partner | Support tool |
| **Complexity** | Low | Medium |
| **Meetings** | None | Daily + weekly |
| **Verification** | Self-check | PM sign-off |
| **Time Overhead** | ~2 hrs/week | ~3-4 hrs/week |
| **Best For** | Solo dev + AI | Teams 3+ people |

---

## SOLO VERSION (For You Alone + AI)

**Location:** `solo/` directory

**Files:** 12 files total (4 workflows × 3 files)

**Key Characteristics:**
- ✅ No team meetings or sign-offs
- ✅ AI is your coding partner throughout the day
- ✅ Quick daily 10-minute plans
- ✅ Self-verification (you verify quality)
- ✅ Solo 30-minute Friday reflection
- ✅ ~2 hours/week overhead

**Workflows:**
1. [Project Setup](./solo/01-project-setup/README.md) — Once, Week 0
2. [Weekly Plan](./solo/02-weekly-plan/README.md) — Monday 30 min
3. [Daily Plan](./solo/03-daily-plan/README.md) — Every 9 AM, 10 min
4. [Weekly Review](./solo/04-weekly-review/README.md) — Friday 30 min

**Start:** [SOLO_DEV_START.md](./SOLO_DEV_START.md)

**Quick Ref:** [SOLO_QUICK_REF.md](./SOLO_QUICK_REF.md) (print this)

---

## TEAM VERSION (For Teams)

**Location:** `workflows/` directory

**Files:** 15 files total (5 workflows × 3 files)

**Key Characteristics:**
- ✅ Clear team communication
- ✅ PM reviews daily work
- ✅ Team alignment meetings
- ✅ Detailed daily plans
- ✅ Team retrospectives Friday
- ✅ Complete documentation
- ✅ ~3-4 hours/week overhead

**Workflows:**
1. [Project Planning](./workflows/01-project-planning/README.md) — Week 0
2. [Weekly Planning](./workflows/02-weekly-planning/README.md) — Monday 1-2 hrs
3. [Daily Planning](./workflows/03-daily-planning/README.md) — Every 9 AM, 15-30 min
4. [Daily Tracking](./workflows/04-daily-tracking/README.md) — Throughout day + 5 PM
5. [Weekly Retrospective](./workflows/05-weekly-retrospective/README.md) — Friday 1 hr

**Start:** [WORKFLOWS.md](./WORKFLOWS.md)

**Quick Ref:** [QUICK_REFERENCE.md](./QUICK_REFERENCE.md) (print this)

**AI Guide:** [AI_WORKFLOW_GUIDE.md](./AI_WORKFLOW_GUIDE.md)

---

## Feature Comparison

### Planning

**SOLO:**
- 30-minute weekly planning (you alone)
- 10-minute daily planning (ask AI to generate)
- Simple templates (fill in key points)

**TEAM:**
- 1-2 hour weekly planning (with team input)
- 15-30 minute daily planning (detailed)
- Comprehensive templates (cover all aspects)
- Team alignment meetings after planning

---

### Execution

**SOLO:**
- Work independently with AI as partner
- Log hours at end of day (5 min)
- Self-verify quality (tests, build)
- Ask AI for code help anytime

**TEAM:**
- Developers work with AI support
- PM available for questions
- Daily PM review at 4:30 PM
- PM verifies and signs off each day
- Blockers documented immediately

---

### Documentation

**SOLO:**
- Day plan + progress log (track yourself)
- Weekly summary (personal reflection)
- Master progress (high-level status)
- Minimal overhead

**TEAM:**
- Detailed day plans (PM reviewed)
- Execution tracking (daily updates)
- Progress log (weekly aggregate)
- Weekly summaries (with team input)
- Comprehensive retrospectives

---

### Velocity & Metrics

**SOLO:**
- Track your own velocity
- Adjust estimates based on actual hours
- Simple metrics (hours, tasks done, quality)
- Personal improvement focus

**TEAM:**
- Team velocity tracked
- Metrics used for next sprint planning
- Shared metrics visibility
- Team improvement retrospectives

---

## Timeline Overhead

### SOLO Version

```
MONDAY:        30 min (plan week)
EVERY MORNING: 10 min (plan day - AI generates)
FRIDAY:        30 min (review week)
DAILY:         10 min (log hours at 5 PM)

Total: ~2 hours/week
```

### TEAM Version

```
MONDAY:        1-2 hours (plan week + align)
EVERY MORNING: 15-30 min (plan day)
EVERY DAY:     20 min (PM review at 4:30 PM)
FRIDAY:        1 hour (retrospective + summary)
DAILY:         10 min (log progress)

Total: ~3-4 hours/week
```

---

## Which Version to Choose?

### Use SOLO if:
- ✅ You're a solo developer
- ✅ You're using AI as your main collaborator
- ✅ You want minimal meetings/overhead
- ✅ You need quick feedback from AI
- ✅ You're comfortable self-verifying quality

### Use TEAM if:
- ✅ You have 3+ developers
- ✅ You need PM oversight
- ✅ You want formal sign-offs
- ✅ You need team coordination
- ✅ Detailed documentation is important

### Use BOTH if:
- ✅ You do both solo projects AND team projects
- They don't conflict (different directories)
- Pick whichever matches your current situation

---

## File Organization

```
Repository Root
├── SOLO_DEV_START.md          ← Solo dev entry point
├── SOLO_QUICK_REF.md          ← Solo quick reference
│
├── WORKFLOWS.md               ← Team entry point
├── QUICK_REFERENCE.md         ← Team quick reference
├── AI_WORKFLOW_GUIDE.md       ← How to use AI with team version
├── CLAUDE.md                  ← AI entry point (both versions)
├── INDEX.md                   ← File index
├── VERSION_GUIDE.md           ← This file
│
├── solo/                      ← SOLO VERSION (4 workflows)
│   ├── 01-project-setup/
│   ├── 02-weekly-plan/
│   ├── 03-daily-plan/
│   └── 04-weekly-review/
│
├── workflows/                 ← TEAM VERSION (5 workflows)
│   ├── 01-project-planning/
│   ├── 02-weekly-planning/
│   ├── 03-daily-planning/
│   ├── 04-daily-tracking/
│   └── 05-weekly-retrospective/
│
└── old-files/                 ← Archive (original docs)
    └── README.md
```

---

## For AI: Understanding Both Versions

**SOLO version AI prompts:**
- Shorter, more conversational
- Assume you're helping one person
- Focus on speed (2-minute generation)
- Encourage iteration/refinement

**TEAM version AI prompts:**
- More structured
- Assume you're helping a team
- Focus on completeness
- Account for coordination overhead

When a user asks for help:
1. Check which version they're using
2. Read the correct ai-prompt.md file
3. Follow the instructions in that prompt

---

## Starting Your First Project

### With SOLO Version

```
Step 1: Read SOLO_DEV_START.md (5 min)
Step 2: Create project-plan.md using solo/01-project-setup/ (30 min)
Step 3: Monday: Create week-1-plan.md using solo/02-weekly-plan/ (30 min)
Step 4: Monday 10 AM: Ask AI to create day-1-plan.md
Step 5: Start building!
Step 6: Every day at 5 PM: Log hours
Step 7: Friday 5 PM: Write week summary

Total setup: 1 hour
Then: 2 hours/week overhead
```

### With TEAM Version

```
Step 1: Read WORKFLOWS.md (3 min)
Step 2: Create master-plan.md using workflows/01-project-planning/ (2-4 hours)
Step 3: Create master-progress.md
Step 4: Brief team on methodology (30 min)
Step 5: Monday: Create week-1-plan.md using workflows/02-weekly-planning/ (1-2 hours)
Step 6: Monday 10 AM: Team alignment meeting (1 hour)
Step 7: Monday 10:30 AM: Each person creates their day-1-plan.md
Step 8: Development starts
Step 9: Daily 4:30 PM: PM reviews each person's work
Step 10: Friday: Team retrospective + write summary

Total setup: 4-6 hours
Then: 3-4 hours/week overhead
```

---

## Switching Between Versions

If you start with SOLO and later need TEAM:
- Keep your SOLO project files
- Start a new TEAM project (different directory)
- Files don't conflict

If you start with TEAM and later go solo:
- Keep your TEAM project files
- Start a new SOLO project
- Pick whichever makes sense for your situation

---

## Summary

| Need | Use | Start |
|------|-----|-------|
| Solo dev + AI | SOLO | [SOLO_DEV_START.md](./SOLO_DEV_START.md) |
| Team development | TEAM | [WORKFLOWS.md](./WORKFLOWS.md) |
| Quick reference | Either | QUICK_REFERENCE.md or SOLO_QUICK_REF.md |
| AI help | Either | AI_WORKFLOW_GUIDE.md (TEAM) or read ai-prompt.md files |

---

**Choose your version. Start your project. Build great things.**

Both versions work. Pick what matches your situation. 🚀
