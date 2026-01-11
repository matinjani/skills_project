---
name: assignment-planner
description: Breaks down assignments into manageable tasks with deadlines and progress tracking. Use when user mentions assignments, homework, projects, essays, or needs help planning academic work. Triggers include "plan my assignment", "break down this project", "assignment due", "homework help", "essay planning", or any academic task management request.
---

# Assignment Planner

Break down any assignment into clear, manageable tasks with realistic deadlines.

## Input Gathering

Ask for:
1. **Assignment name/title**
2. **Subject/Course**
3. **Due date**
4. **Assignment type** (essay, project, presentation, lab report, problem set)
5. **Requirements** (word count, pages, specific deliverables)
6. **Current progress** (not started, research done, outline ready, etc.)

## Step 1: Understand the Assignment

Analyze requirements and identify:
- Main deliverables
- Key components/sections
- Research needed
- Resources required
- Grading criteria (if provided)

Output:
```
### Assignment Overview
**Title:** [Name]
**Course:** [Subject]
**Due:** [Date] ([X] days remaining)
**Type:** [Essay/Project/etc.]

### Key Requirements
- [ ] [Requirement 1]
- [ ] [Requirement 2]
- [ ] [Requirement 3]

### Success Criteria
- [What makes this assignment excellent]
```

## Step 2: Break Down into Tasks

Create task breakdown based on assignment type:

### For Essays/Papers:
```
### Phase 1: Research & Planning (30% of time)
- [ ] Understand the prompt/question
- [ ] Brainstorm initial ideas
- [ ] Research sources (aim for X sources)
- [ ] Take notes on key points
- [ ] Create thesis statement
- [ ] Build outline

### Phase 2: Writing (50% of time)
- [ ] Write introduction
- [ ] Write body paragraph 1: [Topic]
- [ ] Write body paragraph 2: [Topic]
- [ ] Write body paragraph 3: [Topic]
- [ ] Write conclusion
- [ ] Add citations

### Phase 3: Review & Polish (20% of time)
- [ ] First read-through for content
- [ ] Check argument flow and logic
- [ ] Edit for clarity and concision
- [ ] Proofread for grammar/spelling
- [ ] Format according to guidelines
- [ ] Final review
```

### For Projects:
```
### Phase 1: Planning (20% of time)
- [ ] Define project scope
- [ ] Identify deliverables
- [ ] List required resources/tools
- [ ] Create project timeline

### Phase 2: Execution (60% of time)
- [ ] [Task 1]
- [ ] [Task 2]
- [ ] [Task 3]
- [ ] Integration/Assembly

### Phase 3: Finalization (20% of time)
- [ ] Testing/Review
- [ ] Documentation
- [ ] Prepare presentation (if needed)
- [ ] Final polish
```

### For Presentations:
```
### Phase 1: Content Development (40% of time)
- [ ] Research topic
- [ ] Outline key points (aim for 1 slide per minute)
- [ ] Gather visuals/data
- [ ] Write speaker notes

### Phase 2: Slide Creation (30% of time)
- [ ] Create title slide
- [ ] Build content slides
- [ ] Add visuals and formatting
- [ ] Create conclusion/summary slide

### Phase 3: Practice (30% of time)
- [ ] First run-through (timing)
- [ ] Refine delivery
- [ ] Practice Q&A responses
- [ ] Final rehearsal
```

## Step 3: Create Timeline

Using:
- Days until deadline
- Estimated hours per task
- User's available time per day

Generate schedule:
```
### Assignment Timeline

**Today ([Date])** - Day 1
- [ ] [Task] - [Estimated time]
- [ ] [Task] - [Estimated time]

**[Date]** - Day 2
- [ ] [Task] - [Estimated time]

**[Date]** - Day 3
- [ ] [Task] - [Estimated time]

...

**[Due Date]** - Final Day
- [ ] Final review and submit
```

Rules:
- Never schedule tasks on the due date (buffer day)
- Front-load difficult tasks
- Include review time
- Add buffer for unexpected delays

## Step 4: Progress Tracking

Offer progress check-ins:
```
### Progress Update

**Completed:**
- [x] [Task 1]
- [x] [Task 2]

**In Progress:**
- [ ] [Current task] - [% complete]

**Remaining:**
- [ ] [Task 3]
- [ ] [Task 4]

**Status:** On track / Behind / Ahead
**Days remaining:** [X]
**Recommendation:** [Next action]
```

## Rescue Mode (Behind Schedule)

If user is behind:
1. Identify remaining essential tasks
2. Cut non-essential elements
3. Create compressed timeline
4. Focus on minimum viable submission

```
### Rescue Plan

**Must complete:**
- [ ] [Essential task 1]
- [ ] [Essential task 2]

**Can skip/minimize:**
- [Non-essential element]

**New timeline:**
- Today: [Tasks]
- Tomorrow: [Tasks]
- Due date: Submit
```

## Quick Commands

| User Says | Action |
|-----------|--------|
| "Plan [assignment]" | Full breakdown from Step 1 |
| "Timeline only" | Skip to Step 3 |
| "Check progress" | Go to Step 4 |
| "I'm behind" | Activate Rescue Mode |
| "What's next?" | Show next task to complete |
| "Adjust deadline" | Recalculate timeline |

## Assignment Templates

### Quick Essay Plan (1000 words)
- Research: 2 hours
- Outline: 30 min
- Draft: 3 hours
- Edit: 1.5 hours
- **Total: ~7 hours over 3-4 days**

### Quick Presentation (10 slides)
- Research: 1.5 hours
- Slides: 2 hours
- Practice: 1 hour
- **Total: ~4.5 hours over 2-3 days**

### Quick Problem Set
- Read problems: 15 min
- Attempt all: [varies]
- Review difficult ones: 30 min
- Final check: 15 min
