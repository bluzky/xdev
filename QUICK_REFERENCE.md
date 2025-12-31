# Quick Reference Card

Print this. Keep it visible. Refer to it constantly.

---

## Workflow Decision Tree

```
┌─ Are you starting a new project?
│  └─ YES → Workflow 1: Project Planning
│           (2-4 hours, Week 0)
│
├─ Is it Monday morning?
│  └─ YES → Workflow 2: Weekly Planning
│           (1-2 hours, 9 AM)
│
├─ Is it any morning, 9 AM?
│  └─ YES → Workflow 3: Daily Planning
│           (15-30 min, every day)
│
├─ Are you working (or it's 5 PM)?
│  └─ YES → Workflow 4: Daily Tracking
│           (5 min updates + 10 min at 5 PM)
│
└─ Is it Friday 4:30 PM?
   └─ YES → Workflow 5: Weekly Retrospective
            (1 hour, Friday evening)
```

---

## The Weekly Cycle

```
MONDAY 9:00 AM
  ├─ Create week-X-plan.md (1 hour)
  ├─ Team alignment meeting (10-11 AM)
  └─ Create day-1-plan.md (20 min)
  └─ Start work at 10:30 AM

MONDAY-FRIDAY (Each Day)
  ├─ 9:00 AM
  │  └─ Create day-Y-plan.md
  │  └─ Review definition of done
  │
  ├─ 10:00 AM-4:00 PM
  │  └─ Work (log progress every 1-2 hours)
  │
  ├─ 4:00 PM
  │  └─ Complete execution notes
  │  └─ Run all tests
  │  └─ Update progress.md
  │
  ├─ 4:30 PM
  │  └─ PM reviews day-Y-plan.md
  │  └─ PM signs off: ✅ Approved / 🔄 Revision
  │
  └─ 5:00 PM
     └─ Mark day complete
     └─ Notes for next day

FRIDAY 4:30 PM
  ├─ Team retrospective discussion (20 min)
  ├─ Write summary.md (30 min)
  ├─ Update master-progress.md (10 min)
  └─ Done!
```

---

## Key Rules (Don't Break These)

| Rule | Why |
|------|-----|
| **Definition of Done is specific & testable** | Vague criteria = failed reviews |
| **PM signs off DAILY** | Issues caught immediately, not Friday |
| **Track actual time vs estimate** | Improves estimates, measures velocity |
| **Update progress same day** | Blockers documented quickly |
| **No more than 3-4 tasks per day** | Overload = failure + bad estimates |
| **100% test pass rate required** | Quality gate, catches bugs early |
| **Retrospective is mandatory** | Learnings drive next week's plan |

---

## Document Checklist

### Before You Start Work Each Day

- [ ] day-Y-plan.md created and reviewed
- [ ] Definition of Done is clear
- [ ] You understand all 3-4 tasks
- [ ] No blockers from yesterday
- [ ] Tests are ready to run

### At 5:00 PM

- [ ] day-Y-plan.md execution section filled
- [ ] Actual time logged
- [ ] All tasks marked complete/incomplete
- [ ] Blockers documented
- [ ] Quality checks passed (tests, build)
- [ ] progress.md updated with day results
- [ ] Ready for PM review

### Friday at 5:30 PM

- [ ] summary.md created
- [ ] Metrics captured (hours, velocity, quality)
- [ ] Learnings documented
- [ ] Adjustments for next week identified
- [ ] master-progress.md updated

---

## Template Quick Access

| File | When | Location |
|------|------|----------|
| master-plan.md | Week 0 | workflows/01-project-planning/template.md |
| week-X-plan.md | Monday | workflows/02-weekly-planning/template.md |
| day-Y-plan.md | Every day | workflows/03-daily-planning/template.md |
| progress.md | Daily tracking | workflows/04-daily-tracking/template.md |
| summary.md | Friday | workflows/05-weekly-retrospective/template.md |

---

## Red Flags (Stop and Fix These)

🚩 **Definition of Done is vague**
→ Go back and make it testable. Specific criteria only.

🚩 **More than 5 tasks in a day plan**
→ You've packed too much. Remove or move to next day.

🚩 **Didn't track time during the day**
→ At 5 PM, estimate as best you can, but don't skip it.

🚩 **PM review skipped**
→ Issues pile up. Review must happen, even if brief.

🚩 **Progress not updated until Friday**
→ Blockers discovered too late. Update daily.

🚩 **Tests not passing**
→ Don't commit. Fix first. Definition of done requires 100% pass.

🚩 **Retrospective skipped**
→ No learnings → same mistakes next week. Do it, even if short.

---

## Common Questions

**Q: What if I can't finish my day's tasks?**
A: Update day-Y-plan.md with what you DID finish. Note what remains. Move incomplete tasks to tomorrow or next week.

**Q: Tests are failing. Do I stop?**
A: Yes. Definition of Done requires 100% pass. Fix tests before calling day complete.

**Q: Can I skip the retrospective?**
A: No. Even 20 minutes is better than nothing. Write down 3 things: went well, was hard, will improve.

**Q: What if my estimates are always off?**
A: That's OK. Track actual vs estimate. After 2-3 weeks, patterns emerge. Use that data to improve.

**Q: Can I work on multiple weeks' tasks?**
A: No. Focus on current week. Multi-week context switching kills productivity.

**Q: What do I do with incomplete work at end of week?**
A: Document it in summary.md. Explain why. Add to next week's plan. Don't carry guilt.

---

## Success Checklist (By Week End)

- ✅ All P0 objectives complete
- ✅ Build: 0 errors, 0 warnings (all 5 days)
- ✅ Tests: 100% pass rate
- ✅ PM signed off on every day
- ✅ Progress tracked daily
- ✅ Blockers documented same day
- ✅ summary.md written with learnings
- ✅ master-progress.md updated
- ✅ Next week's plan prepared (if needed)
- ✅ Team retrospective completed

---

## Metrics to Track

**Weekly:**
- Estimated hours vs actual hours (velocity)
- Test pass rate (target: 100%)
- Build quality (errors + warnings = 0)
- P0 objectives completed (target: 100%)

**Over Time:**
- Is velocity improving or stable?
- Are estimates getting more accurate?
- Is build quality improving?
- Are blockers decreasing?

---

## Links

- **Full Guide:** [WORKFLOWS.md](./WORKFLOWS.md)
- **Workflow 1:** [Project Planning](./workflows/01-project-planning/README.md)
- **Workflow 2:** [Weekly Planning](./workflows/02-weekly-planning/README.md)
- **Workflow 3:** [Daily Planning](./workflows/03-daily-planning/README.md)
- **Workflow 4:** [Daily Tracking](./workflows/04-daily-tracking/README.md)
- **Workflow 5:** [Weekly Retrospective](./workflows/05-weekly-retrospective/README.md)

---

**Print this. Follow it. Win.**
