# AI Prompt: Daily Tracking (Workflow 4)

**When to use this:** Throughout day (5 min updates) + 5 PM (10 min summary)
**Output files:** `docs/plan/week-X/day-Y-plan.md` execution section + `docs/plan/week-X/progress.md`

---

## Your Task

Populate execution sections of `day-Y-plan.md` and update `progress.md` with actual work results as the day progresses.

---

## Input You'll Receive

The human will provide:

**At 5 PM:**
```
CURRENT STATE:
- Which day (Day Y, Week X)
- Day plan that was created (day-Y-plan.md)
- Work accomplished during day
- Tasks completed/incomplete
- Blockers encountered
- Test results
- Build quality

TIME TRACKING:
- Start time
- End time
- How long each task took (or estimates)
- Breaks taken (if any)

QUALITY DATA:
- Build status (errors, warnings)
- Test pass rate
- Manual testing results
- Any console errors
```

---

## What to Generate

**In day-Y-plan.md execution section, fill:**

1. **Progress Log** (timestamps of work)
   - [HH:MM] — Milestone or blocker
   - [HH:MM] — Progress update

2. **Completion Section**
   - Actual time spent (vs estimate)
   - Tasks completed (checkboxes)
   - Blockers encountered
   - Quality results (tests, build)
   - Key learnings

3. **PM Verification Section**
   - Status (Approved / Needs Revision / Pending)
   - PM feedback/notes

**In progress.md, add:**

- Daily status section for the day
- Completed tasks
- Actual time (vs estimate)
- Blockers
- Quality metrics
- PM sign-off status

---

## Input Format

Human will provide info like:

```
DAY SUMMARY

Day: Day 1, Week 2
Time: 9:00 AM - 5:00 PM (8 hours available, 1 hour lunch)
Work completed:
  - Task 1: Recording buttons (COMPLETE) - 2.5 hours actual
  - Task 2: Status display (COMPLETE) - 2 hours actual
  - Task 3: Layout (COMPLETE) - 1.5 hours actual
  - Task 4: Testing (COMPLETE) - 1 hour actual

Quality:
  - Build: 0 errors, 0 warnings ✅
  - Tests: 100% passing (12/12)
  - Manual testing: All scenarios pass

Blockers: None

PM Review: 4:30 PM - Approved, "Great work"

Learnings:
  - SwiftUI preview faster than expected
  - Button sizing constraints tricky
```

---

## Generation Steps

1. **Calculate actual time:**
   - Sum actual hours from all tasks
   - Compare to estimate
   - Note variance and reason

2. **Populate execution log:**
   - Add timestamps of key milestones
   - Note blockers when they occurred
   - Track progress throughout day

3. **Verify quality:**
   - Check build status (0 errors target)
   - Check test pass rate (100% target)
   - Check manual verification results
   - Note any warnings

4. **Document learnings:**
   - What went well?
   - What was harder than expected?
   - Any process insights?

5. **Update both files:**
   - day-Y-plan.md execution section (detailed)
   - progress.md daily section (summary)

---

## Output Format: Day Plan Execution Section

