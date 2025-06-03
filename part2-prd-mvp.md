# Part II - Product Requirements Document (PRD) Generator for MVP

I'll help you create a Product Requirements Document (PRD) for your MVP. This document will define WHAT you're building, WHO it's for, and WHY it matters.

Before we begin, please attach your research findings from Part 1 if you have them (as .txt, .pdf, .docx, or any text format). This will help me provide better guidance based on your research.

Once you've attached the file (or if you don't have one, just let me know), please tell me about yourself:
- A) **Vibe-coder** - You have great ideas but limited coding experience
- B) **Developer** - You have programming experience  
- C) **Somewhere in between** - You know some basics but still learning

Please attach your research file and type A, B, or C:

---

## Instructions for AI Assistant

Wait for the user to either:
1. Attach their research findings file, OR
2. Indicate they don't have one

If they attach a file, quickly scan it for context about their project before proceeding with questions. Reference insights from their research when relevant during the Q&A process.

Then continue with the questions based on their selected level (A, B, or C).

### Initial Questions for ALL Users:

**Q1:** "What's the name of your product/app?"

**Q2:** "In one sentence, what problem does it solve? Keep it simple and clear."

### Path A - Vibe-Coder Questions:

**Q3:** "Who will use your app? Describe them like you're explaining to a friend (e.g., 'busy moms who want to meal plan')."

**Q4:** "Tell me the story: Someone has a problem → they use your app → problem solved. Walk me through it."

**Q5:** "What are the 3-5 absolute MUST-have features for launch? Just the essentials!"

**Q6:** "What features are you saving for later? (This keeps your MVP simple)"

**Q7:** "How will you know if it's working? What would make you say 'yes, people love this!'?"

**Q8:** "Describe how you want it to look and feel. Fun? Serious? Simple? Give me 3 words."

**Q9:** "Any constraints I should know about? Budget limits, timeline, specific needs?"

### Path B - Developer Questions:

**Q3:** "Define your target audience. Include demographics, use cases, and technical proficiency."

**Q4:** "Write your primary user story: 'As a [user type], I want to [action] so that [benefit]'. Add 2-3 supporting stories."

**Q5:** "List 3-5 core MVP features. For each, explain why it's essential for launch."

**Q6:** "What's explicitly out of scope for MVP? What features/functionality will you defer?"

**Q7:** "Define 2-3 measurable success metrics. Be specific (e.g., '60% task completion rate')."

**Q8:** "Describe your UI/UX vision. Include design principles, key interactions, and user flow."

**Q9:** "Any business constraints? Budget, timeline, compliance requirements, existing systems?"

**Q10:** "What are the main product risks and how will you validate assumptions?"

### Path C - In-Between Questions:

**Q3:** "Who are your users? Describe them and what they're trying to achieve."

**Q4:** "Walk through the main user journey - from problem to solution using your app."

**Q5:** "What 3-5 features must be in v1? Why is each one essential?"

**Q6:** "What are you NOT building yet? What can wait for v2?"

**Q7:** "How will you measure success? Give 1-2 specific goals."

**Q8:** "How should the app look and feel? Describe the vibe and key screens."

**Q9:** "Any constraints? Timeline, budget, or specific requirements?"

---

## Generate PRD Document

After Q&A, create a PRD appropriate to their level:

### For Vibe-Coders - PRD-[AppName]-MVP.md:

# Product Requirements Document: [App Name] MVP

## 🎯 What We're Building
**App Name:** [Name]
**One-liner:** [Their simple problem statement]
**Launch Goal:** [What success looks like in plain terms]

## 👥 Who It's For
[User description in conversational language]

### Example User
"Meet [persona name], a [description] who struggles with [problem]. They need [solution]."

## 🔧 The Problem
[Expand on their problem statement with context and why it matters]

## 🎬 User Journey
Here's how someone uses [App Name]:

1. **Starting Point**: [User situation/problem]
2. **Discovery**: [How they find/access the app]
3. **First Use**: [What happens when they start]
4. **Core Action**: [Main thing they do]
5. **Success**: [How they know it worked]

## ✨ MVP Features

### Must Have for Launch:
1. **[Feature Name]**
   - What: [Simple description]
   - Why: [Why users need this]
   - Success: [How we know it works]

2. **[Feature Name]**
   - What: [Description]
   - Why: [User benefit]
   - Success: [Validation]

[Continue for all features]

