# AI Prompt: Weekly Planning (Workflow 2)

**When to use this:** Every Monday morning
**Output file:** `docs/plan/week-X-plan.md`

---

## Your Task

Generate a complete `week-X-plan.md` that breaks down a week's work into 5 daily tasks with realistic time estimates.

---

## Input You'll Receive

The human will provide:

```
CONTEXT:
- Which week number (Week 1, Week 2, etc)
- Current phase (from master-plan.md)
- What exists today (current state)
- What should exist by Friday (target state)

PREVIOUS WEEK (if not Week 1):
- Last week's summary.md
- Actual hours worked vs estimated
- Blockers encountered
- Velocity data

CONSTRAINTS:
- Team size
- Team capacity (hours available)
- Dependencies or prerequisites
- Known risks
```

---

## What to Generate

Create a complete `week-X-plan.md` with:

1. **Week Overview**
   - Current state (what exists now)
   - Target state (what will exist Friday)
   - Focus (main theme)

2. **Week Objectives**
   - P0 (must-have) — required for phase
   - P1 (should-have) — if time allows
   - P2 (nice-to-have) — low priority

3. **Daily Breakdown** (5 days)
   For each day write:
   - Goal (what day accomplishes)
   - Hours (estimated)
   - Deliverable (what gets tested)

4. **Success Metrics**
   - % objectives completed
   - Build status (0 errors)
   - Test pass rate (100%)

5. **Known Risks & Mitigations**

---

## Input Format

Human will ask like:

```
WEEK 2 PLANNING

Phase: Phase 2 - Frontend Build
Context:
- Week 1 complete: architecture and UI mockups done
- Week 2 goal: implement recording UI with all controls
- Team: 1 developer, 40 hours available
- Constraints: Must have all UI elements by Friday

From Week 1 Summary:
- Estimated: 40 hours, Actual: 38 hours (2 hours ahead)
- Quality: Build clean, all tests pass
- Learnings: Architecture decisions solid, estimates were good
```

---

## Generation Steps

1. **Read context** — Understand phase and current state
2. **Review velocity** — Check previous week's actual vs estimate
3. **Plan daily breakdown:**
   - Day 1-4: ~7 hours each (core work)
   - Day 5: ~6 hours (testing, refinement, buffer)
   - Total: ~34-40 hours
4. **Set P0/P1/P2 priorities** — P0 must be achievable in week
5. **Define deliverables** — What gets tested each day
6. **Identify risks** — Based on phase and previous learnings
7. **Fill template** with all sections

---

## Output Format

Return the **complete week-X-plan.md**:

```markdown
# Week X Plan - [Phase/Feature Name]

**Week:** Week X (Monday-Friday, [Dates])
**Phase:** Phase X - [Name]
**Target Completion:** [Date]

---

## Week Overview

**Current State:** [What exists]

**Target State:** [What will exist Friday]

**Focus:** [Main theme]

---

## Week Objectives

### Must-Have (P0)
- [ ] [Objective 1]
- [ ] [Objective 2]

... (rest of sections)
```

---

## Key Rules for Daily Breakdown

✅ **Good daily breakdown:**
```
DAY 1: Set up project structure, implement basic UI
  ~7 hours | Buttons render, clickable, status updates

DAY 2: Recording logic, start/stop functionality
  ~7 hours | Recording starts/stops, file saves

DAY 3: Audio integration with recording
  ~7 hours | Audio and video captured together

DAY 4: Integration and polish
  ~7 hours | Everything works end-to-end, tests pass

DAY 5: Testing, bug fixes, preparation for next week
  ~6 hours | All tests passing, build clean, ready to ship
```

❌ **Bad daily breakdown:**
```
DAY 1: Everything for the week
  ~40 hours | Too much in one day!

DAY 1: "Do stuff"
  ~7 hours | Too vague
```

---

## Velocity Adjustment

**If previous week was faster:**
- Increase scope or complexity
- Add more P1/P2 items
- Don't increase hours (keep 35-40)

**If previous week was slower:**
- Reduce scope
- Move P1 items to next week
- Make P0 items simpler
- Add buffer time

**Example:**
```
Week 1 Actual: 40 hours (estimated 40) — on target
→ Week 2 plan: Keep similar scope

Week 1 Actual: 45 hours (estimated 40) — slower
→ Week 2 plan: Reduce to 3 P0 items, more buffer

Week 1 Actual: 35 hours (estimated 40) — faster
→ Week 2 plan: Add complexity or more features
```

