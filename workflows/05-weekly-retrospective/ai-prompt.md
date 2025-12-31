# AI Prompt: Weekly Retrospective (Workflow 5)

**When to use this:** Friday 4:30 PM
**Output files:** `docs/plan/week-X/summary.md` + updated `docs/plan/master-progress.md`

---

## Your Task

Generate a comprehensive `summary.md` that analyzes the week's work, captures learnings, and identifies improvements for next week.

---

## Input You'll Receive

The human will provide:

```
WEEK DATA:
- Week number (Week X)
- Phase (from master-plan.md)

DAILY RESULTS:
- All 5 day-Y-plan.md files with execution sections
- progress.md with all daily entries

METRICS:
- Total hours estimated vs actual
- Test pass rates per day
- Build quality (errors/warnings)
- Blockers encountered
- P0/P1/P2 objectives completed

TEAM FEEDBACK:
- What went well (retrospective discussion)
- What was harder than expected
- Surprises or discoveries
- Ideas for improvement
```

---

## What to Generate

Create a complete `summary.md` with:

1. **What Got Done**
   - P0 objectives completed (✓/✗)
   - Additional achievements
   - Deliverables shipped

2. **Metrics**
   - Hours estimated vs actual
   - Test pass rate
   - Build quality (0 errors target)
   - Blockers and resolutions

3. **Team Reflections**
   - What went well
   - What was harder than expected
   - Surprises
   - Technical learnings
   - Process learnings

4. **Quality Assessment**
   - Code quality observations
   - Technical debt (if any)
   - Performance notes

5. **Adjustments for Next Week**
   - Estimation adjustments
   - Process improvements
   - Scope changes
   - Approach changes

6. **Grade & Overall Assessment**

---

## Input Format

Human will ask like:

```
WEEK 2 RETROSPECTIVE

Phase: Phase 2 - Frontend Build
Date: Jan 6-10, 2025

WEEK RESULTS:
Completed:
  - Recording UI buttons (all 3): DONE
  - Status display: DONE
  - Layout polish: DONE
  - Unit testing: DONE (12/12 tests pass)

Metrics:
  - Estimated: 40 hours
  - Actual: 38 hours (2 hours ahead)
  - Build: 0 errors, 0 warnings (all days)
  - Tests: 100% pass rate (all days)
  - Blockers: 1 (button constraints, fixed same day)

P0 Objectives:
  - Recording UI functional: ✅
  - Status display: ✅
  - Layout complete: ✅
  - Tests passing: ✅

Team Notes from Retrospective:
What went well:
  - Design mockups were clear
  - Time estimates were accurate
  - Team stayed focused

What was harder:
  - SwiftUI constraints more complex than expected
  - Device testing revealed layout issues on iPad

Surprises:
  - Preview canvas was really helpful
  - Could have done more work if we had more time

Process observations:
  - Daily planning is really effective
  - PM reviews help catch issues early
```

---

## Generation Steps

1. **Analyze week data:**
   - Sum hours estimated vs actual
   - Calculate velocity
   - Check quality metrics

2. **Review daily files:**
   - Extract learnings from each day
   - Note patterns in blockers
   - Identify what worked well

3. **Assess quality:**
   - Build status across all days
   - Test pass rates
   - Code quality patterns

4. **Create reflections section:**
   - What went well (specific examples)
   - What was harder (with explanations)
   - Surprises and insights
   - Learnings (technical and process)

5. **Identify improvements:**
   - Estimation adjustments
   - Process changes
   - Scope adjustments for next week
   - New approaches to try

6. **Grade the week:**
   - Overall assessment
   - Key successes
   - Areas for improvement

7. **Prepare for next week:**
   - Preview of upcoming week
   - Recommendations based on learnings

---

## Output Format

Return the **complete summary.md**:

```markdown
# Week X Summary

**Week:** Week X (Mon-Fri)
**Phase:** Phase X - [Name]
**Team:** [Names]

---

## What Got Done

### P0 Objectives (Required)
- [x] [Objective 1 — COMPLETE]
- [x] [Objective 2 — COMPLETE]
- [ ] [Objective 3 — Not completed, reason: X]

### Additional Achievements
- [Achievement not in plan but valuable]

### Did NOT Get Done
- [ ] [P1 objective — moving to Week X+1]

**Reason:** [Why not enough time / blocked / deprioritized]

---

## Metrics

| Metric | Target | Actual | Notes |
|--------|--------|--------|-------|
| Estimated Hours | 40 | — | |
| Actual Hours | 40 | — | [Faster/slower] |
| Variance | 0% | — | |
| Test Pass Rate | 100% | — | |
| Build Quality | 0 errors | — | |

... (rest of sections)
```

