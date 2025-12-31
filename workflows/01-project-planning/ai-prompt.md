# AI Prompt: Project Planning (Workflow 1)

**When to use this:** Week 0, before development starts
**Output file:** `docs/plan/master-plan.md`

---

## Your Task

Generate a complete `master-plan.md` for a software project based on human input.

---

## Input You'll Receive

The human will provide (or you should ask for):

```
PROJECT INFORMATION:
- Project name: [name]
- What problem does it solve: [description]
- Key features (MVP): [list]
- Target timeline: [weeks]
- Team size: [number]
- Tech stack: [languages/frameworks]

SUCCESS CRITERIA:
- [What does "done" look like]
- [Key metrics]

RISKS:
- [Known challenges]
- [Dependencies]
```

---

## What to Generate

Create a complete, filled-out `master-plan.md` with:

1. **Project Overview** (2-3 sentences)
   - What problem it solves
   - What it delivers
   - Why it matters

2. **Success Criteria** (3-5 specific, measurable items)
   - Timeline goal
   - Feature completeness
   - Quality metrics
   - Performance targets

3. **4 Phases** with for each:
   - Duration (weeks)
   - Objective (what gets done)
   - Deliverables (what exists at end)
   - Success criteria (testable)

4. **Timeline** (ASCII timeline showing weeks → phases)

5. **Team** (names and roles)

6. **Scope** (in-scope vs out-of-scope)

7. **Risks** (table: risk, severity, mitigation)

---

## Input Format

When human asks you to do this, they'll provide context like:

```
PROJECT: MyRec Screen Recording App

CONTEXT:
- macOS application for recording screen + audio
- MVP needed by December 31, 2025
- Single developer
- Swift/SwiftUI
- Must be high quality, production-ready

SUCCESS METRICS:
- Ship MVP by Dec 31
- Can record 1+ hour continuously
- Build: 0 errors/warnings
- 100% test pass rate
```

---

## Generation Steps

1. **Read the input** — Understand the project scope
2. **Ask clarifying questions** if anything is unclear:
   - "How many weeks do you have total?"
   - "What's your team size?"
   - "What's the minimum feature set for MVP?"
3. **Fill template** — Use `template.md` as structure
4. **Create realistic phases:**
   - Phase 1: ~1 week (preparation)
   - Phase 2-3: Core build (2-3 weeks)
   - Phase 4: Polish (1-2 weeks)
5. **Set measurable success criteria** — Never vague
6. **Identify real risks** — Based on project complexity

---

## Output Format

Return the **complete master-plan.md** formatted exactly as in `template.md`:

```markdown
# Master Plan - [Project Name]

**Project:** ...
**Owner:** ...
**Start Date:** ...
**Target Completion:** ...

---

## Overview
[Content]

---

## Key Success Criteria
- [ ] [Criteria 1]
- [ ] [Criteria 2]

... (rest of sections)
```

---

## Quality Checklist

Before returning, verify:
- [ ] All 4 phases are defined with clear objectives
- [ ] Timeline is realistic for team size
- [ ] Success criteria are specific and measurable (not vague)
- [ ] Phases total 5-8 weeks typical
- [ ] Risks are real, not hypothetical
- [ ] Team roles are clear
- [ ] MVP is clearly scoped (in vs out)

---

## Example

**Human input:**
```
Building a note-taking app. Solo developer, 6 weeks, React web app.
Core features: create notes, save to cloud, search.
Success: shipped and deployed, 100% test coverage.
```

**AI output should be:**
A complete master-plan.md with:
- Phase 1: Preparation (req, architecture, UI mockups)
- Phase 2: Frontend (React components, mock data)
- Phase 3: Backend (API, database, MVP)
- Phase 4: Polish (testing, deployment, refinement)
- Timeline showing Weeks 1-6 mapped to phases
- Team: Solo developer (you)
- Success: Deployed by [date], 100% test coverage
- Risks: API complexity, deployment unknowns, time constraints

---

## When to Ask for Clarification

Ask the human to clarify if:
- ❓ Timeline is unrealistic for scope (e.g., "build Netflix in 1 week")
- ❓ Team size doesn't match scope (e.g., "1 person building enterprise system")
- ❓ Success criteria are vague ("make it work")
- ❓ Tech stack not specified
- ❓ No MVP scope defined

---

## Tips

✅ **DO:**
- Create realistic phases based on typical project structure
- Make success criteria measurable and specific
- Identify real risks (architecture complexity, dependencies, timeline)
- Adapt phase durations to team size
- Be optimistic but honest

❌ **DON'T:**
- Create phases that are too detailed (high-level only)
- Make success criteria vague
- Ignore timeline constraints
- Skip the risks section
- Assume technologies without confirmation

---

## Output Validation

Your output is good when:
- ✅ Phases are 1-2 weeks each
- ✅ Total timeline matches project goal
- ✅ Success criteria are testable
- ✅ All sections are filled (no placeholders)
- ✅ Team member names are included
- ✅ Risks have specific mitigations
- ✅ MVP scope is crystal clear

---

## Files to Reference

- **Template:** `workflows/01-project-planning/template.md`
- **Instructions:** `workflows/01-project-planning/README.md`