```markdown
## EXECUTION NOTES

### Progress Log

**Start:** [HH:MM]

**[HH:MM]** — [Milestone: "Task 1 started"]
**[HH:MM]** — [Progress: "Task 1 buttons rendering, moving to styling"]
**[HH:MM]** — [Milestone: "Task 1 complete"]
**[HH:MM]** — [Progress: "Task 2 underway, status display layout"]
**[HH:MM]** — [Challenge: "Button tap detection required event handling, fixed"]
**[HH:MM]** — [Milestone: "Task 4 testing complete"]

**Complete:** [HH:MM]

---

### Completion

**Actual Time Spent:** ~X hours (estimated: ~X hours)

**Variance Reason:** [Why actual differs, if significant]

**Tasks Completed:**
- [x] Task 1
- [x] Task 2
- [x] Task 3
- [x] Task 4

**Blockers Encountered:**
- [x] Fixed: [Blocker description and resolution]
- None

**Quality Results:**
- ✅ Build Status: Clean (0 errors, 0 warnings)
- ✅ Test Pass Rate: 100% (12 tests)
- ✅ Manual Testing: All scenarios pass

---

### Key Learnings

- [Learning 1 about technical approach]
- [Process improvement identified]

---

### Notes for Next Day

- [Handoff: what next developer should know]
- [Follow-up if not completed]

---

## PM VERIFICATION

**PM Reviewed:** [Date/Time]
**PM Notes:** [Feedback from PM]
**Status:** ✅ Approved / 🔄 Needs Revision / ⏳ Pending

**PM Sign-off Date:** [Date]

---

**Day Status:** ✅ Complete
```

---

## Output Format: Progress.md Daily Section

```markdown
## Day Y (Day-Name, Date)

**Status:** ✅ Complete / 🔄 In Progress

**Plan:** [Brief description from week plan]

**Completed:**
- [x] Task 1: [Outcome]
- [x] Task 2: [Outcome]
- [x] Task 3: [Outcome]
- [x] Task 4: [Outcome]

**Actual Time:** ~X hours (estimated: ~X hours)

**Blockers:** None / [Brief description]

**Quality:**
- ✅ Build: 0 errors, 0 warnings
- ✅ Tests: 100% passing (X tests)
- ✅ Manual: All scenarios pass

**Notes:** [Any learnings or blockers to carry forward]

**PM Sign-Off:** ✅ Approved

---
```

---

## Quality Checklist

When populating execution sections, verify:
- [ ] All timestamps are reasonable (chronological)
- [ ] Actual hours are tracked
- [ ] Variance from estimate is noted
- [ ] Build status is 0 errors, 0 warnings
- [ ] Test pass rate is 100% (with count)
- [ ] Blockers are documented
- [ ] Key learnings captured
- [ ] PM sign-off obtained
- [ ] Tasks marked complete/incomplete accurately

---

## Example: Complete Day Execution

**Human input:**
```
DAY COMPLETION

Day: Day 1, Week 2
Date: Jan 6, 2025

TIMELINE:
9:00 AM - Started
11:30 AM - Task 1 complete (2.5 hours)
1:30 PM - Task 2 complete (2 hours)
3:00 PM - Task 3 complete (1.5 hours)
4:00 PM - Task 4 testing complete (1 hour)
4:30 PM - PM review
5:00 PM - Done

QUALITY:
- Build: 0 errors, 0 warnings
- Tests: 12/12 passing
- Manual: All scenarios verified
- No console warnings

LEARNINGS:
- Preview canvas was really helpful
- Button constraints took longer than expected
- Time estimates were good

PM FEEDBACK: "Looks great, all UI matches design"
```

**AI should generate:**

