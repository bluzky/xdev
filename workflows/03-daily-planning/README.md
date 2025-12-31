# Workflow 3: Daily Planning

**Duration:** 15-30 minutes
**When:** Every morning, 9 AM
**Output:** `docs/plan/week-X/day-Y-plan.md`

---

## What to Do

Create a detailed plan before starting work. This is your contract with the PM.

### Step 1: Review Context (5 min)

- [ ] Read this week's plan (week-X-plan.md)
- [ ] Find the day's goal and deliverable
- [ ] Check if any blockers from yesterday

---

### Step 2: Define What "Done" Means (5 min)

Write specific, testable criteria:

✅ Good:
- [ ] User can click "Record" button and recording starts
- [ ] Recording stops when clicking stop button
- [ ] Video file saved to disk
- [ ] All tests pass
- [ ] Build: 0 errors

❌ Bad:
- [ ] Recording feature works
- [ ] No errors
- [ ] Tests pass

---

### Step 3: Break Into 3-4 Tasks (10 min)

For each task, write:
- **What:** What needs to be built
- **Why:** Why it matters
- **Acceptance:** How to test it

Example:
```
TASK 1: Build recording UI
  What: Create buttons (Record, Stop, Pause)
  Why: User needs interface to control recording
  Acceptance:
    - Buttons render correctly
    - Buttons are clickable
    - Status text updates

TASK 2: Implement basic recording logic
  What: Start/stop recording, save file
  Why: Core functionality
  Acceptance:
    - Recording starts when button clicked
    - File saved with correct name
    - No errors in logs

TASK 3: Test & verify
  What: Manual testing, unit tests, integration
  Why: Ensure quality before PM review
  Acceptance:
    - All manual scenarios pass
    - All unit tests pass
    - No console errors
```

---

### Step 4: Fill Template (10 min)

Copy `template.md` to `docs/plan/week-X/day-Y-plan.md` and fill in:

1. Definition of Done (specific, testable)
2. Tasks (3-4 max)
3. Testing strategy
4. Estimated time per task

---

## Key Rules

- **Be specific:** Every criterion should be testable
- **Be realistic:** 3-4 tasks per day, not 10
- **Be honest:** If you're not sure, write that down as a risk
- **Include testing:** Last task should always be testing/verification

---

## Template to Use

→ Copy and use: [template.md](./template.md)

---

## Before Starting Work

After creating the plan:
1. **9:30 AM:** Review plan once more
2. **9:30 AM:** Team confirms understanding (2 min quick sync)
3. **10:00 AM:** Start work

---

## During the Day

Keep the plan visible:
- Check it regularly
- Update if blockers arise
- Log time spent
- Add notes to execution section

---

## Checklist Before Calling It Done

- [ ] Definition of Done is specific and testable
- [ ] 3-4 clear tasks (not 10+)
- [ ] Each task has "What, Why, Acceptance"
- [ ] Testing strategy is clear
- [ ] Time estimates are realistic (total ~6-8 hours)
- [ ] You understand what success looks like

---

## Next Step

Go to [Workflow 4: Daily Tracking](../04-daily-tracking/)

During the day, log progress and results.
