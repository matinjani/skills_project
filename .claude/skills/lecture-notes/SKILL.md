---
name: lecture-notes
description: Converts messy, unorganized lecture notes into clean, structured, exam-ready study material. Use when user shares class notes, lecture content, handwritten notes transcription, or asks to organize/summarize their notes. Triggers include "organize my notes", "clean up these notes", "make my notes exam-ready", "summarize this lecture", or pasting raw lecture content.
---

# Lecture Notes Organizer

Transform messy class notes into structured, exam-ready study material.

## Input Gathering

Ask for:
1. **Raw notes** (paste or describe)
2. **Subject/topic name**
3. **Output preference**: Summary, detailed, or flashcard format

## Processing Steps

### Step 1: Identify Structure

Analyze notes and identify:
- Main topics/headings
- Key concepts
- Definitions
- Formulas (if any)
- Examples
- Important points (marked or emphasized)

### Step 2: Organize Content

Structure the notes using this format:

```markdown
# [Topic Name]

## Overview
[2-3 sentence summary of the entire lecture]

## Key Concepts

### 1. [Concept Name]
**Definition:** [Clear definition]
**Explanation:** [Simple explanation]
**Example:** [If available]

### 2. [Concept Name]
...

## Important Points
- [Point 1]
- [Point 2]
- [Point 3]

## Formulas/Rules (if applicable)
| Name | Formula | When to Use |
|------|---------|-------------|
| [Name] | [Formula] | [Context] |

## Quick Review (Exam Focus)
1. [Key takeaway 1]
2. [Key takeaway 2]
3. [Key takeaway 3]

## Questions to Test Yourself
1. [Question based on content]
2. [Question based on content]
3. [Question based on content]
```

### Step 3: Enhance for Exams

Add:
- **Mnemonics** for lists (if helpful)
- **Connections** between concepts
- **Common exam questions** likely from this material
- **Potential confusion points** to watch out for

## Output Formats

### Format 1: Detailed Notes (Default)
Full structured notes as shown above.

### Format 2: Summary
Condensed 1-page version with only:
- Key definitions
- Main points
- Quick review

### Format 3: Flashcards
Convert into Q&A pairs:
```
Q: What is [concept]?
A: [Definition]

Q: Explain [topic]
A: [Brief explanation]
```

## Quick Commands

| User Says | Action |
|-----------|--------|
| "Just summarize" | Use Format 2 |
| "Make flashcards" | Use Format 3 |
| "Full notes" | Use Format 1 |
| "Add more questions" | Generate 5 more test questions |
| "Explain [concept]" | Expand on specific concept |

## Quality Checklist

Before delivering, ensure:
- [ ] All main topics covered
- [ ] Definitions are clear
- [ ] Examples included where helpful
- [ ] Exam-focused points highlighted
- [ ] Self-test questions added
