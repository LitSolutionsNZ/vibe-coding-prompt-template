# Part IV - Generate NOTES.md for AI IDE Agent

I'll help you create a NOTES.md file that will guide your AI IDE agent (like GitHub Copilot, Cursor, Windsurf) to build your MVP.

Please attach the following documents:
1. **Required**: Your PRD document (from Part II)
2. **Required**: Your Technical Design document (from Part III)
3. **Optional**: Your research findings (from Part I)

Attach these files in any text format (.txt, .pdf, .docx, .md), then confirm your technical level:
- A) **Vibe-coder** - Limited coding experience, using AI to build
- B) **Developer** - Experienced programmer
- C) **Somewhere in between** - Some coding knowledge, still learning

Please attach your files and type A, B, or C:

---

## Instructions for AI Assistant

After receiving the files, thoroughly analyze:
- PRD: Product name, features, user stories, UI/UX requirements
- Tech Design: Tech stack, architecture, implementation approach
- Research (if provided): Additional context and insights

Then generate NOTES.md appropriate to their level:

### For Vibe-Coders - Generate NOTES.md:

# NOTES.md - AI Agent Instructions for [App Name]

## 🤖 AI Agent: Read This First!

You are building an MVP for [App Name]. I'm a vibe-coder with limited programming experience, so please:
- Explain what you're doing as you go
- Use simple, working solutions over complex ones
- Ask me before making big decisions
- Create helpful comments in the code

## 📋 What You're Building

**App Name:** [From PRD]
**Purpose:** [Simple explanation from PRD]
**Tech Approach:** [From Tech Design - no-code/low-code/simple stack]

## 👤 User Story
[Primary user story from PRD in simple terms]

## 🏗 Project Setup Instructions

Please create this project structure:
```
[Project structure from Tech Design]
```

### Step 1: Initialize Project
[Specific commands/steps based on Tech Design]

### Step 2: Install Dependencies
```bash
# Install these packages:
[List from Tech Design]
```

### Step 3: Create Base Files
Start with these core files:
1. [Main file] - Entry point
2. [Config file] - Settings
3. [Key component] - Main feature

## ✨ Features to Implement

### Feature 1: [Name from PRD]
**What it does:** [Simple description]
**How to build:**
1. Create [component/file]
2. Add [functionality]
3. Connect to [other part]
4. Test by [simple test]

**Success check:** [How to verify it works]

### Feature 2: [Name from PRD]
[Same structure]

### Feature 3: [Name from PRD]
[Same structure]

## 🎨 UI/UX Implementation

**Design Approach:** [From PRD - their 3 words/description]

### Main Screen
```
[ASCII mockup or description from PRD]
```

**Implementation notes:**
- Keep it [adjective from their description]
- Focus on [key UI element]
- Must be mobile-friendly

## 📱 Responsive Design
Make sure everything works on:
- Mobile (320px - 768px)
- Tablet (768px - 1024px)  
- Desktop (1024px+)

## 🧪 Testing Each Feature

### After implementing each feature:
1. Does [core action] work?
2. Does it match the PRD description?
3. Is it easy to understand?
4. Does it handle errors gracefully?

## ⚠️ Important Constraints
[From Tech Design - limitations, budget, etc.]

## 🚀 Deployment Preparation

When all features are complete:
1. Create README with setup instructions
2. Add .env.example file
3. Test full user journey
4. Prepare for [deployment platform from Tech Design]

## 📝 Code Style Guidelines

- Use clear variable names (e.g., `userEmail` not `email`)
- Add comments explaining "why" not "what"
- Keep functions small (under 20 lines)
- Handle errors with user-friendly messages

## ❓ When You're Unsure

If something is unclear:
1. Check the PRD for requirements
2. Check Tech Design for implementation guidance
3. Ask me for clarification
4. Choose the simpler approach

## 📁 File References
- Full requirements: See `PRD-[AppName]-MVP.md`
- Technical details: See `TechDesign-[AppName]-MVP.md`
- Research context: See `[Research filename if provided]`