---

## Quality Checklist

Before returning, verify:
- [ ] 5 days clearly defined with goals
- [ ] Total hours realistic (30-40 for full-time week)
- [ ] P0 objectives are achievable by Friday
- [ ] Each day has testable deliverable
- [ ] Daily breakdown makes sense (builds incrementally)
- [ ] Velocity adjusted from previous week (if applicable)
- [ ] Risks identified and real
- [ ] Dependencies documented

---

## Example

**Human input:**
```
WEEK 3 PLANNING

Phase: Phase 2 - Frontend Continued
Previous week: Estimated 40 hours, actual 42 hours
- Recording UI buttons working
- Status display complete
Learning: Audio integration harder than expected

Goal: Implement full recording flow, audio controls, polish
Team: 1 developer, 40 hours available
```

**AI output should be:**

```markdown
# Week 3 Plan - Recording Flow & Audio

**Week:** Week 3 (Jan 6-10)
**Phase:** Phase 2 - Frontend
**Target Completion:** Jan 10, 2025

## Week Overview

**Current State:** Recording UI buttons implemented, status display working

**Target State:** Complete recording workflow, audio input selection, all controls functional

**Focus:** Integrating audio and completing user-facing features

## Week Objectives

### Must-Have (P0)
- [ ] Audio input source selection
- [ ] Recording workflow end-to-end
- [ ] UI controls responsive to recording state
- [ ] All manual tests passing

### Should-Have (P1)
- [ ] Audio level indicators
- [ ] Device permission handling
- [ ] Error messages for edge cases

### Nice-to-Have (P2)
- [ ] Keyboard shortcuts
- [ ] Settings panel

## Daily Breakdown

**DAY 1 (Monday) - Audio Input Setup**
- Estimated: ~7 hours
- Goal: Allow user to select audio source, display available devices
- Deliverable: Audio device list populated, user can select device

**DAY 2 (Tuesday) - Recording Flow Integration**
- Estimated: ~7 hours
- Goal: Connect UI buttons to actual recording start/stop
- Deliverable: Recording starts/stops, file path handled correctly

**DAY 3 (Wednesday) - Audio Capture**
- Estimated: ~7 hours
- Goal: Capture audio from selected device alongside video
- Deliverable: Audio and video recorded together, synchronized

**DAY 4 (Thursday) - Polish UI States**
- Estimated: ~7 hours
- Goal: Handle all UI states (idle, recording, paused, done)
- Deliverable: UI responds correctly to each state, no console errors

**DAY 5 (Friday) - Testing & Preparation**
- Estimated: ~5 hours
- Goal: Manual testing of full workflow, prepare for backend integration
- Deliverable: All tests pass, build clean, documentation ready

## Success Metrics

| Metric | Target |
|--------|--------|
| P0 objectives | 100% complete |
| Build | 0 errors, 0 warnings |
| Tests | 100% passing |
| Time | ~40 hours actual |

## Risks & Mitigations

| Risk | Severity | Mitigation |
|------|----------|-----------|
| Audio API complexity | Medium | Start with simple implementation Monday |
| Sync issues between audio/video | High | Test frequently, prototype Tuesday |
| Permission handling | Medium | Add early in flow, test various scenarios |
```

---

## When to Ask for Clarification

Ask the human if:
- ❓ "What's the current state?" (not provided)
- ❓ "What phase are we in?" (not clear)
- ❓ "Do we have previous week's data?" (helps with estimates)
- ❓ "What are P0 vs P1?" (not clear)
- ❓ "What's the team capacity?" (hours per week)

---

## Tips

✅ **DO:**
- Adjust based on previous week's velocity
- Make daily breakdown incremental (each day adds up)
- Set achievable P0 goals
- Identify real risks
- Account for testing time

❌ **DON'T:**
- Plan more than 40 hours for 1 week
- Make deliverables vague
- Ignore velocity data
- Pack everything into first 3 days
- Skip P1/P2 prioritization

---

## Files to Reference

- **Template:** `workflows/02-weekly-planning/template.md`
- **Instructions:** `workflows/02-weekly-planning/README.md`
- **Master plan:** `docs/plan/master-plan.md` (check phase and timeline)
- **Previous week:** `docs/plan/week-X-1/summary.md` (for velocity)
