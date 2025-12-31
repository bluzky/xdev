# AI Workflow Guide

Use this guide to give AI instructions for each workflow.

---

## How AI Prompts Work

Each workflow has 3 files:

1. **README.md** — For humans (step-by-step instructions)
2. **template.md** — Blank form to fill in
3. **ai-prompt.md** — Structured instructions for AI ← **USE THIS WITH AI**

---

## Quick: How to Ask AI to Do Work

### Step 1: Choose Your Workflow

Tell AI which workflow:
```
"Help me with Workflow 2: Weekly Planning"
```

### Step 2: Provide Context

Give AI the information it needs:
```
"I'm planning Week 3.

Previous week data:
- Estimated: 40 hours, Actual: 38 hours
- All tests passed, 0 build errors
- Team was 2 hours ahead of schedule

For Week 3:
- Phase 2 - Frontend Build (continuing)
- Team capacity: 40 hours
- Focus: Audio controls and state management"
```

### Step 3: Let AI Read the Prompt

Direct AI to the prompt file:
```
"Follow the instructions in workflows/02-weekly-planning/ai-prompt.md

Use the template at workflows/02-weekly-planning/template.md

Generate the complete week-3-plan.md"
```

### Step 4: AI Generates the Output

AI will produce:
- Complete, filled-out document
- Specific and testable criteria
- Realistic time estimates
- Based on your context

---

## AI Prompts by Workflow

### Workflow 1: Project Planning
**Use this:** Week 0, project setup
**AI Prompt File:** `workflows/01-project-planning/ai-prompt.md`

**What to tell AI:**
```
"I'm starting a new project. Help me create master-plan.md

Project Details:
- Name: [Project name]
- What it does: [Description]
- Core features: [List]
- Timeline: [Weeks available]
- Team size: [Number]

Follow: workflows/01-project-planning/ai-prompt.md
Template: workflows/01-project-planning/template.md
Output: docs/plan/master-plan.md"
```

---

### Workflow 2: Weekly Planning
**Use this:** Every Monday morning
**AI Prompt File:** `workflows/02-weekly-planning/ai-prompt.md`

**What to tell AI:**
```
"Plan Week 3 for me.

Context:
- Phase: Phase 2 - Frontend Build
- Week 1 results: [summary of what got done]
- Week 2 velocity: Estimated 40 hours, Actual 38 hours
- Team capacity: 40 hours this week

Current state: [What exists now]
Target state: [What should exist Friday]

Follow: workflows/02-weekly-planning/ai-prompt.md
Template: workflows/02-weekly-planning/template.md
Output: docs/plan/week-3-plan.md"
```

---

### Workflow 3: Daily Planning
**Use this:** Every morning at 9 AM
**AI Prompt File:** `workflows/03-daily-planning/ai-prompt.md`

**What to tell AI:**
```
"Create Day 1 plan for Week 3.

Context:
- From Week Plan: [What Day 1 should accomplish]
- Goal: [Specific day goal]
- Time available: ~8 hours
- Architecture: [Key decisions]

Follow: workflows/03-daily-planning/ai-prompt.md
Template: workflows/03-daily-planning/template.md
Output: docs/plan/week-3/day-1-plan.md"
```

---

### Workflow 4: Daily Tracking
**Use this:** At 5 PM end of day
**AI Prompt File:** `workflows/04-daily-tracking/ai-prompt.md`

**What to tell AI:**
```
"Complete the execution sections for Day 1.

Day 1 Results:
- Time: 9 AM - 5 PM (7 hours actual work)
- Tasks completed: Task 1, Task 2, Task 3, Task 4
- Build status: 0 errors, 0 warnings
- Tests: 100% passing (12/12)
- Blockers: None
- PM review: Approved

Follow: workflows/04-daily-tracking/ai-prompt.md
Update:
  - docs/plan/week-3/day-1-plan.md (execution section)
  - docs/plan/week-3/progress.md (daily entry)"
```

---

### Workflow 5: Weekly Retrospective
**Use this:** Friday 4:30 PM
**AI Prompt File:** `workflows/05-weekly-retrospective/ai-prompt.md`

**What to tell AI:**
```
"Create Week 3 retrospective summary.

Week 3 Results:
- Estimated: 40 hours, Actual: 39 hours
- P0 objectives: All 4 completed
- P1 objectives: 2 of 3 completed
- Test pass rate: 100%
- Build: 0 errors, 0 warnings
- Blockers: 1 (audio state management, fixed)

Team feedback:
- What went well: [Feedback from retrospective]
- What was harder: [Feedback]
- Surprises: [Feedback]

Follow: workflows/05-weekly-retrospective/ai-prompt.md
Generate:
  - docs/plan/week-3/summary.md
  - Update: docs/plan/master-progress.md"
```

---

## Each Workflow's AI Prompt Includes

Every `ai-prompt.md` file contains:

✅ **Your Task** — What AI should do
✅ **Input You'll Receive** — What the human provides
✅ **What to Generate** — Exactly what output is needed
✅ **Input Format** — Example of how human will ask
✅ **Generation Steps** — Step-by-step process for AI
✅ **Output Format** — Expected format with examples
✅ **Quality Checklist** — Verify before returning
✅ **Examples** — Real examples of good vs bad
✅ **Tips & Rules** — Do's and don'ts
✅ **File References** — Where to find templates

---

## File Structure for Reference

