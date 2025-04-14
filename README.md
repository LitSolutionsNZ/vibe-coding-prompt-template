# Development Workflow: Gemini + AI IDE (e.g., Copilot)

This guide details a structured workflow using Google’s Gemini tools and an AI-powered IDE (like VS Code + GitHub Copilot) to define and code an application MVP, assuming you have specific prompt templates for certain steps.

## Workflow Overview

1.  **Generate Deep Research (Gemini Website):** Create a research report on your topic using Gemini Website and your dedicated research prompt template.
2.  **Generate PRD & TDD (Gemini App / AI Studio):** Run your interactive PRD/TDD template prompt to produce the MVP’s PRD and TDD documents.
3.  **Create IDE Context (`NOTES.md`):** Summarize key specs from the PRD/TDD in a `NOTES.md` file for your IDE’s AI assistant.
4.  **Generate Code (AI IDE):** Write code feature-by-feature in your AI IDE, using `NOTES.md` for context, and test locally.
5.  **Refine Code (AI IDE):** Debug, refactor, and improve the generated code, then validate with users and deploy the app.

---

## Step 1: Generate Deep Research (Gemini Website)

Use [Gemini Website](https://gemini.google.com/app) with your research prompt template to generate a comprehensive research report.
* The prompt will ask you a multitude of questions about what you want.
* After you answer, it'll then give you a deep research prompt that then you'll put into Gemini Deep Research with 2.5 Pro.
* P.S. OpenAI and Perplexity works as well, but I prefer Gemini.

**Goal:** Obtain foundational background information to inform the PRD.
**Output:** Research findings document (e.g., `research-report.md`).

---

## Step 2: Generate PRD & TDD (Gemini App / AI Studio)

1.  Execute your "Interactive Prompt for Generating PRD and TDD" template in Gemini App or aistudio.google.com. Complete the Q&A process.
2.  Review the generated PRD and TDD for accuracy (e.g., ensure PRD has user stories, TDD has a feasible tech stack).
3.  Save the documents as `PRD.md` and `TDD.md` in your project repository (after creating it on GitHub).

**Goal:** Produce formal PRD and TDD documents for the MVP.
**Output:** Separate PRD (`PRD.md`) and TDD (`TDD.md`) documents.

---

## Step 3: Create IDE Context (`NOTES.md`)

1.  Create a `NOTES.md` file in your project’s root directory (after setting up the repository on GitHub).
2.  Summarize critical information from your PRD and TDD, focusing on:
    * Core purpose and MVP goal.
    * Key user stories (must-haves).
    * Core MVP features (prioritize must-haves).
    * UI concept.
    * Tech stack and architecture overview.
3.  Commit `NOTES.md` to your GitHub repository.

**Example `NOTES.md` Structure:**

```markdown
# Project Notes: [App Name] MVP

## Core Purpose
- Solves [Problem] for [Target Audience].
- MVP Goal: [Specific Goal].

## Key User Stories (from PRD)
1. As a [User Type], I want to [Action], so that [Benefit].
2. ...

## Core MVP Features (from PRD)
- [Feature 1 Name]: Must-Have. Desc: ...
- [Feature 2 Name]: Must-Have. Desc: ...
- ...

## UI Concept (from PRD)
- [Brief description].

## Tech Stack (from TDD)
- Platform: [e.g., Web App]
- Frontend: [e.g., HTML, Tailwind CSS, Vanilla JS]
- Backend: [e.g., Python (Flask)]
- AI API: [e.g., Google AI API]
- Key Libraries: [e.g., requests]

## Architecture Overview (from TDD)
- [Brief flow].
Goal: Provide a concise reference sheet in the IDE for the AI assistant.Step 4: Generate Code (AI IDE)Work in your AI-powered IDE (VS Code + Copilot, Cursor, etc.) to generate code:Setup: Clone your GitHub repository (git clone), create necessary files/folders (e.g., app.py, index.html), and install dependencies based on the tech stack in NOTES.md.Code Generation: Use NOTES.md as the context source to prompt the AI assistant (inline via comments or in the chat panel). Generate code feature-by-feature using specific, contextual prompts based on your notes.Test: After generating each feature, run the app locally to verify it works as expected (e.g., test the /generate endpoint).Commit: Commit the code to GitHub after each feature (git add ., git commit -m "Add [feature]", git push).Goal: Build the application iteratively, ensuring each feature aligns with NOTES.md specs and works correctly.Step 5: Refine Code (AI IDE)Use your IDE’s AI assistant to refine the generated code:Refine: Perform actions like explaining, refactoring, fixing bugs, and generating documentation using the AI assistant. Use specific prompts related to the code and requirements.Validate: Share the app with a small group (e.g., colleagues, target users) to gather feedback. Update the code based on feedback if needed.Deploy: Package or deploy the app (e.g., for a web app, deploy to Netlify; for a desktop app, create a distributable package). Share the app link or binary.Commit: Commit final changes to GitHub (git add ., git commit -m "Final MVP refinements", git push).Goal: Ensure the code is clean, functional, meets MVP requirements (ref NOTES.md), and is validated by users before final deployment.Tips for SuccessKeep NOTES.md Updated: Reflect minor requirement changes here (major ones need Step 2 redo).Provide Context: Reference NOTES.md or paste relevant snippets in AI prompts.Be Specific: Clear prompts get better results.Iterate: Generate, test, refine.Focus Prompts: Ask for smaller code chunks (functions, components).Version Control: Use Git commits frequently to track progress and revert if needed.
