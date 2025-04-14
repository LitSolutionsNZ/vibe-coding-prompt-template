# Development Workflow: Gemini + AI IDE Agent

This guide details a structured workflow using Google’s Gemini tools and an AI-powered IDE Agent (like GitHub Copilot Chat in VS Code, Cursor, etc.) to define, plan, generate, and refine an application MVP. This workflow utilizes specific prompt templates provided in this repository (`part1-deepresearch.md`, `part2-interactive-prd-tech-design.md`, `part3-generate-notes-for-agent.md`).

## Workflow Overview

1.  **Generate Deep Research (Gemini Website):** Use `part1-deepresearch.md` to create a research prompt on your topic for you to use on the [Gemini Website](https://gemini.google.com/app). Capture the key findings/summary.
2.  **Generate PRD & Tech Design Doc (Gemini App / AI Studio):** Use `part2-interactive-prd-tech-design.md` to produce the MVP’s Product Requirements Document (PRD) and Technical Design Document (Tech Design Doc) as separate files (e.g., `PRD-MVP.txt`, `Tech-Design-MVP.txt`).
3.  **Generate IDE Agent Guide (`NOTES.md`) (Gemini App / AI Studio):** Use `part3-generate-notes-for-agent.md`. Provide it with the PRD, Tech Design Doc files from Step 2, and the key findings from the deep research in Step 1. Gemini will generate a structured `NOTES.md` file designed to guide the IDE agent.
4.  **Setup Project & Prompt IDE Agent (AI IDE):** Set up your local project, including the PRD, Tech Design Doc, and the `NOTES.md` generated in Step 3. Activate your IDE Agent and provide an initial prompt instructing it to build the MVP based on these files.
5.  **Supervise Agent Code Generation (AI IDE):** Monitor the IDE agent as it generates the initial codebase, creates files, and follows the plan in `NOTES.md`. Provide clarifications as needed via the agent's chat interface.
6.  **Setup & Validation (AI IDE):** Once the agent completes the initial build, install dependencies, run smoke tests, and ensure the basic structure is functional. Commit the initial code.
7.  **Refine & Iterate Code (AI IDE):** Use the IDE agent or standard AI assistance (like Copilot suggestions) to debug, refactor, add tests, enhance features, and ensure the code meets all requirements, referencing the PRD, Tech Design Doc, and `NOTES.md`.

---
## Recommended LLMs:

* For Deep Research: Gemini Deep Research with 2.5 Pro (or latest powerful model)
* For PRD/Tech Design Doc/NOTES.md Generation: Gemini 2.5 Pro (or latest powerful model)
* For Code Generation/Refinement: Your IDE's integrated AI Agent (Copilot Chat, Cursor, etc.)

## Step 1: [Generate Deep Research (Gemini Website)](https://github.com/KhazP/vibe-coding-prompt-template/blob/main/part1-deepresearch.md)

* ### Disclaimer: If Gemini attempts to create a deep research report with **`part1-deepresearch.md`** prompt, press **Try again without Deep Research** below the Deep Research window.
* Use the [Gemini Website](https://gemini.google.com/app) with the **`part1-deepresearch.md`** prompt template.
* Follow the instructions within the prompt to define your research scope collaboratively, and complete the Q&A process.
* After creating a Deep Research prompt with the Q&A process done, run the resulting research prompt on Gemini.
* **Save the key findings** from the deep research output (e.g., as `Deep-Research-Summary.txt`).

---

## Step 2: [Generate PRD & Tech Design Doc (Gemini App / AI Studio)](https://github.com/KhazP/vibe-coding-prompt-template/blob/main/part2-interactive-prd-tech-design.md)

1.  Execute the **`part2-interactive-prd-tech-design.md`** prompt template in Gemini App or aistudio.google.com. Complete the Q&A process.
2.  Review the generated PRD and Tech Design Doc for accuracy.
3.  **Save the output from the prompts as separate txt files** (e.g., `PRD-MVP.txt` and `Tech-Design-MVP.txt`) in your planned project directory.

---

## Step 3: [Generate IDE Agent Guide (`NOTES.md`) (Gemini App / AI Studio)](https://github.com/KhazP/vibe-coding-prompt-template/blob/main/part3-generate-notes-for-agent.md)

1.  Use the **`part3-generate-notes-for-agent.md`** prompt template in Gemini App or AI Studio.
2.  **Configure the Prompt:** Update the filename placeholders within the prompt to match the actual names of your PRD and Tech Design Doc files saved in Step 2.
3.  **Execute Prompt:** Run the complete prompt, providing the PRD (`PRD-MVP.txt`), Tech Design Doc (`Tech-Design-MVP.txt`), and the saved deep research findings (e.g., `Deep-Research-Summary.txt`) as attachments.
4.  **Review & Save:** Gemini will generate the content for `NOTES.md`. Review it for clarity and accuracy. Save this content as `NOTES.md` in your project directory alongside the PRD and Tech Design Doc.
5.  **Commit Planning Files:** Commit `PRD-MVP.txt`, `Tech-Design-MVP.txt`, `Deep-Research-Summary.txt`, and `NOTES.md` to your GitHub repository.

*Goal: Create a comprehensive guide (`NOTES.md`) derived from the PRD/Tech Design Doc, specifically structured to instruct the AI IDE agent.*

---

## Step 4: Setup Project & Prompt IDE Agent (AI IDE)

1.  **Setup:** Clone your repository (`git clone ...`) to your local machine. Ensure `PRD-MVP.txt`, `Tech-Design-MVP.txt`, `Deep-Research-Summary.txt`, and `NOTES.md` are present in the project root. Set up your basic project environment if needed (e.g., `virtualenv`, `npm init`).
2.  **Activate IDE Agent:** Open your project in your AI-powered IDE (VS Code with Copilot Chat, Cursor, etc.). Activate the chat or agent feature.
3.  **Craft Initial Prompt for Agent:** Provide a clear starting prompt to the agent. This prompt is crucial. Example structure:

    ```text
    Please generate the initial MVP codebase for the '[App Name]' project.

    Your primary instructions and plan are in the `NOTES.md` file in the project root. Please read it carefully first.

    You MUST adhere to the detailed requirements specified in `PRD-MVP.txt` and the technical implementation details outlined in `Tech-Design-MVP.txt`. `NOTES.md` provides a summary and plan based on these files. Additional context may be available in `Deep-Research-Summary.txt`.

    Start by creating the main application file (e.g., `app.py`, `main.js`) and the basic project structure outlined in the Tech Design Doc or `NOTES.md`.

    Let me know if you have any questions before you begin generating the files.
    ```
    *(Adapt the filenames and starting file as needed based on your project)*

4.  **Send Prompt:** Execute the prompt in the agent's interface.

*Goal: Initiate the code generation process by instructing the IDE agent using the prepared planning documents.*

---

## Tips for Success

* **Quality of Inputs is Key:** The better the PRD, Tech Design Doc, and the resulting `NOTES.md`, the better the IDE agent's initial code generation will be.
* **Use a Model with Large Context Window:** Try to use models with large context windows like Claude 3.7 Sonnet Thinking, Gemini 2.5 Pro, and such.
* **Break Down Complex Tasks:** If the agent struggles with the entire MVP at once, prompt it to generate specific parts or features sequentially based on the plan in `NOTES.md`.

