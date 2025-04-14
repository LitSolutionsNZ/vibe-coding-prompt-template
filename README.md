# Development Workflow: Gemini + AI IDE Agent

This guide details a structured workflow using Google’s Gemini tools and an AI-powered IDE Agent (like GitHub Copilot Chat in VS Code, Cursor, etc.) to define, plan, generate, and refine an application MVP. This workflow utilizes specific prompt templates provided in this repository (`part1-deepresearch.md`, `part2-interactive-prd-tech-design.md`, `part3-generate-notes-for-agent.md`).

## Workflow Overview

1.  **Generate Deep Research (Gemini Website):** Use `part1-deepresearch.md` to create a research prompt on your topic for you to use on the [Gemini Website](https://gemini.google.com/app). Capture the key findings/summary.
2.  **Generate PRD & Tech Design Doc (Gemini App / AI Studio):** Use `part2-interactive-prd-tech-design.md` to produce the MVP’s Product Requirements Document (PRD) and Technical Design Document (Tech Design Doc) as separate files (e.g., `PRD-MVP.md`, `Tech-Design-MVP.md`).
3.  **Generate IDE Agent Guide (`NOTES.md`) (Gemini App / AI Studio):** Use `part3-generate-notes-for-agent.md`. Provide it with the PRD and Tech Design Doc files from Step 2. Gemini will generate a structured `NOTES.md` file designed to guide the IDE agent.
4.  **Setup Project & Prompt IDE Agent (AI IDE):** Set up your local project, including the PRD, Tech Design Doc, and the `NOTES.md` generated in Step 3. Activate your IDE Agent and provide an initial prompt instructing it to build the MVP based on these files.
5.  **Supervise Agent Code Generation (AI IDE):** Monitor the IDE agent as it generates the initial codebase, creates files, and follows the plan in `NOTES.md`. Provide clarifications as needed via the agent's chat interface.
6.  **Setup & Validation (AI IDE):** Once the agent completes the initial build, install dependencies, run smoke tests, and ensure the basic structure is functional. Commit the initial code.
7.  **Refine & Iterate Code (AI IDE):** Use the IDE agent or standard AI assistance (like Copilot suggestions) to debug, refactor, add tests, enhance features, and ensure the code meets all requirements, referencing the PRD, Tech Design Doc, and `NOTES.md`.

---
## Recommended LLM:

*   For Deep Research: Gemini Deep Research with 2.5 Pro (or latest powerful model)
*   For PRD/Tech Design Doc/NOTES.md Generation: Gemini 2.5 Pro (or latest powerful model)
*   For Code Generation/Refinement: Your IDE's integrated AI Agent (Copilot Chat, Cursor, etc.)

## Step 1: Generate Deep Research (Gemini Website)

*   Use the [Gemini Website](https://gemini.google.com/app) with the **`part1-deepresearch.md`** prompt template.
*   Follow the instructions within the prompt to define your research scope collaboratively.
*   Run the resulting research prompt on Gemini.
*   **Save a concise summary or the key findings** from the deep research output. (While not directly used by the agent, it informs your understanding and the PRD/Tech Design).

---

## Step 2: Generate PRD & Tech Design Doc (Gemini App / AI Studio)

1.  Execute the **`part2-interactive-prd-tech-design.md`** prompt template in Gemini App or aistudio.google.com. Complete the Q&A process.
2.  Review the generated PRD and Tech Design Doc for accuracy.
3.  **Save these documents as separate files** (e.g., `PRD-MVP.md` and `Tech-Design-MVP.md`) in your planned project directory.

---

## Step 3: Generate IDE Agent Guide (`NOTES.md`) (Gemini App / AI Studio)

1.  Use the **`part3-generate-notes-for-agent.md`** prompt template in Gemini App or AI Studio.
2.  **Configure the Prompt:** Update the filename placeholders within the prompt to match the actual names of your PRD and Tech Design Doc files saved in Step 2.
3.  **Execute Prompt:** Run the complete prompt, providing the PRD and Tech Design Doc files as context/attachments if possible, or ensuring Gemini can access them.
4.  **Review & Save:** Gemini will generate the content for `NOTES.md`. Review it for clarity and accuracy. Save this content as `NOTES.md` in your project directory alongside the PRD and Tech Design Doc.
5.  **Commit Planning Files:** Commit `PRD-MVP.md`, `Tech-Design-MVP.md`, and `NOTES.md` to your GitHub repository.

*Goal: Create a comprehensive guide (`NOTES.md`) derived from the PRD/Tech Design Doc, specifically structured to instruct the AI IDE agent.*

---

## Step 4: Setup Project & Prompt IDE Agent (AI IDE)

1.  **Setup:** Clone your repository (`git clone ...`) to your local machine. Ensure `PRD-MVP.md`, `Tech-Design-MVP.md`, and `NOTES.md` are present in the project root. Set up your basic project environment if needed (e.g., `virtualenv`, `npm init`).
2.  **Activate IDE Agent:** Open your project in your AI-powered IDE (VS Code with Copilot Chat, Cursor, etc.). Activate the chat or agent feature.
3.  **Craft Initial Prompt for Agent:** Provide a clear starting prompt to the agent. This prompt is crucial. Example structure:

    ```text
    Hi [Agent Name],

    Please generate the initial MVP codebase for the '[App Name]' project.

    Your primary instructions and plan are in the `NOTES.md` file in the project root. Please read it carefully first.

    You MUST adhere to the detailed requirements specified in `PRD-MVP.md` and the technical implementation details outlined in `Tech-Design-MVP.md`. `NOTES.md` provides a summary and plan based on these files.

    Start by creating the main application file (e.g., `app.py`, `main.js`) and the basic project structure outlined in the Tech Design Doc or `NOTES.md`.

    Let me know if you have any questions before you begin generating the files.
    ```
    *(Adapt the filenames and starting file as needed based on your project)*

4.  **Send Prompt:** Execute the prompt in the agent's interface.

*Goal: Initiate the code generation process by instructing the IDE agent using the prepared planning documents.*

---

## Step 5: Supervise Agent Code Generation (AI IDE)

1.  **Monitor:** Observe the agent as it processes the information and starts generating files and code.
2.  **Interact:** The agent might ask clarifying questions or state its plan. Respond clearly.
3.  **Correct:** If the agent misunderstands requirements (check against `NOTES.md`/PRD/Tech Design Doc) or generates incorrect code, intervene via chat. Provide specific corrections or point it back to the relevant section in the documents.
4.  **Patience:** Generating a full initial structure might take time and multiple interactions. Guide the agent step-by-step if necessary, potentially focusing on one feature or file structure at a time based on the plan in `NOTES.md`.

*Goal: Guide the IDE agent to produce a complete and accurate initial draft of the MVP codebase based on the specifications.*

---

## Step 6: Setup & Validation (AI IDE)

1.  **Dependency Installation:** Once the agent indicates the initial generation is complete, ensure all necessary dependencies mentioned in the Tech Design Doc (or inferred by the code) are installed (e.g., `pip install -r requirements.txt`, `npm install`).
2.  **Initial Run/Build:** Try running the application or executing its main functions. Perform basic smoke tests.
3.  **Debugging:** Fix any immediate errors required to get the application running at a basic level (you can use the agent for help here too).
4.  **Commit:** Commit the initial, agent-generated codebase (`git add .`, `git commit -m "feat: Initial MVP code generation by AI agent"`, `git push`).

*Goal: Get the agent-generated code into a runnable state and under version control.*

---

## Step 7: Refine & Iterate Code (AI IDE)

Now, treat the agent-generated code as a first draft and use your IDE's AI tools for refinement:

1.  **Review:** Go through the generated code file by file or feature by feature. Compare against `NOTES.md`, PRD, and Tech Design Doc.
2.  **Refactor:** Use the AI agent or inline suggestions (e.g., Copilot) to:
    *   Improve code clarity and readability.
    *   Optimize performance if needed.
    *   Ensure adherence to best practices for the language/framework.
    *   Add or improve comments.
3.  **Debug:** Fix any bugs or logical errors found during testing.
4.  **Enhance:** Implement more robust error handling, add missing minor details, or slightly improve UI/UX based on the initial concept.
5.  **Test:** Write unit tests or perform thorough manual testing. Use the AI agent to help generate test cases.
6.  **Validate:** (Optional) Share with users for feedback.
7.  **Deploy:** Package and deploy the refined MVP.
8.  **Commit Frequently:** Commit changes regularly during refinement (`git commit -m "refactor: Improve error handling for feature X"`).

*Goal: Transform the initial draft into a polished, robust, and fully functional MVP that meets all requirements.*

---

## Tips for Success

*   **Quality of Inputs is Key:** The better the PRD, Tech Design Doc, and the resulting `NOTES.md`, the better the IDE agent's initial code generation will be.
*   **Master Your IDE Agent:** Understand the capabilities and limitations of your specific IDE agent. Learn how to prompt it effectively, especially for reading files (`@workspace` in Copilot Chat, etc.).
*   **Be Specific with the Agent:** Provide clear, concise instructions and corrections during generation (Step 5) and refinement (Step 7).
*   **Break Down Complex Tasks:** If the agent struggles with the entire MVP at once, prompt it to generate specific parts or features sequentially based on the plan in `NOTES.md`.
*   **Don't Trust Blindly:** Always review agent-generated code. It's a powerful assistant, not an infallible developer.
