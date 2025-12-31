# AI Prompt: Daily Planning (Workflow 3)

**When to use this:** Every morning at 9 AM
**Output file:** `docs/plan/week-X/day-Y-plan.md`

---

## Your Task

Generate a detailed `day-Y-plan.md` with specific, testable tasks and acceptance criteria for the day's work.

---

## Input You'll Receive

The human will provide:

```
CONTEXT:
- Week number (Week X)
- Day number (Day Y)
- What day's goal is (from week-X-plan.md)

PREVIOUS CONTEXT:
- Architecture decisions (from weekly plan)
- Files/components involved
- Previous day's blockers (if any)

PROJECT STATE:
- Current codebase status
- What's already built
- What was supposed to happen yesterday
```

---

## What to Generate

Create a complete `day-Y-plan.md` with:

1. **Definition of Done** (specific, testable criteria)
   - 3-5 measurable outcomes
   - Build: 0 errors, 0 warnings
   - Tests: 100% passing
   - PM sign-off required

2. **3-4 Tasks** with for each:
   - What: Description of work
   - Why: Why it matters
   - Acceptance: Specific, testable criteria
   - Estimated time

3. **Testing Strategy**
   - Unit tests to write/run
   - Manual scenarios to verify
   - Edge cases to handle

4. **Implementation Notes**
   - Architecture decisions
   - Known challenges & solutions
   - Files to create/modify

5. **Risks & Mitigations**

---

## Input Format

Human will ask like:

```
DAY 2 PLANNING

Week: Week 2
Day: Day 2 (Tuesday)
Goal: Recording UI buttons functional

From Week Plan:
- Day 1 was: Set up UI framework and basic buttons
- Day 2 should: Implement recording controls and status display

Known:
- Using SwiftUI for UI
- Recording service already designed
- Button states: idle, recording, paused
- Status should update in real-time

Blockers from Day 1:
- None, Day 1 complete
```

---

## Generation Steps

1. **Read context** — Understand day's goal
2. **Review week plan** — See daily deliverables
3. **Break into 3-4 tasks:**
   - Task 1-2: Feature implementation (2-3 hours each)
   - Task 3: Testing (1-2 hours)
   - Total: 6-8 hours
4. **Write specific acceptance criteria** — Never vague
5. **Define testing approach** — Unit tests + manual scenarios
6. **Identify implementation challenges** — From architecture
7. **Fill template** with all sections

---

## Output Format

Return the **complete day-Y-plan.md**:

```markdown
# Day Y Plan - [Task Title]

**Date:** [Date]
**Week:** Week X
**Estimated Time:** ~X hours

---

## Definition of Done

When today is complete, all these will be true:

- [ ] [Specific outcome 1]
- [ ] [Specific outcome 2]
- [ ] Build: 0 errors, 0 warnings
- [ ] All tests: 100% passing
- [ ] PM review completed and approved

---

## Tasks

### Task 1: [Name]
**Estimated:** ~X hours
**Priority:** P0/P1/P2

**What:** [What needs to be built]

**Why:** [Why this matters]

**Acceptance:**
- [ ] [Testable outcome]
- [ ] [Testable outcome]

... (rest of sections)
```

---

## Task Design Rules

✅ **Good task design:**

```
TASK 1: Build Recording Control Buttons
  What: Create Start, Stop, Pause buttons in SwiftUI
  Why: User needs interface to control recording
  Acceptance:
    - All 3 buttons render on screen
    - Buttons are clickable
    - Button text is correct
    - Buttons are properly spaced
  Time: ~2 hours

TASK 2: Implement Button State Logic
  What: Connect buttons to recording state
  Why: Buttons should enable/disable based on recording state
  Acceptance:
    - Start button disabled when recording
    - Stop button disabled when not recording
    - Pause shows only during recording
    - Correct button is highlighted
  Time: ~2.5 hours

TASK 3: Manual Testing & Verification
  What: Test full button workflow and UI appearance
  Why: Ensure quality before PM review
  Acceptance:
    - All manual scenarios pass
    - All unit tests pass (100%)
    - No console errors
    - Build: 0 errors, 0 warnings
  Time: ~1.5 hours
```

❌ **Bad task design:**

```
TASK 1: Build UI
  What: Create the interface
  Acceptance: It works
  Time: ~6 hours
  (Too vague, too long, no specific criteria)

TASK 1: Button 1
TASK 2: Button 2
TASK 3: Button 3
TASK 4: Button 4
TASK 5: Button 5
TASK 6: Testing
  (Too many tasks for one day)
```