```
workflows/
├── 01-project-planning/
│   ├── README.md          ← Read first (human)
│   ├── template.md        ← Blank form
│   └── ai-prompt.md       ← Give this to AI ✅
│
├── 02-weekly-planning/
│   ├── README.md          ← Read first (human)
│   ├── template.md        ← Blank form
│   └── ai-prompt.md       ← Give this to AI ✅
│
├── 03-daily-planning/
│   ├── README.md          ← Read first (human)
│   ├── template.md        ← Blank form
│   └── ai-prompt.md       ← Give this to AI ✅
│
├── 04-daily-tracking/
│   ├── README.md          ← Read first (human)
│   ├── template.md        ← Blank form
│   └── ai-prompt.md       ← Give this to AI ✅
│
└── 05-weekly-retrospective/
    ├── README.md          ← Read first (human)
    ├── template.md        ← Blank form
    └── ai-prompt.md       ← Give this to AI ✅
```

---

## Complete Example: Week 2 Planning with AI

### What You (Human) Do:

1. Read the weekly plan from master-plan.md
2. Gather context from Week 1 results
3. Ask AI to plan Week 2:

```
"Create week-2-plan.md using Workflow 2.

Context:
Phase: Phase 2 - Frontend Build
Week 1 completed:
  - Architecture approved
  - UI mockups finalized
  - Development environment set up
  - Estimated 40 hours, Actual 38 hours

Week 2 goal:
  - Build complete recording UI
  - All controls functional
  - Ready for backend integration

Reference:
- Instructions: workflows/02-weekly-planning/ai-prompt.md
- Template: workflows/02-weekly-planning/template.md"
```

### What AI Does:

1. Reads ai-prompt.md to understand the task
2. Understands you'll provide context (done ✓)
3. Reads template.md to understand structure
4. Generates week-2-plan.md with:
   - Clear week overview
   - Realistic daily breakdown (5 days)
   - P0/P1/P2 objectives
   - Adjusted for Week 1's +5% velocity
   - Specific success metrics
   - Identified risks

### What You Get:

Complete, ready-to-use `week-2-plan.md` that:
- Builds on Week 1 learnings
- Has realistic time estimates
- Clear daily objectives
- Testable deliverables
- Team can start work immediately

---

## When AI Needs to Ask You Questions

AI will ask for clarification if:

- Missing context (previous week data, current state)
- Unclear scope (what's in MVP vs post-MVP)
- Conflicting constraints (timeline vs scope)
- Vague requirements (what does "working" mean?)

**Just answer the questions and AI continues.**

---

## Common Workflow Patterns

### Pattern 1: Project Setup (Week 0)

```
You provide: Project vision, timeline, team size
AI generates: master-plan.md with all phases
You: Review and approve
```

### Pattern 2: Weekly Cycle (Mon-Fri)

```
Monday 9 AM:
  You: "Plan this week" → AI: Generates week-X-plan.md

Monday-Friday (Each Day):
  You: "Plan today" → AI: Generates day-Y-plan.md
  You: "Summarize day" → AI: Updates progress.md

Friday 4:30 PM:
  You: "Retrospective" → AI: Generates summary.md
```

### Pattern 3: Using Previous Week Data

```
Week 1 Summary shows: 5% ahead of schedule
You: "Plan Week 2 with this velocity"
AI: Adjusts scope up, adds P1 items
You: Get more ambitious Week 2 plan
```

---

## Handoff Format for AI

When you ask AI to follow a workflow, provide:

```markdown
# Workflow: [Workflow Name]

## Context
[Provide human context here]

## Instructions
Follow: workflows/XX-workflow-name/ai-prompt.md
Template: workflows/XX-workflow-name/template.md

## Output Location
Create: docs/plan/[your-file].md

## Additional Notes
[Any special requirements]
```

---

## Quality Expectations from AI

When AI follows these prompts, expect:

✅ **Specific, testable acceptance criteria** (not vague)
✅ **Realistic time estimates** based on velocity data
✅ **Clear P0/P1/P2 prioritization**
✅ **Identified risks and mitigations**
✅ **Complete sections** (no placeholders)
✅ **Data-driven adjustments** (from previous weeks)
✅ **Consistent quality** across days/weeks

❌ **No vague statements** ("good", "works", "nice")
❌ **No incomplete sections**
❌ **No unrealistic estimates**
❌ **No contradictions** between daily and weekly plans

---

## Troubleshooting

**Q: AI output is vague or generic**
A: You didn't provide enough context. Give AI specific previous week data, team feedback, blockers.

**Q: AI overestimated time**
A: Provide actual velocity data from previous week. AI uses it to adjust.

**Q: AI generated too much scope**
A: Tell AI the team was slower last week or has less time available.

**Q: AI forgot PM sign-off section**
A: AI didn't read the template. Ask it to follow the template exactly.

**Q: Output has errors**
A: Review against ai-prompt.md quality checklist. Ask AI to fix specific issues.

---

## Quick Reference: Which Prompt to Use

| When | Workflow | Prompt File |
|------|----------|------------|
| Week 0, starting project | 1 | workflows/01-project-planning/ai-prompt.md |
| Monday, 9 AM | 2 | workflows/02-weekly-planning/ai-prompt.md |
| Every day, 9 AM | 3 | workflows/03-daily-planning/ai-prompt.md |
| End of day, 5 PM | 4 | workflows/04-daily-tracking/ai-prompt.md |
| Friday, 4:30 PM | 5 | workflows/05-weekly-retrospective/ai-prompt.md |

---

**You're ready to work with AI on your development workflow!**

Each prompt is detailed, structured, and designed to get high-quality output from AI. Follow the prompts, provide context, and you'll get consistently good documents.