---

## Metrics Analysis

**Calculate and include:**

- **Velocity:** Total hours actual vs estimated
  - "Estimated 40, actual 38 = 5% ahead"
  - Use this to adjust next week's scope

- **Quality Trend:** Are errors/warnings decreasing?
  - "5 warnings Day 1 → 0 warnings Day 5"
  - Shows improving quality discipline

- **Test Coverage:** Did test pass rate improve?
  - "100% all days = consistent quality"
  - "95% → 100% improvement" = good

- **Blocker Velocity:** How many blockers per day?
  - "1 blocker Day 2, resolved same day"
  - Shows good problem-solving

---

## Team Reflections Section

**Good reflections (specific):**
```
What Went Well:
- UI mockups were very detailed and clear
  Why: Team didn't have to guess at spacing/colors
  Impact: Saved 2-3 hours of rework

- Time estimates were within 5% of actual
  Why: Daily planning broke work into small chunks
  Impact: Can trust estimates for future weeks

- PM reviews caught alignment issues early
  Why: PM reviewed every day, not just Friday
  Impact: No major rework needed
```

**Bad reflections (vague):**
```
What Went Well:
- Good teamwork
- Great communication
- Nice progress
(Too vague, not actionable)
```

---

## Quality Assessment

Analyze code quality:
- Build status (0 errors trend)
- Test pass rates
- Code organization
- Architecture decisions working well
- Any technical debt incurred
- Performance observations

Example:
```
Build Quality:
- Achieved 0 errors, 0 warnings all 5 days
- Consistent discipline with code review
- No quality regressions

Code Quality:
- Components are well-organized
- Tests are comprehensive (12 tests for UI)
- SwiftUI patterns are clean
- No technical debt

Performance:
- Preview canvas renders instantly
- App launch time < 1 second
- No memory issues noted
```

---

## Adjustments for Next Week

Based on learnings, identify:

**Estimation Adjustments:**
```
If actual faster than estimated:
- Increase scope next week
- Add complexity
- Don't increase hours

If actual slower:
- Reduce scope
- Move P1 to next week
- Keep same hours
- Add buffer for research
```

**Process Improvements:**
```
- Change to daily planning? (keep as is)
- Change to PM review timing? (Friday 4:30 PM is good)
- Need more specification? (mockups were clear)
- Need different tools? (SwiftUI is working well)
```

**Scope Changes:**
```
- Promote P1 items if ahead of schedule
- Demote P0 if behind schedule
- Add complexity if velocity allows
- Simplify if velocity lower than expected
```

---

## Grade the Week

Assess overall performance:

**Example:**
```
Grade: ⭐⭐⭐⭐ (4/5 stars)

Reasoning:
✅ All P0 objectives completed on time
✅ Quality metrics all green (0 errors, 100% tests)
✅ Team velocity reliable (2 hours ahead)
✅ No major blockers or rework needed

Areas for improvement:
🔄 iPad layout needed Day 5 fixes
🔄 Could have started with more aggressive schedule
```

---

## Quality Checklist

Before returning, verify:
- [ ] All P0 objectives marked complete/incomplete
- [ ] Metrics calculated (hours, quality, tests)
- [ ] Blockers documented with resolutions
- [ ] Team reflections are specific (not vague)
- [ ] Adjustments for next week identified
- [ ] Grade assigned with reasoning
- [ ] Preview of next week included
- [ ] No incomplete sections

---

## Example: Complete Summary

**Human input:**
```
WEEK 2 SUMMARY

Dates: Jan 6-10, 2025
Phase: Phase 2 - Frontend
Team: Solo developer

RESULTS:
- All UI buttons complete
- Status display working
- Layout responsive
- 12/12 tests passing
- 0 build errors all 5 days

Time: Estimated 40 hours, Actual 38 hours

Blockers:
- Day 2: Button constraints (fixed same day)
- Day 4: iPad layout issues (fixed Day 5)

Retrospective feedback:
- Mockups were clear and helpful
- Preview canvas saved time
- Device testing important (found iPad issue)
- Estimates were accurate
- PM reviews worked great
```

**AI should generate:**