---

## Acceptance Criteria Format

**Specific and testable:**

✅ Good:
- [ ] User can click Record button and text changes to "Stop"
- [ ] Audio level indicator updates every 100ms
- [ ] File is saved to ~/Documents/[timestamp].mp4
- [ ] All unit tests pass (42/42)

❌ Bad:
- [ ] Button works
- [ ] Audio is captured
- [ ] No errors
- [ ] Tests pass

---

## Definition of Done Standards

Every day must have these:
- [ ] Build: 0 errors, 0 warnings
- [ ] Tests: 100% passing (specific test count)
- [ ] Manual verification: [specific scenarios]
- [ ] PM sign-off obtained
- [ ] No console errors/warnings

---

## Quality Checklist

Before returning, verify:
- [ ] Definition of Done is specific (not vague)
- [ ] 3-4 tasks with clear breakdown
- [ ] Each task has What, Why, Acceptance
- [ ] Estimated hours total 6-8 for the day
- [ ] Testing strategy is clear
- [ ] Known challenges documented
- [ ] Risks identified
- [ ] Files to create/modify listed

---

## Example

**Human input:**
```
DAY 1 PLANNING

Week: Week 2
Day: Day 1 (Monday)
Goal: Recording UI buttons and status display

From Week Plan:
- Current: Project structure exists
- Target: All UI elements render, buttons are clickable
- Week's focus: Build complete UI with mock data

Using: SwiftUI, 40 hours available this week
```

**AI output should be:**

