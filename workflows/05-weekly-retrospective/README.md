# Workflow 5: Weekly Retrospective

**Duration:** 1 hour total
**When:** Friday 4:30 PM
**Output:** `docs/plan/week-X/summary.md` + updated `master-progress.md`

---

## What to Do

Reflect on the week, capture learnings, plan improvements.

### Part 1: Team Retrospective (20 min)

Gather the team Friday 4:30 PM. Discuss:

**What went well?**
- What were we efficient at?
- What was easier than expected?
- Which decisions worked great?

**What was harder?**
- What took longer than estimated?
- Where did we get stuck?
- What was underestimated?

**What surprised us?**
- What did we learn about this project?
- What technical insight emerged?
- Any unexpected blockers?

**What can we improve?**
- Process: How should we work differently?
- Estimation: What should we adjust next week?
- Architecture: Any refactoring needed?

---

### Part 2: Write Summary (30 min)

Create `week-X/summary.md` with:

1. **What got done**
   - P0 objectives completed
   - Additional achievements
   - Quality metrics

2. **What didn't get done**
   - P1/P2 items moved to next week
   - Why (time, complexity, blockers)

3. **Metrics**
   - Hours estimated vs actual
   - Test pass rate
   - Build quality (errors/warnings)

4. **Learnings**
   - What we discovered about the project
   - Technical insights
   - Process improvements

5. **Adjustments for Next Week**
   - What to do differently
   - What estimates to adjust
   - New approach to try

---

### Part 3: Update Master Progress (10 min)

In `master-progress.md`, add:

```markdown
## Week X Results

**Phase:** Phase X - [Name]
**Status:** ✅ Complete

**Objectives:** [List P0 objectives]
**Completed:** [Which ones done]
**Velocity:** X hours actual vs Y estimated

**Quality:** Build clean, 100% tests passing
**Blockers:** [Any major blockers encountered]

**Next Week:** [Preview of what's coming]
```

---

## Template to Use

→ Copy and use: [template.md](./template.md)

---

## Key Output: Insights for Next Week

The retrospective should answer:

1. **Velocity:** Did we estimate correctly?
   - If actual > estimated: reduce scope next week or extend timeline
   - If actual < estimated: increase scope next week or celebrate

2. **Quality:** Is the build getting better?
   - Track errors/warnings over time
   - Track test pass rate over time
   - Identify patterns in failures

3. **Process:** Should we work differently?
   - Daily planning too long/short?
   - PM review timing working?
   - Team communication sufficient?

4. **Blockers:** What keeps slowing us down?
   - Technical (architecture, dependencies)
   - Process (unclear requirements, approval delays)
   - Resource (not enough time, skills gaps)

---

## Friday Evening Tasks

1. **4:30-4:50 PM:** Team retrospective (discussion)
2. **4:50-5:20 PM:** Write summary.md
3. **5:20-5:30 PM:** Update master-progress.md
4. **5:30-6:00 PM:** (Optional) Plan Week X+1 prep

---

## Checklist Before Leaving Friday

- [ ] Team discussion completed
- [ ] summary.md created with all sections
- [ ] Metrics captured (hours, quality, blockers)
- [ ] Learnings documented
- [ ] Adjustments identified for next week
- [ ] master-progress.md updated
- [ ] Team knows what to expect next week

---

## Using Retrospective Data

**Monday morning** when creating next week's plan:
1. Review this week's summary.md
2. Note velocity (actual hours vs estimate)
3. Check if blockers are ongoing
4. Adjust estimates for similar work
5. Identify improved approach based on learnings

This creates a **feedback loop:**
```
Retrospective → Learnings → Next Week's Plan → Better Execution
```

---

## Next Cycle

After completing retrospective:

**Friday Evening/Monday Early:** Prepare [Workflow 2: Weekly Planning](../02-weekly-planning/)

Create `week-X+1-plan.md` for next Monday.

---

## Tips for Good Retrospectives

✅ **Do:**
- Be honest about what was hard
- Celebrate what went well
- Focus on process, not people
- Make concrete improvements
- Document for future reference

❌ **Don't:**
- Blame individuals
- Skip the retrospective
- Say "we'll do better" without specifics
- Ignore data (velocity, metrics)
- Make plans without learning from this week