```markdown
# Week 2 Summary - Frontend Build

**Week:** Week 2 (Jan 6-10, 2025)
**Phase:** Phase 2 - Frontend Build
**Team:** Solo developer

---

## What Got Done

### P0 Objectives (Required) ✅
- [x] Recording control buttons (Record, Stop, Pause)
- [x] Status display with state updates
- [x] Responsive layout for iPhone and iPad
- [x] Comprehensive unit tests (all passing)

### Additional Achievements
- Responsive layout works perfectly on multiple screen sizes
- Button interaction logic mockup complete and ready for Day 6
- Device testing revealed and fixed iPad layout issues
- Clear patterns established for future UI components

### Did NOT Get Done
None - all P0 objectives completed.

**Other items:**
- [ ] P1: Keyboard shortcuts (moved to Week 3)
- [ ] P2: Settings panel (moved to Week 4)

---

## Metrics

| Metric | Target | Actual | Status |
|--------|--------|--------|--------|
| Estimated Hours | 40 | — | |
| Actual Hours | 40 | 38 | ✅ 5% ahead |
| Variance | 0% | -5% | ✅ Favorable |
| Test Pass Rate | 100% | 100% | ✅ All days |
| Build Quality | 0 errors | 0 errors | ✅ Consistent |
| Build Warnings | 0 | 0 | ✅ None |
| P0 Completion | 100% | 100% | ✅ Complete |

---

## Team Reflections

### What Went Well

**Clear Design Mockups**
- Why: Mockups were detailed with spacing, colors, typography
- Impact: No ambiguity during implementation, saved 2-3 hours rework
- Lesson: Detailed mockups before coding saves time

**Accurate Time Estimates**
- Why: Daily planning broke work into specific tasks
- Impact: All 5 days within 10% of estimate
- Lesson: Small task breakdown improves estimation accuracy

**Daily PM Reviews**
- Why: PM reviewed each day at 4:30 PM, not Friday
- Impact: iPad layout issue caught Day 4, fixed Day 5 (not at end)
- Lesson: Frequent feedback prevents major rework

**SwiftUI Preview Canvas**
- Why: Used live preview during development
- Impact: Caught layout issues instantly
- Lesson: Live preview is faster than device testing for iteration

---

### What Was Harder Than Expected

**SwiftUI Layout Constraints**
- What: Button spacing and alignment required more precision
- Why: Grid-based spacing needed careful constraint setup
- Resolution: Used 8pt grid system, worked well
- Time Impact: Added ~30 minutes to Day 1
- Lesson: Layout constraints need upfront consideration

**iPad Responsiveness**
- What: Layout worked on iPhone but not iPad
- Why: Text sizing and button spacing didn't scale
- Resolution: Added size class handling, tested both devices
- Time Impact: Day 5 focus switched to iPad fixes
- Lesson: Test on all target devices, not just primary

---

### Surprises & Discoveries

**SwiftUI Preview Speed**
- Discovery: Live preview is much faster than device testing for iteration
- Impact: Could iterate designs 5x faster using preview
- Action: Use preview-first approach next week

**Velocity Ahead of Schedule**
- Discovery: 2 hours ahead of estimate for the week
- Impact: Could have added more scope
- Action: Next week, add 1-2 P1 items to challenge team

**Pattern Reuse Opportunity**
- Discovery: Button styling pattern created is reusable
- Impact: Can use same button component for future controls
- Action: Document pattern for Day 6+

---

### Technical Learnings

- SwiftUI layout constraints are powerful but require careful setup
- Grid-based spacing (8pt) maintains consistency better than manual spacing
- View modifiers should be extracted for reusability
- Testing UI components is straightforward with XCTest

### Process Learnings

- Daily planning (15 minutes) is worth it (saves rework)
- Breaking work into small tasks improves estimates
- PM daily reviews catch issues before they compound
- Retrospectives should be specific, not vague

---

## Quality Assessment

**Build Quality:** Excellent
- Achieved 0 errors, 0 warnings all 5 days
- Consistent code review discipline
- No quality degradation
- No technical debt incurred

**Code Quality:** Very Good
- Components well-organized by responsibility
- Tests comprehensive (12 tests, good coverage)
- SwiftUI patterns clean and idiomatic
- Ready for backend integration

**Performance:** Good
- Preview canvas renders instantly
- No performance issues on device
- App launch time excellent
- Memory usage normal

**Areas for Improvement:**
- iPad testing earlier (would have caught layout sooner)
- More aggressive accessibility testing (a11y)

---

## Adjustments for Week 3

### Estimation Adjustments

**Why:** Actual 2 hours ahead of estimate

**Adjustment for Week 3:**
- Add 1-2 additional P1 objectives
- Increase complexity of features
- Same 40-hour estimate (don't increase hours)
- Use learnings from Week 2 to challenge team more

### Process Improvements

**Keep Same:** Daily planning is working great
**Keep Same:** PM reviews at 4:30 PM catching issues
**Improve:** Start iPad testing Day 1 (not Day 5)
**Improve:** Create reusable component library from patterns

### Scope Changes

**For Week 3:**
- Promote button logic implementation (was P1, now P0)
- Add audio state management (was Week 4, now Week 3)
- Keep P2 items for Week 4

### Approach Changes

**Use preview-first approach:**
- Iterate in preview canvas before device
- Save device testing for final verification
- Should save another 1-2 hours

---

## Blockers & Resolutions

| Blocker | Day | Severity | Resolution | Impact |
|---------|-----|----------|-----------|--------|
| Button constraints | Day 2 | Medium | Used grid-based system | +30 min, resolved same day |
| iPad layout issues | Day 4 | Medium | Added size class handling | Day 5 focus, fully resolved |

**Lessons:**
- Blockers resolved same day = good problem-solving
- No multi-day blockers = team is effective
- Pattern: most blockers solved by end of day

---

## Grade This Week

**Overall Grade: ⭐⭐⭐⭐ (4/5 stars)**

**Why This Grade:**
✅ All P0 objectives completed on schedule
✅ Quality metrics all green (0 errors, 100% tests, clean build)
✅ Velocity reliable (2 hours ahead, estimates accurate)
✅ No rework needed
✅ Team workflow efficient (daily planning, PM reviews working)

🔄 Minor: iPad testing should have started earlier
🔄 Minor: Could have pushed scope harder (were ahead)

**Comparison to baseline:**
- Better than Week 1: Estimates more accurate (+5%)
- Same quality: Both weeks 0 errors, 100% tests
- Better velocity: Week 2 ahead, Week 1 on target

---

## Recommendations for Week 3

1. **Start with aggressive scope** — Week 2 shows capacity
2. **Test across all devices from Day 1** — iPad caught late
3. **Reuse button patterns** — Already established good design
4. **Use preview-first approach** — Faster iteration
5. **Maintain daily PM reviews** — Catching issues early

---

## Preview: Week 3

Based on Week 2 results:

**Phase:** Phase 2 - Frontend (continuing)

**Focus:** Button logic and state management

**Adjustments:**
- Start with more aggressive scope (were 5% ahead)
- Add device testing earlier in the week
- Apply reusable button pattern to new controls

**Known Challenges:**
- Audio state management will be more complex
- State synchronization between UI and logic
- Mock data structures need to be well-designed

**Team Confidence:** High
- Week 2 showed accurate estimates and efficient execution
- Team has good patterns and process
- Ready to tackle more complex work

---

**Created:** Jan 10, 2025
**Discussed With:** Solo developer (retrospective)
**Approved By:** Project owner
```

