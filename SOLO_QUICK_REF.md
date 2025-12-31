# Solo Dev + AI: Quick Reference

**Print this. Keep it visible.**

---

## Your Weekly Rhythm

```
MONDAY 9:00 AM
  └─ (30 min) Plan the week → week-X-plan.md

EVERY DAY 9:00 AM
  └─ (10 min) Ask AI to plan day → day-Y-plan.md
  └─ Work all day (use AI as partner)
  └─ (5 min) Log actual hours at 5 PM

FRIDAY 5:00 PM
  └─ (30 min) Write week summary → summary.md
  └─ Done!
```

---

## The 4 Workflows

| When | Workflow | File | Time |
|------|----------|------|------|
| Once (Week 0) | [Project Setup](./solo/01-project-setup/README.md) | project-plan.md | 30 min |
| Every Monday | [Weekly Plan](./solo/02-weekly-plan/README.md) | week-X-plan.md | 30 min |
| Every Morning | [Daily Plan](./solo/03-daily-plan/README.md) | day-Y-plan.md | 10 min |
| Every Friday | [Weekly Review](./solo/04-weekly-review/README.md) | summary.md | 30 min |

---

## Use AI For

✅ **Daily Plans** (2 min)
```
"Plan my day following solo/03-daily-plan/ai-prompt.md

Goal: [today's goal from weekly plan]
Time: ~8 hours

Generate day-Y-plan.md with 3-4 tasks"
```

✅ **Weekly Plans** (optional)
```
"Plan this week following solo/02-weekly-plan/ai-prompt.md

Goal: [what should exist by Friday]
Previous: [last week's results if available]

Generate week-X-plan.md"
```

✅ **Code Help** (anytime)
```
"I'm stuck on [problem]. Help me [fix/implement/debug] [thing]"
```

✅ **Weekly Summary** (optional)
```
"Draft week-X summary following solo/04-weekly-review/ai-prompt.md

This week:
- Estimated: 40 hours, Actual: [actual]
- Completed: [list]
- Blockers: [list]

Generate summary.md"
```

---

## Day Plan Structure

```
Definition of Done: [Specific, testable criteria]

Task 1: [Name] (~2.5 hours)
  What: [Description]
  Why: [Why it matters]
  Acceptance: [Testable outcomes]

Task 2: [Name] (~2.5 hours)
  What: [Description]
  Why: [Why it matters]
  Acceptance: [Testable outcomes]

Task 3: [Name] (~2 hours)
  What: [Description]
  Why: [Why it matters]
  Acceptance: [Testable outcomes]

Task 4: Testing (~1 hour)
  What: Manual test + verify quality
  Build: 0 errors, 0 warnings
  Tests: 100% passing
```

---

## At 5 PM Every Day

**In day-Y-plan.md:**
- [ ] Mark tasks done/incomplete
- [ ] Log actual hours (vs estimate)
- [ ] Note any blockers

**In progress.md:**
- [ ] Add day's entry
- [ ] What completed
- [ ] Actual time
- [ ] Any blockers

**Takes:** 5 minutes

---

## Friday Evening (30 min)

**Write summary.md:**
- What got done vs planned?
- What was harder/easier?
- What to improve?
- Metrics (hours, velocity)

**Update master-progress.md:**
- Week X results
- Quick wins
- Next week preview

---

## Definition of Done Rules

✅ **Good (specific):**
- User can click Record button
- Button changes to "Stop"
- Tests pass (12/12)
- Build clean (0 errors)

❌ **Bad (vague):**
- Recording works
- Tests pass
- No errors

---

## Metrics You Track

**Weekly:**
- Estimated vs actual hours
- What you accomplished
- Build quality (0 errors target)
- Test coverage (100% target)

**Over Time:**
- Is velocity stable?
- Are estimates improving?
- Is quality improving?

---

## Daily Work Flow

