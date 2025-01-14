
# **UltiPrompting: Advanced Prompting Framework for Fullstack Applications**

**UltiPrompting** combines cutting-edge techniques in prompt engineering with an easy-to-use, modular approach for creating fully functional fullstack applications. This README provides clear, step-by-step instructions to guide the development process.

---

## **How to Use the UltiPrompting Framework**

Follow these steps sequentially to create and refine a fullstack application:

---

### **Step 1: Start with Documentation Creation**

The foundation of any project begins with strong documentation.

#### **Prompt**
```plaintext
Create complete project documentation. Follow these steps:

### Step 1: Gather Information
1. Ask detailed questions to collect all necessary information:
   - What is the product’s name and purpose?
   - Who is the target audience?
   - What are the must-have features?

### Step 2: Build Documentation Files
1. Create or update the following files:
   - `/docs/overview.md`: Project goals, target audience, and key value.
   - `/docs/features.md`: Detailed feature list with dependencies and scenarios.
   - `/docs/system_architecture.md`: Diagrams and communication flows.
   - `/docs/agents.md`: Detailed descriptions of each agent’s purpose, functionality, and specific tasks.
     ```plaintext
     ## Example Agent Entry
     ### MVP Agent
     Purpose: Build a browser-testable Minimum Viable Product.
     Triggers: Missing or incomplete core features.
     Workflow:
       - Identify and implement essential features.
       - Test functionality in a browser environment.
       - Log outcomes in `/docs/progress_X.md`.

     ### Testing Agent
     Purpose: Validate the robustness of the application.
     Triggers: New features added or bugs identified.
     Workflow:
       - Create and execute unit, integration, and end-to-end tests.
       - Log test results and gaps in `/docs/progress_X.md`.
       - Propose fixes for failures.

     ### Design Agent
     Purpose: Refine system architecture and user experience.
     Triggers: Need for optimization or design updates.
     Workflow:
       - Propose architectural improvements.
       - Create or update design diagrams in `/docs/system_architecture.md`.
       - Ensure compatibility with existing features.
     ```
2. Validate the initial documentation for completeness and alignment with project goals.
```

---

### **Step 2: Progress Documentation Management**

Keep track of development progress with detailed logs.

#### **Prompt**
```plaintext
Manage progress documentation dynamically. Follow these steps:

### Step 1: Check Existing Progress Logs
1. Scan the `/docs/` directory for the latest progress file (e.g., `progress_X.md`).
   - If no progress file exists, create `/docs/progress_1.md`.
   - Use the highest-indexed file for ongoing work.

### Step 2: Log Development Activities
1. Update the current progress file with:
   - Tasks completed.
   - Challenges or blockers encountered.
   - Next steps or proposed tasks.

### Step 3: Archive and Create New Logs
1. At the end of an iteration:
   - Rename the current file as archived (e.g., `/docs/progress_X_archived.md`). Use a clear naming convention such as including the date or task in the filename (e.g., `/docs/progress_2023-12-01_archived.md`).
   - Create a new progress file incrementing the index (e.g., `/docs/progress_X+1.md`) to maintain clarity and organization.
```

---

### **Step 3: Iterate and Execute Tasks Dynamically**

This step replaces the need for a separate agent selection step by integrating both agent selection and task execution into a single prompt.

#### **Prompt**
```plaintext
Iteratively refine the application and execute tasks dynamically. Follow these steps:

### Step 1: Retrieve Context
1. Open `/docs/progress_X.md` to review and explicitly fetch the following data:
   - Tasks completed in the last iteration.
   - Pending tasks or blockers.
   - Proposed next steps.
Ensure the AI reads and interprets the data directly from the file to maintain continuity and avoid context loss.
2. Cross-reference `/docs/agents.md` to determine the relevant agent:
   - Identify the agent whose triggers match the current progress log. Ensure that workflows in `/docs/agents.md` are detailed enough to handle complex tasks or dependencies, including edge cases and multi-step processes.
   - Retrieve the agent’s workflow for execution, and validate it against the current project requirements.

### Step 2: Execute the Task
1. Follow the workflow for the selected agent:
   - For MVP Agent: Implement core features and test them in a browser.
   - For Testing Agent: Write and execute tests, then document results.
   - For Design Agent: Refine architecture diagrams and ensure compatibility.
2. Ensure tasks adhere to best practices:
   - Modular, scalable, and maintainable code.
   - Validated outputs with tests and reviews.
   - Include manual validation steps to confirm the tasks meet project goals and align with the expected outcomes beyond automated testing.

### Step 3: Log Progress and Propose Next Steps
1. Update `/docs/progress_X.md` with:
   - Tasks completed and their outcomes.
   - Challenges encountered and how they were resolved.
   - Next steps or recommendations for the following iteration.
```

---

## **How the Prompts Work Together to Create Fullstack Applications**

The UltiPrompting framework is designed to guide you step-by-step through the development process of a fullstack application. Here’s how the prompts interact to deliver results:

1. **Documentation Creation (Step 1)**:
   - Establishes the foundation by defining the product, its features, and the technical requirements.
   - Creates `/docs/agents.md`, detailing the role of each agent, triggers, and workflows.

2. **Progress Documentation Management (Step 2)**:
   - Keeps an ongoing log of actions, ensuring clarity and traceability.
   - Enables agents to dynamically manage tasks without duplication.

3. **Iterative Execution and Refinement (Step 3)**:
   - Dynamically selects the appropriate agent based on `/docs/progress_X.md` and `/docs/agents.md`.
   - Executes workflows specific to the agent (e.g., MVP creation, testing, or design refinement).
   - Logs progress and proposes next steps for iterative improvement.

### **Using the Prompts to Develop Fullstack Applications**

#### **Step 1: Start with Documentation**
- Begin by creating the foundational documentation for your project.
- Use the **Step 1 Prompt** to generate `/docs/overview.md`, `/docs/features.md`, `/docs/system_architecture.md`, and `/docs/agents.md`.

#### **Step 2: Manage Progress**
- Use the **Step 2 Prompt** to keep your progress logs organized and up-to-date.
- Ensure that all completed tasks, blockers, and next steps are recorded in `/docs/progress_X.md`.

#### **Step 3: Execute and Iterate**
- Use the **Step 3 Prompt** repeatedly to:
  - Retrieve context dynamically from the documentation.
  - Select the relevant agent and execute its workflow.
  - Log all progress and refine the application iteratively.

By following these steps, you can efficiently create, test, and refine a fullstack application while maintaining clarity and structure throughout the development lifecycle.

---

## **License**

This project is licensed under the [MIT License](LICENSE).
