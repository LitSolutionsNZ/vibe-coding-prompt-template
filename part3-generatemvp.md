## Part III - Generate MVP Application Code

**Goal:** Generate the complete, runnable source code for the Minimum Viable Product (MVP) based on the provided research summary, Product Requirements Document (PRD), and Technical Design Document (Tech Design Doc).

**AI Role:** Act as a Senior Software Engineer. Your task is to synthesize the information in the provided summary and referenced documents to build the functional MVP application code.

**Inputs & References:**

*   **Deep Research Findings Summary:**
    *   [ USER: PASTE THE CONCISE SUMMARY OR KEY FINDINGS FROM THE PART I DEEP RESEARCH OUTPUT HERE. Focus on goals, target audience insights, and critical context not fully captured in the PRD/Tech Design Doc. Keep it brief to respect context limits. ]

*   **Product Requirements Document (PRD):**
    *   Please refer to the attached/provided PRD file (`[Specify PRD Filename Here, e.g., PRD-MVP.md]`). This document contains the finalized requirements, user stories, features, and scope for the MVP. **This is the primary source for *what* to build.**

*   **Technical Design Document (Tech Design Doc):**
    *   Please refer to the attached/provided Tech Design Doc file (`[Specify Tech Design Doc Filename Here, e.g., Tech-Design-MVP.md]`). This document outlines the agreed-upon tech stack, architecture, data flow, and implementation approach. **This is the primary source for *how* to build it.**

**Instructions for AI:**

1.  **Analyze Inputs:** Carefully read the provided Research Findings Summary and understand the referenced PRD and Tech Design Doc files.
2.  **Prioritize PRD & Tech Design:** Strictly adhere to the requirements, features, platform, UI concepts, tech stack, architecture, data flow, and implementation details specified in the PRD and Tech Design Doc. If there's a conflict between the Research Summary and the PRD/Tech Design, the PRD/Tech Design take precedence.
3.  **Use Research for Context:** Leverage the Deep Research Findings Summary for overall context, understanding user needs, and informing subtle implementation details where the PRD/Tech Design are not specific, but **do not** let it override explicit specifications in the PRD/Tech Design.
4.  **Focus on MVP:** Implement *only* the features listed as 'Core Features' or 'Must-Have' in the PRD. Exclude anything marked as 'Out of Scope'.
5.  **Generate Code:** Produce clean, well-commented, and runnable code for the complete MVP application according to the Tech Design Doc specifications. Use appropriate file blocks for each distinct file (e.g., HTML, CSS, Python script).
6.  **Completeness:** Ensure all necessary code components are included for the application to run based on the specified tech stack.
7.  **Error Handling:** Implement basic error handling as described in the Tech Design Doc/PRD.
8.  **Comments:** Add clear comments explaining the code logic, especially for complex sections or non-obvious decisions.

**Output:**

*   The complete source code for the MVP application, organized into separate file blocks (e.g., ```html name=index.html ... ```, ```python name=main.py ... ```).
*   Brief setup or running instructions *only if* absolutely necessary beyond standard practices for the specified tech stack (e.g., specific API keys needed, non-standard build steps).

---

**Execution Request:**

Please generate the MVP application code based on the provided Research Summary and the referenced PRD and Tech Design Doc files. Remember to prioritize the PRD and Tech Design Doc for specific requirements and implementation details.