---

## When to Ask for Clarification

Ask the human if:
- ❓ "What were the actual results?" (need specifics)
- ❓ "What did the team say went well?" (need retrospective feedback)
- ❓ "What were the blockers?" (need challenge details)
- ❓ "How many tests passed?" (need quality data)
- ❓ "Should we adjust scope next week?" (get human input)

---

## Tips

✅ **DO:**
- Base adjustments on actual data (velocity, quality)
- Make reflections specific with examples
- Identify patterns (e.g., all blockers resolved same day = good)
- Grade objectively based on metrics
- Make recommendations actionable
- Compare to previous weeks (show trends)

❌ **DON'T:**
- Make vague statements ("good work")
- Ignore metrics and base on feelings
- Skip learnings section
- Make reflections generic
- Forget to grade the week
- Skip recommendations for next week

---

## Key Rules

**Base Everything on Data:**
- Use actual hours, not opinions
- Use test pass rates, not "it works"
- Use build status, not "looks good"

**Be Specific About Learnings:**
- Not: "Communication was good"
- Yes: "Daily 15-min planning saved 2 hours rework"

**Make Adjustments Actionable:**
- Not: "Try to be faster next week"
- Yes: "Week 2 was 5% ahead, add 2 P1 items Week 3"

**Grade Objectively:**
- Based on: P0 completion, quality metrics, velocity
- Not based on: Effort, difficulty, team mood

---

## Files to Reference

- **Template:** `workflows/05-weekly-retrospective/template.md`
- **Instructions:** `workflows/05-weekly-retrospective/README.md`
- **Daily plans:** `docs/plan/week-X/day-Y-plan.md` (all 5 days)
- **Progress log:** `docs/plan/week-X/progress.md`
- **Previous summary:** `docs/plan/week-X-1/summary.md` (for comparison)
- **Master progress:** `docs/plan/master-progress.md` (to update)