## 🎯 Definition of Done
The MVP is complete when:
- [ ] All features from PRD work
- [ ] UI matches the design vision
- [ ] Basic error handling exists
- [ ] README has setup instructions
- [ ] Code has helpful comments
- [ ] It runs without crashing

Start by creating the project structure and base files. Let me know when you're ready to begin!


### For Developers - Generate NOTES.md:

# NOTES.md - AI Agent Instructions for [App Name]

## Overview
Build the [App Name] MVP according to the specifications in the PRD and Technical Design documents.

## Quick Reference
- **Product**: [Name]
- **Stack**: [Tech stack summary]
- **Architecture**: [Pattern]
- **Primary User Story**: [From PRD]

## Project Initialization

### Setup Commands
```bash
# Create project structure
[Specific commands based on tech stack]

# Install dependencies
[Package installation commands]

# Initialize services
[Database, cache, etc.]
```

### Environment Configuration
Create `.env` with:
```
[Required environment variables]
```

## Implementation Plan

### Phase 1: Core Infrastructure
1. **Project Setup**
   - Initialize [framework]
   - Configure [build tools]
   - Set up [testing framework]

2. **Base Architecture**
   - Implement [pattern] structure
   - Create base models/entities
   - Set up routing/controllers

### Phase 2: Feature Implementation

#### Feature 1: [From PRD]
**Acceptance Criteria:**
- [ ] [Criterion 1]
- [ ] [Criterion 2]

**Technical Implementation:**
- Endpoint: `[Method] /api/[path]`
- Frontend: [Component structure]
- Data Model: [Schema/type]
- Business Logic: [Service/handler]

#### Feature 2: [From PRD]
[Similar structure]

### Phase 3: Integration & Polish
- Error handling middleware
- Input validation
- Security measures
- Performance optimization
- Documentation

## Technical Specifications

### API Design
```
[API routes table or OpenAPI snippet]
```

### Database Schema
```sql
[Schema from Tech Design]
```

### State Management
[Approach from Tech Design]

### Security Implementation
- [ ] Authentication: [Method]
- [ ] Authorization: [Strategy]
- [ ] Data validation: [Approach]
- [ ] CORS configuration
- [ ] Rate limiting

## Testing Requirements

### Unit Tests
- Coverage target: [X]%
- Focus areas: [List]

### Integration Tests
- Critical paths: [List]

### E2E Tests
- User journeys: [From PRD]

## Code Quality Standards
- Linting: [Rules/config]
- Type safety: [If applicable]
- Documentation: JSDoc/comments
- Git hooks: pre-commit checks

## Performance Targets
- Page load: < [X]s
- API response: < [X]ms
- Bundle size: < [X]KB

## Deployment Checklist
- [ ] Environment variables configured
- [ ] Database migrations run
- [ ] Build optimization enabled
- [ ] Monitoring configured
- [ ] Error tracking setup
- [ ] CI/CD pipeline working

## References
- PRD: `PRD-[AppName]-MVP.md`
- Tech Design: `TechDesign-[AppName]-MVP.md`
- Research: `[Filename if provided]`

Begin with Phase 1: Core Infrastructure setup.
```

### For In-Between Users - Generate NOTES.md:
```markdown
# NOTES.md - AI Agent Instructions for [App Name]

## 🎯 Project Overview

You're building [App Name] for someone with basic coding knowledge. Please:
- Explain complex concepts simply
- Provide working code with clear comments
- Suggest learning resources when introducing new concepts
- Balance simplicity with best practices

## 📚 What We're Building

