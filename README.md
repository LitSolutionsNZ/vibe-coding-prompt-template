# Development Workflow: Gemini + AI IDE (e.g., Copilot)

This guide details a structured workflow using Google’s Gemini tools and an AI-powered IDE (like VS Code + GitHub Copilot) to define, generate, and refine an application MVP. This workflow utilizes specific prompt templates provided in this repository (`part1-deepresearch.md`, `part2-interactive-prd-tdd.md`, `part3-generate-mvp-code.md`).

## Workflow Overview

1.  **Generate Deep Research (Gemini Website):** Use `part1-deepresearch.md` to create a research propmpt on your topic for you to use on [Gemini Website](https://gemini.google.com/app).
2.  **Generate PRD & TDD (Gemini App / AI Studio):** Use `part2-interactive-prd-tdd.md` (your interactive PRD/TDD template prompt) to produce the MVP’s Product Requirements Document (PRD) and Technical Design Document (TDD).
3.  **Generate MVP Code (Gemini App / AI Studio):** Use `part3-generate-mvp-code.md`. Paste the outputs from Step 1 (Research) and Step 2 (PRD, TDD) into this prompt at the bottom to generate the initial source code for the MVP.
4.  **Create IDE Context (`NOTES.md`):** Summarize key specs from the PRD/TDD in a `NOTES.md` file. This will serve as a quick reference for your AI assistant *during refinement* in the IDE.
5.  **Setup & Initial Code Integration (AI IDE):** Set up your local development environment and integrate the code generated in Step 3. Perform initial validation.
6.  **Refine & Iterate Code (AI IDE):** Use your AI IDE (e.g., Copilot) along with `NOTES.md` to debug, refactor, enhance, and test the codebase generated in Step 3. Validate with users and deploy.

---
## Recommended LLM:

For Deep Research: Gemini Deep Research with 2.5 Pro
For the rest: Gemini 2.5 Pro
---

## Step 1: Generate Deep Research (Gemini Website)

Use [Gemini Website](https://gemini.google.com/app) with the **`part1-deepresearch.md`** prompt template.
* Follow the instructions within `part1-deepresearch.md`. It guides you through a question-and-answer process with the AI to define your research scope.
* The goal is to collaboratively generate a clear deep research prompt.
* Once the Q&A is complete, the AI will synthesize the information into a deep research prompt, which you will paste and run it on Gemini Deep Research with 2.5 Pro.
* Save this deep research output for Step 3.

---

## Step 2: Generate PRD & TDD (Gemini App / AI Studio)

1.  Execute the **`part2-interactive-prd-tdd.md`** prompt template in Gemini App or aistudio.google.com. Complete the Q&A process defined in that prompt.
2.  Review the generated PRD and TDD for accuracy (e.g., ensure PRD has user stories, TDD has a feasible tech stack).
3.  Save the outputs anywhere on your computer. Save the content for Step 3.

---

## Step 3: Generate MVP Code (Gemini App / AI Studio)

1.  Use the **`part3-generate-mvp-code.md`** prompt template in Gemini App or AI Studio.
2.  **Paste Inputs:** Copy the Deep Research output from Step 1 and the full content of `PRD.txt` and `TDD.txt` from Step 2 into the designated sections within the `part3` prompt (at the bottom).
3.  **Execute Prompt:** Run the complete prompt. The AI will act as a Senior Software Engineer to generate the initial codebase based strictly on the provided PRD and TDD, using the research for context.
4.  **Review & Save:** Review the generated code for completeness and adherence to the TDD. Save the generated code into the appropriate files within your project structure (e.g., `app.py`, `index.html`, `style.css`).

---

## Step 4: Create IDE Context (`NOTES.md`)

1.  Create a `NOTES.md` file in your project’s root directory (if you haven't already alongside PRD/TDD).
2.  Summarize critical information from your PRD and TDD using Gemini 2.5 Pro, making the AI focus on:
    * Core purpose and MVP goal.
    * Key user stories (must-haves).
    * Core MVP features (prioritize must-haves).
    * UI concept.
    * Tech stack and architecture overview.
3.  This file serves as a quick reference for you and your AI IDE assistant during the refinement phase (Step 6).
4.  Commit `NOTES.md` to your GitHub repository.

**Example `NOTES.md` Structure which you can paste into Gemini 2.5 Pro:**

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
Goal: Provide a concise reference sheet in the IDE for guiding AI-assisted refinement.Step 5: Setup & Initial Code Integration (AI IDE)Work in your local development environment and IDE:Setup: Clone your GitHub repository (git clone ...). Ensure you have the code files generated in Step 3 saved in the correct project structure. Install dependencies based on the tech stack (npm install, pip install -r requirements.txt, etc.).Initial Run: Try running the application locally based on standard procedures for the tech stack. Perform basic smoke tests to ensure it runs without immediate errors.Commit: Commit the initial codebase generated from Step 3 to your repository (git add ., git commit -m "Add initial MVP code generated by Part 3 prompt", git push).Goal: Get the generated codebase running in your local environment and under version control.Step 6: Refine & Iterate Code (AI IDE)Use your AI-powered IDE (VS Code + Copilot, Cursor, etc.) to improve and finalize the code:Refine: Work through the codebase feature by feature or file by file. Use your AI assistant, providing context from NOTES.md or specific code snippets, to:Explain complex code sections.Refactor for clarity, efficiency, or adherence to best practices.Fix bugs identified during testing.Add or improve comments and documentation.Implement more robust error handling if needed.Make minor adjustments based on initial testing.Test: Continuously test the application locally as you refine it. Test individual features and the overall workflow.Validate: Share the app with a small group (e.g., colleagues, target users) to gather feedback. Update the code based on feedback if needed.Deploy: Package or deploy the app (e.g., for a web app, deploy to Netlify; for a desktop app, create a distributable package). Share the app link or binary.Commit: Commit changes frequently during refinement (git add ., git commit -m "Refactor feature X", git push). Commit final changes before deployment (git commit -m "Final MVP refinements").Goal: Ensure the code is clean, robust, functional, meets MVP requirements (ref NOTES.md, PRD, TDD), and is validated by users before final deployment.Tips for SuccessKeep NOTES.md Handy: Use it as a quick reference during Step 6 refinement. Major requirement changes should ideally go back to Step 2 (PRD/TDD) and potentially Step 3 (code regeneration).Provide Context to IDE AI: When asking for refinement help in Step 6, reference NOTES.md or paste relevant code snippets/PRD/TDD sections into the AI assistant's chat or comments.Be Specific with Prompts: Clear prompts get better results, both in the initial generation (Steps 1-3) and refinement (Step 6).Iterate: Generate (Step 3), Integrate (Step 5), Refine & Test (Step 6).Focus Refinement Prompts: Ask the IDE AI for specific, smaller tasks (