```
9:00 AM
  └─ Ask AI to create day plan (2 min)
  └─ Review plan (3 min)
  └─ Start work (9:05 AM)

Throughout Day
  └─ Follow the plan
  └─ Work with AI (ask questions, pair program)
  └─ Log progress every 1-2 hours
  └─ Test as you go

4:00 PM
  └─ Complete final tasks
  └─ Run all tests
  └─ Verify build clean

5:00 PM
  └─ Update execution section in day plan (5 min)
  └─ Update progress.md (5 min)
  └─ Review quality checklist

5:30 PM
  └─ Done for the day!
```

---

## Red Flags (Fix These)

🚩 **Definition of Done is vague**
→ Stop, rewrite with specific criteria

🚩 **More than 4 tasks in a day**
→ Too much. Remove or split across days.

🚩 **Don't track time during the day**
→ At 5 PM, estimate as best you can. Don't skip.

🚩 **Tests not passing**
→ Fix before day ends. Definition of done requires 100%.

🚩 **Build has errors**
→ Fix before day ends. Definition of done requires 0.

---

## Files You Need

| Location | Purpose |
|----------|---------|
| solo/01-project-setup/ | Create once |
| solo/02-weekly-plan/ | Create each Monday |
| solo/03-daily-plan/ | Create each morning |
| solo/04-weekly-review/ | Create each Friday |
| docs/plan/project-plan.md | Your project vision |
| docs/plan/week-X-plan.md | Weekly scope |
| docs/plan/week-X/day-Y-plan.md | Daily plan |
| docs/plan/week-X/progress.md | Track days |
| docs/plan/week-X/summary.md | Week reflection |
| docs/plan/master-progress.md | Project status |

---

## AI Prompts Location

To ask AI for help, give it:

| Workflow | Prompt File |
|----------|------------|
| Project Setup | solo/01-project-setup/ai-prompt.md |
| Weekly Plan | solo/02-weekly-plan/ai-prompt.md |
| Daily Plan | solo/03-daily-plan/ai-prompt.md ← Use daily |
| Weekly Review | solo/04-weekly-review/ai-prompt.md |

---

## Success Looks Like

✅ Each day produces working code
✅ Days are independently testable
✅ Build stays clean (0 errors, all days)
✅ Tests pass (100%, all days)
✅ Velocity is predictable
✅ You know what to do next without thinking
✅ AI helps you move faster
✅ No meetings, all execution

---

## One Week Schedule

```
MONDAY
  9:00 AM: Weekly plan (30 min)
  9:30 AM: Daily plan (10 min)
  10:00 AM: Start work
  5:00 PM: Log hours (5 min)

TUESDAY-THURSDAY (Same Daily Pattern)
  9:00 AM: Daily plan (10 min)
  10:00 AM: Work
  5:00 PM: Log hours (5 min)

FRIDAY
  9:00 AM: Daily plan (10 min)
  10:00 AM: Work
  5:00 PM: Log hours (5 min)
  5:30 PM: Weekly summary (30 min)
```

**Total overhead:** ~2 hours per week
**Benefit:** Clear direction, AI partnership, velocity tracking

---

## Questions?

**What if I can't finish my task?**
→ Update day plan. Note blockers. Continue tomorrow.

**Tests are failing. Do I stop?**
→ Yes. Definition of done requires 100% pass.

**Can I skip the daily plan?**
→ No, but AI generates it in 2 minutes. Use AI.

**Can I skip Friday review?**
→ You can, but 30 minutes saves rework next week.

**What if I work 10 hours/day?**
→ Same process, adjust hours. Still use daily plans.

---

## Start Now

1. **Today:** Read [SOLO_DEV_START.md](./SOLO_DEV_START.md)
2. **This week:** Create project-plan.md using [solo/01-project-setup/](./solo/01-project-setup/README.md)
3. **Next Monday:** Create week-1-plan.md
4. **Next Monday 10 AM:** Ask AI to create day-1-plan.md
5. **Start building!**

---

**You've got everything you need. The system is simple. You + AI. Build.**