day-Y-plan.md execution section:
```markdown
## EXECUTION NOTES

### Progress Log

**Start:** 9:00 AM

**[9:00 AM]** — Day 1 started, reviewing mockups and requirements
**[9:15 AM]** — Task 1: Recording buttons - started implementation
**[11:15 AM]** — Completed button rendering and styling
**[11:30 AM]** — Task 1 complete, all buttons displaying correctly
**[11:45 AM]** — Task 2: Status display - started layout design
**[1:30 PM]** — Task 2 complete, status text updates on mock events
**[2:00 PM]** — Task 3: Layout arrangement - started organizing UI elements
**[2:30 PM]** — Encountered button constraint issue, fixed with proper spacing
**[3:00 PM]** — Task 3 complete, full layout matches design mockup
**[3:15 PM]** — Task 4: Testing started, writing unit tests
**[4:00 PM]** — All tests passing (12/12), manual testing complete
**[4:30 PM]** — PM review session started

**Complete:** 5:00 PM

---

### Completion

**Actual Time Spent:** ~7 hours (estimated: ~7 hours) ✅ On estimate

**Variance Reason:** None - estimate was accurate

**Tasks Completed:**
- [x] Task 1: Recording buttons rendering and styled
- [x] Task 2: Status display with mock updates
- [x] Task 3: Layout arrangement matching mockup
- [x] Task 4: Testing and quality verification

**Blockers Encountered:**
- [x] Fixed: Button constraint spacing required adjustment, resolved with 8pt grid

**Quality Results:**
- ✅ Build Status: Clean (0 errors, 0 warnings)
- ✅ Test Pass Rate: 100% (12/12 tests passing)
- ✅ Manual Testing: All 3 scenarios verified on device

---

### Key Learnings

- SwiftUI preview canvas was extremely helpful for iterative design
- Button sizing constraints were more complex than initially estimated (worked out)
- Time estimates were accurate for this type of work - good baseline for future UI tasks
- Starting with mockup review saved time during implementation

---

### Notes for Next Day

- All UI elements complete and tested
- Ready to implement button state logic on Day 2
- No architectural changes needed
- Button styling can be reused for other controls

---

## PM VERIFICATION

**PM Reviewed:** 4:30 PM, Jan 6, 2025

**PM Notes:** "Excellent work! All UI elements match the design perfectly. Responsive layout works great on both iPhone and iPad. No issues, ready for logic implementation tomorrow."

**Status:** ✅ Approved

**PM Sign-off Date:** Jan 6, 2025

---

**Day Status:** ✅ Complete
```

progress.md entry:
```markdown
## Day 1 (Monday, Jan 6)

**Status:** ✅ Complete

**Plan:** Recording UI setup - implement all buttons and status display

**Completed:**
- [x] Recording control buttons (Record, Stop, Pause)
- [x] Status display area with state text
- [x] Overall layout and spacing
- [x] Unit tests (12 tests, all passing)
- [x] Manual verification on device

**Actual Time:** ~7 hours (estimated: ~7 hours) ✅

**Blockers:** None

**Quality:**
- ✅ Build: 0 errors, 0 warnings
- ✅ Tests: 100% passing (12/12)
- ✅ Manual: All scenarios pass

**Notes:** Time estimates accurate, all deliverables met, ready for Day 2 logic implementation

**PM Sign-Off:** ✅ Approved by PM at 4:30 PM

---
```

---

## When to Ask for Clarification

Ask the human if:
- ❓ "What was actually accomplished?" (need specifics)
- ❓ "How long did each task take?" (need time tracking)
- ❓ "What were the blockers?" (any issues?)
- ❓ "Did tests pass?" (need quality data)
- ❓ "Did PM review? What feedback?" (need sign-off)

---

## Tips

✅ **DO:**
- Log progress in real-time (every 1-2 hours)
- Track actual vs estimated time
- Document blockers immediately
- Record test results accurately
- Capture learnings for future
- Get PM sign-off before marking day complete

❌ **DON'T:**
- Leave execution section empty
- Guess at actual time (track it)
- Skip blocker documentation
- Ignore test failures
- Forget PM review
- Make learnings vague

---

## Key Rules

**Build Quality Non-Negotiable:**
- Must be: 0 errors, 0 warnings
- If not met: Day is not complete

**Test Pass Rate Non-Negotiable:**
- Must be: 100%
- If not met: Day is not complete

**PM Sign-off Non-Negotiable:**
- Must have: Approved status
- If not: Day is pending, can't move to next day

**Time Tracking Non-Negotiable:**
- Must log: Actual vs estimated
- Use this data to improve estimates

---

## Files to Reference

- **Template:** `workflows/04-daily-tracking/template.md`
- **Instructions:** `workflows/04-daily-tracking/README.md`
- **Day plan:** `docs/plan/week-X/day-Y-plan.md`
- **Progress log:** `docs/plan/week-X/progress.md`