**App:** [Name from PRD]
**Purpose:** [Clear explanation]
**Tech Stack:** [From Tech Design with why each choice]
**Learning Goals:** [Technologies they'll understand better]

## 🛠 Setup Instructions

### Prerequisites Check
```bash
# Ensure these are installed:
node --version  # Should be 16+
npm --version   # Should be 8+
git --version   # Any recent version
```

### Project Initialization
```bash
# Create and enter project directory
mkdir [app-name]
cd [app-name]

# Initialize project
[Framework-specific commands with explanations]
```

### Project Structure
```
[Structure with explanations for each directory]
```

## 🚀 Implementation Phases

### Phase 1: Foundation (Day 1-2)
**Goal:** Get basic app running

1. **Setup Project**
   ```bash
   [Commands with explanations]
   ```

2. **Create Base Layout**
   - File: `[layout file path]`
   - Purpose: Main app structure
   - Key concepts: [Component basics, routing]

3. **Test It Works**
   ```bash
   npm run dev  # Start development server
   # Open http://localhost:3000
   ```

### Phase 2: Core Features (Day 3-7)
**Goal:** Implement main functionality

#### Feature 1: [From PRD]
**Learning Focus:** [New concept they'll learn]

1. **Create Component/Module**
   ```javascript
   // [Filename]
   // This handles [what it does]
   [Starter code with comments]
   ```

2. **Connect to App**
   - Where: [File and location]
   - How: [Code snippet]
   - Why: [Explanation]

3. **Test Feature**
   - Action: [What to do]
   - Expected: [What should happen]

#### Feature 2: [From PRD]
[Similar structure]

### Phase 3: Polish & Deploy (Day 8-10)
**Goal:** Make it production-ready

1. **Add Error Handling**
   ```javascript
   // Example of good error handling
   [Code example with explanation]
   ```

2. **Style & Responsiveness**
   - Mobile-first approach
   - Key breakpoints
   - Accessibility basics

3. **Deploy to [Platform]**
   - Step-by-step guide
   - Common issues & fixes

## 💡 Learning Resources

### For [Technology 1]:
- **Quick Start:** [Link/Resource]
- **When Stuck:** [Specific docs page]
- **Video Tutorial:** [If applicable]

### For [Technology 2]:
[Similar structure]

## 🐛 Common Issues & Solutions

### "Error: [Common error]"
**Why it happens:** [Simple explanation]
**Fix:** 
```bash
[Solution with explanation]
```

### "Feature X not working"
**Check these:**
1. [Common cause 1]
2. [Common cause 2]
3. [How to debug]

## 📝 Code Patterns to Use

### Pattern 1: [E.g., Handling User Input]
```javascript
// Good pattern for [use case]
[Code example with comments]
```

### Pattern 2: [E.g., API Calls]
```javascript
// Reusable pattern for [use case]
[Code example with explanation]
```

## 🧪 Testing Your Features

### Manual Testing Checklist:
- [ ] Feature 1: [What to test]
- [ ] Feature 2: [What to test]
- [ ] Error cases: [What to break]
- [ ] Mobile view: [What to check]

### Simple Automated Test:
```javascript
// Example test for [feature]
[Basic test with explanation]
```

## 📊 Understanding the Architecture

### Data Flow:
```
User Action → [Component] → [Handler] → [State/DB] → [UI Update]
```

### Key Concepts Explained:
1. **[Concept 1]:** [Simple explanation with analogy]
2. **[Concept 2]:** [Simple explanation with analogy]

## 🚀 Deployment Guide

### Pre-deployment:
- [ ] Remove console.logs
- [ ] Check all features work
- [ ] Update environment variables
- [ ] Test on different devices

### Deploy to [Platform]:
1. [Step with screenshot reference]
2. [Step with common gotcha]
3. [Verification step]

## 📚 What You've Learned

By completing this MVP, you now understand:
- ✅ [Skill/concept 1]
- ✅ [Skill/concept 2]
- ✅ [Skill/concept 3]

## 🎯 Definition of Done

Your MVP is complete when:
- [ ] All PRD features work
- [ ] Code has helpful comments
- [ ] README explains setup
- [ ] Deployed and accessible
- [ ] You understand how each part works

## 📁 Reference Documents
- Requirements: `PRD-[AppName]-MVP.md`
- Technical Plan: `TechDesign-[AppName]-MVP.md`
- Research: `[Filename if provided]`

## 💬 Final Notes

Remember:
- It's okay to ask for clarification
- Choose simple solutions that work
- Focus on learning one thing at a time
- The goal is a working MVP, not perfect code

Start with Phase 1 and work through systematically. Good luck!

---

## Final Instructions

After generating the appropriate NOTES.md based on their level, say:

"I've created your NOTES.md file above. This document will guide your AI IDE agent through building your MVP.

**Save this as `NOTES.md` in your project root directory.**
