---
name: exam-revision
description: Exam revision system builder that transforms any syllabus into a structured, question-driven study plan. Use when user mentions exams, revision, study planning, syllabus breakdown, exam preparation, weak areas identification, or creating a study schedule. Triggers include "help me revise", "exam in X days", "break down this syllabus", "create study plan", "identify weak areas", or any exam preparation request.
---

# Exam Revision System Builder

Transform any syllabus into a clear, repeatable revision system with question-driven learning and weakness-focused planning.

## Workflow Overview

```
Syllabus → Topics → Exam Questions → Weak Areas → Daily Plan → Active Revision → High-Yield Final
```

## Step 1: Gather Information

Ask the user for:
1. **Subject name**
2. **Syllabus** (paste or describe)
3. **Exam date** (days remaining)
4. **Daily study hours available**

## Step 2: Topic Breakdown

Convert the syllabus into clear, exam-oriented topics.

Output format:
```
## Unit 1: [Name]
- Topic 1.1: [Clear topic]
- Topic 1.2: [Clear topic]
  - Subtopic 1.2.1
  - Subtopic 1.2.2

## Unit 2: [Name]
...
```

Guidelines:
- Break vague syllabus points into specific, testable topics
- Group related concepts
- Estimate weight/importance of each unit if possible

## Step 3: Generate Exam Questions

For each topic, generate:

| Type | Count | Purpose |
|------|-------|---------|
| Conceptual | 5 | Test understanding |
| Numerical/Practical | 5 | Test application |
| Short answer | 5 | Test recall |

Format:
```
### Topic: [Name]

**Conceptual Questions:**
1. Explain why...
2. Compare and contrast...

**Numerical/Practical:**
1. Calculate...
2. Solve...

**Short Answer:**
1. Define...
2. List three...
```

## Step 4: Identify Weak Areas

Guide user through self-assessment:

1. Present questions from Step 3
2. Ask user to rate each:
   - ✅ Confident (can answer fully)
   - ⚠️ Partial (some gaps)
   - ❌ Weak (cannot answer)

3. Analyze patterns:
   - Which topics have most ❌/⚠️?
   - What type of weakness? (formulas, concepts, memory)
   - Which subtopics need focus?

Output a **Weak Areas Summary**:
```
### High Priority (❌ Weak)
- Topic X: [specific gap]
- Topic Y: [specific gap]

### Medium Priority (⚠️ Partial)
- Topic Z: [specific gap]

### Weakness Patterns
- Formula retention issues in: [topics]
- Concept confusion in: [topics]
```

## Step 5: Create Daily Revision Plan

Using:
- Days remaining
- Hours per day
- Weak areas priority

Generate a day-by-day plan:

```
### Day 1 (Date)
- [ ] Topic A (weak) - 2 hours
- [ ] Topic B (review) - 1 hour
- [ ] Practice questions - 1 hour

### Day 2 (Date)
...
```

Rules:
- Weak areas get 2x time allocation
- Include daily question practice
- Build in review cycles (Day 1 topics revisited on Day 4)
- Reserve last 5-7 days for high-yield revision

## Step 6: Active Revision Mode

During revision, use active recall methods:

### Method 1: Question Testing
Ask user questions without warning, check answers, provide feedback.

### Method 2: Explain Back
Ask user to explain a concept. Evaluate for:
- Accuracy
- Completeness
- Clarity

### Method 3: Quick Fire
Rapid short questions to test recall speed.

Prompt to offer:
> "Ready to test your knowledge on [topic]? I'll ask questions and check your understanding."

## Step 7: High-Yield Final Revision (Last 5-7 Days)

Identify and focus on:

1. **Most repeated exam topics** - Historical patterns
2. **High-weight questions** - Maximum marks potential
3. **Common mistakes** - Typical student errors
4. **Formula sheets** - Quick reference compilation
5. **Key diagrams** - Visual memory aids

Output:
```
### Must-Know for Exam
1. [Topic] - [Why important]
2. [Topic] - [Why important]

### Common Mistakes to Avoid
1. [Mistake] - [Correct approach]

### Quick Formula Reference
- [Formula 1]
- [Formula 2]
```

## Session Management

### Starting a Session
Begin by asking:
> "What subject are you preparing for? Share your syllabus and tell me your exam date and daily study hours."

### Continuing a Session
If user returns mid-revision:
> "Welcome back! Where did we leave off? Would you like to:
> 1. Continue with the daily plan
> 2. Test yourself on a topic
> 3. Update weak areas
> 4. Jump to high-yield revision"

### Progress Tracking
Maintain awareness of:
- Topics completed
- Weak areas addressed
- Days remaining
- Confidence improvements

## Quick Commands

| User Says | Action |
|-----------|--------|
| "Break down syllabus" | Go to Step 2 |
| "Generate questions" | Go to Step 3 |
| "Find weak areas" | Go to Step 4 |
| "Make daily plan" | Go to Step 5 |
| "Test me on [topic]" | Go to Step 6 |
| "Final revision mode" | Go to Step 7 |
| "Update plan" | Regenerate daily plan with current progress |