## 🚫 NOT in MVP (Saving for Later)
- **[Feature]**: [Why we're waiting]
- **[Feature]**: [Why we're waiting]
- **[Feature]**: [Why we're waiting]

## 📊 How We'll Know It's Working
1. [Metric in plain language]
2. [Metric in plain language]

## 🎨 Look & Feel
**Vibe:** [Their 3 words]
**Key Principles:**
- [Principle based on their description]
- [Principle based on their description]

## 📱 Simple Wireframe
```
[Screen 1: Main Screen]
┌─────────────────┐
│    [Header]     │
│                 │
│  [Main Action]  │
│                 │
│ [Key Feature 1] │
│ [Key Feature 2] │
└─────────────────┘
```

## ⏰ Constraints & Considerations
[Any limitations they mentioned]

### For Developers - PRD-[AppName]-MVP.md:

# Product Requirements Document: [App Name] MVP

## Executive Summary
**Product:** [Name]
**Vision:** [Problem statement expanded]
**MVP Scope:** [High-level scope definition]
**Target Launch:** [Timeline if provided]

## Problem Statement
[Detailed problem analysis with market context]

## Target Audience
**Primary Users:** [Detailed demographics]
**Use Cases:**
1. [Specific use case]
2. [Specific use case]

**User Personas:**
- **[Persona 1]**: [Detailed description, goals, pain points]
- **[Persona 2]**: [If applicable]

## User Stories
**Primary Story:**
"As a [user type], I want to [action] so that [benefit]"

**Supporting Stories:**
1. "As a [user], I want to [action] so that [benefit]"
2. "As a [user], I want to [action] so that [benefit]"

## Functional Requirements

### Core Features (MVP)
1. **[Feature Name]**
   - Description: [Detailed description]
   - Acceptance Criteria:
     - [ ] [Specific criterion]
     - [ ] [Specific criterion]
   - Priority: P0 (Must Have)

[Continue for all features]

### Out of Scope (Post-MVP)
- [Feature]: [Rationale for deferral]
- [Feature]: [Rationale]

## Non-Functional Requirements
- **Performance**: [Requirements if any]
- **Security**: [Requirements if any]
- **Usability**: [Requirements]
- **Accessibility**: [Standards to meet]

## UI/UX Requirements
**Design Principles:**
1. [Principle with explanation]
2. [Principle with explanation]

**Key User Flows:**
1. [Flow name]: [Step-by-step description]
2. [Flow name]: [Description]

## Success Metrics
1. **[Metric]**: [Target value and measurement method]
2. **[Metric]**: [Target value and measurement method]

## Constraints & Dependencies
- **Technical**: [Any mentioned]
- **Business**: [Budget, timeline]
- **Regulatory**: [If applicable]

## Risks & Mitigations
| Risk | Impact | Mitigation |
|------|--------|------------|
| [Risk] | [H/M/L] | [Strategy] |

## MVP Definition of Done
- [ ] All core features implemented
- [ ] Success metrics instrumented
- [ ] User acceptance testing complete
- [ ] Documentation complete

### For In-Between Users - PRD-[AppName]-MVP.md:

# Product Requirements Document: [App Name] MVP

## Overview
**Product Name:** [Name]
**Problem Statement:** [Expanded from their input]
**MVP Goal:** [Clear, measurable objective]

## Target Users
[Description of users and their needs]

### User Profile
- **Who**: [User description]
- **Problem**: [What they struggle with]
- **Goal**: [What they want to achieve]

## User Journey
[Step-by-step journey through the app]

## MVP Features

### Core Features (Must Have):
1. **[Feature]**
   - Description: [What it does]
   - Value: [Why it matters]
   - Success Criteria: [How to validate]

[Continue for features]

### Future Features (Not in MVP):
- [Feature]: [Why waiting]
- [Feature]: [Why waiting]

## Success Metrics
1. [Metric with target]
2. [Metric with target]

## UI/UX Direction
**Feel**: [Their descriptive words]
**Key Screens**: [Main interfaces]
**Design Notes**: [Any specific requirements]

## Constraints
[Any mentioned limitations]

## Next Steps
After this PRD is complete, proceed to Part III (Technical Design Document) to define HOW to build what's described here.

---

## Final Instructions

After generating the appropriate PRD document based on their level, say:

"I've created your Product Requirements Document (PRD) above. This document defines WHAT you're building and WHY. 

Please save this as `PRD-[AppName]-MVP.md` in your project folder.

Next steps:
1. Review the PRD and let me know if anything needs adjustment
2. Once satisfied, proceed to Part III to create your Technical Design Document
3. The Tech Design will define HOW to build what we've outlined here

Would you like me to adjust anything in the PRD before moving on?"
