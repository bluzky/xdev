# Workflow 4: Daily Tracking

**Duration:** 5 minutes (updates) + 10 minutes (end of day)
**When:** Throughout day + 5 PM
**Output:** `docs/plan/week-X/progress.md`

---

## What to Do

Track actual progress as work happens.

### During Day (Throughout)

**Every 1-2 hours, update day-Y-plan.md:**

In the "Execution → Progress Log" section, add timestamps:

```
[2:15 PM] — Task 1 complete, all buttons rendering correctly
[3:30 PM] — Task 2 started, implementing recording logic
[4:45 PM] — Found issue with file path, fixed
[5:00 PM] — All tests passing, ready for PM review
```

**What to log:**
- When you complete something
- When you hit a blocker
- When you find/fix an issue
- Time-based progress

---

### End of Day (5:00 PM)

**In day-Y-plan.md, fill in:**

1. **Actual Time Spent** (how long did it really take?)
2. **Tasks Completed** (mark them done)
3. **Blockers** (any issues you hit?)
4. **Quality Check** (tests pass? Build clean?)
5. **Learnings** (anything discovered?)

Example:
```
Time Spent: 7.5 hours (estimated: 8 hours)

Tasks Completed:
- [x] Task 1: Recording UI
- [x] Task 2: Recording logic
- [x] Task 3: Testing

Blockers:
- None

Quality Check:
- [x] Build: 0 errors, 0 warnings
- [x] Tests: 100% passing (42/42)
- [x] Manual: All scenarios pass

Learnings:
- File API faster than expected
- Need to handle permissions earlier
```

---

### End of Day (5:30 PM)

**In progress.md, add a section for today:**

```markdown
## Day Y - [Title]

**Status:** ✅ Complete

**Completed:**
- Recording UI implemented
- Recording logic working
- All tests passing

**Time:** 7.5 hours (est: 8 hours)

**Blockers:** None

**Next day:**
- Begin audio capture integration
```

---

## What Goes in progress.md

Create one section per day:

```markdown
## Day 1 (Monday)

**Status:** ✅ Complete
**Objectives:** Set up project, build UI
**Completed:** 5/5 planned tasks
**Actual Time:** 7.5 hours (est: 8)
**Blockers:** None
**Quality:** ✅ All tests pass, build clean

---

## Day 2 (Tuesday)

**Status:** ✅ Complete
**Objectives:** Implement recording
**Completed:** 4/4 planned tasks
**Actual Time:** 8 hours (est: 8)
**Blockers:** None
**Quality:** ✅ All tests pass

---

## Summary

**Week Progress:** 5/5 days complete
**Velocity:** 38.5 hours actual vs 40 estimated
**Build Quality:** Clean (0 errors, 0 warnings)
**Test Pass Rate:** 100%
**Blockers:** None this week
```

---

## Template to Use

→ Copy and use: [template.md](./template.md)

---

## Key Rules

- **Log as you go:** Don't wait until end of day
- **Be specific:** "Implemented video capture" not "worked on stuff"
- **Track time:** Actual vs estimated helps improve estimates
- **Note blockers:** Same day, not Friday
- **Update before PM review:** Execution section must be complete

---

## PM Review (4:30 PM)

PM will review day-Y-plan.md execution section:
- Does definition of done match actual completion?
- Do tests pass?
- Is quality acceptable?
- Any concerns?

**If approved:** ✅ Approved
**If not:** 🔄 List what needs fixing

---

## Checklist at End of Day

- [ ] day-Y-plan.md execution section is filled in
- [ ] Progress log has timestamps of work
- [ ] Actual time logged
- [ ] All tasks marked complete/incomplete
- [ ] Blockers documented
- [ ] Quality checks done
- [ ] Learnings captured
- [ ] progress.md updated with day's results
- [ ] Ready for PM review

---

## Next Workflow

→ Go to [Workflow 5: Weekly Retrospective](../05-weekly-retrospective/)

Do this every day. Friday, also do the weekly retrospective.
