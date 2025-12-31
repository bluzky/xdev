# Workflow 2: Weekly Planning

**Duration:** 1-2 hours
**When:** Monday morning, before 10 AM
**Output:** `docs/plan/week-X-plan.md`

---

## What to Do

Follow these 4 steps to plan your week.

### Step 1: Review Context (15 min)

Gather information:
- [ ] Read master-plan.md (what phase are we in?)
- [ ] Read last week's summary.md (what did we learn?)
- [ ] Check this week's phase from master-plan.md
- [ ] Note team capacity (who's available?)

---

### Step 2: Define Week Scope (20 min)

Answer these questions:

**What state are we in?**
- What exists today (before this week)
- What should exist by Friday

**What are the priorities?**
- P0 (must-have, required for phase)
- P1 (should-have, if time allows)
- P2 (nice-to-have, low priority)

Example:
```
P0: Recording UI functional
P0: Audio capture integrated
P1: Performance tested
P2: Edge cases handled
```

---

### Step 3: Create Daily Breakdown (25 min)

For each of 5 days, write:
- **Goal:** What this day accomplishes (1 sentence)
- **Hours:** Estimate (usually 6-7 hours/day)
- **Deliverable:** What gets tested/verified

Example:
```
Day 1: Set up project structure, UI framework, basic buttons
  ~7 hours | Test: All UI renders, buttons clickable

Day 2: Implement recording controls and status display
  ~7 hours | Test: Controls work, status updates in real-time
```

---

### Step 4: Fill Template (20 min)

Copy `template.md` to `docs/plan/week-X-plan.md` and fill in:

1. Week overview (current state → target state)
2. Week objectives (P0, P1, P2)
3. Daily breakdown (5 days)
4. Success metrics
5. Known risks

---

## Key Rules

- **Don't overload:** 3-4 days of solid work + 1 day for buffer/testing
- **Be realistic:** Use velocity from previous week
- **Make it testable:** Each day should have something you can verify
- **Document decisions:** Write why you're doing this (not just what)

---

## Template to Use

→ Copy and use: [template.md](./template.md)

---

## Team Alignment Meeting

After creating the plan:

**Time:** Monday 10 AM (1 hour)
**Attendees:** Whole team
**Agenda:**
1. Explain week goal (5 min)
2. Review daily breakdown (10 min)
3. Discuss risks/blockers (10 min)
4. Q&A (15 min)
5. Confirm everyone understands (5 min)

**Outcome:** Team knows what to do, no questions

---

## Checklist Before Calling It Done

- [ ] All 5 days have clear goals
- [ ] Time estimates are realistic (total ~35-40 hours)
- [ ] P0 objectives are clear
- [ ] Team has reviewed and approved
- [ ] Known risks documented
- [ ] Ready to create Day 1 plan

---

## Next Step

Go to [Workflow 3: Daily Planning](../03-daily-planning/)

Create `day-1-plan.md` right after team alignment.