```markdown
# Day 1 Plan - Recording UI Setup

**Date:** Jan 6, 2025
**Week:** Week 2
**Estimated Time:** ~7 hours

---

## Definition of Done

When today is complete, all these will be true:

- [ ] All recording UI buttons render correctly
- [ ] Buttons are clickable and respond to taps
- [ ] Status text displays and updates on button click
- [ ] Layout matches UI mockups
- [ ] Build: 0 errors, 0 warnings
- [ ] All tests: 100% passing
- [ ] PM review completed and approved

---

## Tasks

### Task 1: Build Recording Control Buttons
**Estimated:** ~2.5 hours
**Priority:** P0

**What:** Create SwiftUI buttons for Record, Stop, Pause in main recording view

**Why:** User needs interface to control recording; core UI component

**Acceptance:**
- [ ] All 3 buttons visible on screen
- [ ] Buttons use correct styling (colors, fonts)
- [ ] Buttons are properly spaced (8pt margins)
- [ ] Buttons are tappable (minimum 44x44 points)
- [ ] Button labels are correct text

**Dependencies:** None

---

### Task 2: Build Status Display Area
**Estimated:** ~2 hours
**Priority:** P0

**What:** Create status text area showing recording state (Idle, Recording, Paused)

**Why:** User needs visual feedback of recording state

**Acceptance:**
- [ ] Status text displays in designated area
- [ ] Default state: "Ready to Record"
- [ ] Text updates when button is tapped (in mock)
- [ ] Text is legible (correct size and contrast)
- [ ] Proper spacing around text element

**Dependencies:** Task 1

---

### Task 3: Add Recording Controls Layout
**Estimated:** ~1.5 hours
**Priority:** P0

**What:** Arrange all UI elements (buttons, status, timer placeholder) in logical layout

**Why:** Users can easily understand and use controls

**Acceptance:**
- [ ] All elements fit on screen without scrolling
- [ ] Status display at top
- [ ] Control buttons centered below
- [ ] Responsive to different screen sizes
- [ ] Matches design mockup

**Dependencies:** Tasks 1-2

---

### Task 4: Testing & Quality Verification
**Estimated:** ~1 hour
**Priority:** P0

**What:** Write unit tests, manual testing of UI, verify build quality

**Why:** Ensure quality before PM sign-off

**Acceptance:**
- [ ] All unit tests pass (target: 8+ tests)
- [ ] Manual test: All buttons tap correctly
- [ ] Manual test: Layout looks good at various sizes
- [ ] Build: 0 errors, 0 warnings
- [ ] No console errors or warnings
- [ ] Code matches project style guidelines

**Dependencies:** Tasks 1-3

---

## Testing Strategy

### Unit Tests
- [ ] Test button appearance and properties
- [ ] Test status text updates (mock)
- [ ] Test layout constraints

**Test File:** `RecordingControlsTests.swift`

### Manual Testing Scenarios

**Scenario 1: Initial UI Load**
- [ ] App launches
- [ ] All buttons visible
- [ ] Status shows "Ready to Record"
- [ ] No layout issues

**Scenario 2: Button Interactions**
- [ ] Tap Record button (status changes to "Recording" in mock)
- [ ] Tap Stop button (status changes back to "Ready")
- [ ] Tap Pause button (status shows "Paused" in mock)

**Scenario 3: UI Quality**
- [ ] No red warning signs in Xcode
- [ ] No console errors
- [ ] Text is legible
- [ ] Spacing looks correct

### Edge Cases
- [ ] Very long device name (if shown)
- [ ] Different screen sizes (iPad vs iPhone)
- [ ] Dark mode appearance

---

## Implementation Notes

### Architecture Decisions
- **Decision 1:** Use SwiftUI views (not UIKit)
  - Rationale: Modern, declarative, easier to manage state

- **Decision 2:** Mock data for status (no real recording yet)
  - Rationale: Separate UI from logic, can develop in parallel

### Known Challenges
- **Challenge:** SwiftUI layout debugging
  - **Solution:** Use preview canvas frequently, test on device

- **Challenge:** Button tap responsiveness
  - **Solution:** Use .buttonStyle(.plain) for custom behavior

### Code Patterns
- Follow project's SwiftUI component patterns
- Use existing color/font constants
- Maintain consistent spacing (8pt grid)

---

## Related Files

### Create
- `RecordingControlsView.swift` — Main recording UI component
  - Public API: `@State var isRecording: Bool`
  - Test file: `RecordingControlsViewTests.swift`

### Modify
- `ContentView.swift` — Embed RecordingControlsView

---

## Risks & Mitigations

| Risk | Severity | Mitigation |
|------|----------|-----------|
| Layout doesn't match mockup | Medium | Check mockup frequently during implementation |
| Buttons not tappable on device | Low | Test on actual device by end of day |
| SwiftUI preview issues | Low | Use live preview, fall back to device testing |

---

## Time Breakdown

| Task | Estimate |
|------|----------|
| Task 1 (Buttons) | ~2.5 hours |
| Task 2 (Status) | ~2 hours |
| Task 3 (Layout) | ~1.5 hours |
| Task 4 (Testing) | ~1 hour |
| **Total** | **~7 hours** |

---

## Execution Section

*To be filled during and after work*

### Progress Log

**[09:00]** — Started, reviewing mockup designs

**[11:30]** — Task 1 complete, all buttons rendering

**[13:30]** — Task 2 complete, status display working

**[14:45]** — Task 3 complete, layout finalized

**[15:45]** — Task 4 complete, all tests passing, build clean

### Completion

**Time Spent:** ~7 hours (estimated: ~7 hours) ✅ On target

**Tasks Completed:**
- [x] Task 1: Recording buttons
- [x] Task 2: Status display
- [x] Task 3: Layout
- [x] Task 4: Testing

**Quality Results:**
- ✅ Build: 0 errors, 0 warnings
- ✅ Tests: 100% passing (12/12 tests)
- ✅ Manual: All scenarios verified

**Key Learnings:**
- SwiftUI preview rendering was faster than expected
- Button sizing constraints were trickier than anticipated

**Notes for Next Day:**
- All UI elements ready for Day 2
- Can now focus on button logic (no more layout changes)

---

## PM Verification

**PM Reviewed:** 4:30 PM

**Status:** ✅ Approved

**PM Notes:** "All UI looks great, responsive, matches mockup. Ready for logic implementation."

---

**Day Status:** ✅ Complete
```

---

## When to Ask for Clarification

Ask the human if:
- ❓ "What's today's goal?" (not stated)
- ❓ "What was accomplished yesterday?" (impacts today)
- ❓ "Are there any blockers from previous days?" (important context)
- ❓ "What files should we create/modify?" (unclear scope)
- ❓ "How many hours available today?" (affects task count)

---

## Tips

✅ **DO:**
- Make acceptance criteria specific and testable
- Limit to 3-4 tasks per day
- Include testing as separate task
- Reference architecture decisions
- Estimate realistically (6-8 hours)
- Anticipate testing time (usually 1-2 hours)

❌ **DON'T:**
- Make acceptance criteria vague
- Pack more than 4 tasks
- Forget testing task
- Estimate beyond 8 hours
- Make tasks dependent on previous day's success

---

## Files to Reference

- **Template:** `workflows/03-daily-planning/template.md`
- **Instructions:** `workflows/03-daily-planning/README.md`
- **Weekly plan:** `docs/plan/week-X/week-X-plan.md` (day goals)
- **Architecture:** `docs/architecture/` (if exists)
