# UltiPrompting
An engineered prompting architecture one for creating documentation and another for working on the program documented in the documentation

Spam this prompt:
### Step 1: Analyze and Understand the Current State
1. **Read All Relevant Documentation**:
   - Carefully review /docs/progress.md for:
     - Tasks completed in the last iteration.
     - Issues encountered, challenges resolved, and next steps proposed.
   - Cross-reference these sections for the context needed:
     - /docs/features.md: Ensure feature dependencies and interactions are fully understood.
     - /docs/system_architecture.md: Validate how new features/components fit into the overall architecture.
     - /docs/api_specifications.md: Confirm API dependencies and data flows.
     - /docs/database_schema.md: Identify any database-related changes needed for this iteration.

2. **Summarize the Current State**:
   - Provide a brief summary of the project’s status, including:
     - Features completed so far.
     - Pending tasks or unresolved dependencies.
     - Any outstanding questions or gaps in documentation.

---

### Step 2: Plan the Next Logical Task
1. **Determine Priorities**:
   - Based on /docs/progress.md and current documentation, identify the next most important task.
   - Focus on tasks that:
     - Have clear dependencies on previously completed work.
     - Are required for a milestone or core functionality.
     - Resolve existing issues or gaps.

2. **Propose Tasks**:
   - Suggest one or more tasks for this iteration, including:
     - If documentation: Which file(s) to refine, expand, or create.
     - If coding: Which feature/module/component to implement or enhance.
   - Explain why these tasks are the next logical step.

---

### Step 3: Execute the Task
1. **Update Documentation**:
   - If the task involves documentation:
     - Add or refine content in the relevant /docs/ files.
     - Ensure all changes align with the existing system design and feature dependencies.

2. **Implement Code**:
   - If the task involves coding:
     - Write clean, modular, and maintainable code that aligns with the documentation.
     - Include inline comments to explain functionality.
     - Follow best practices (e.g., DRY, SOLID, security, scalability).

3. **Test and Validate Code**:
   - Write and run unit tests for new code.
   - If applicable, create integration tests to ensure the new feature works with the system.

---

### Step 4: Validate Changes and Integration
1. **Check Compatibility**:
   - Validate that new features or documentation updates integrate seamlessly with existing components.
   - Ensure that changes align with system architecture and design principles.

2. **Proactively Identify Risks**:
   - Highlight potential edge cases, risks, or technical limitations introduced by the changes.
   - Suggest mitigations or follow-ups to address them.

---

### Step 5: Update the Progress Log
Update /docs/progress.md with the following:

1. **Tasks Completed**:
   - List tasks completed in this iteration, along with a brief description of each.
   - Specify files created, updated, or deleted.

2. **Features/Components Added**:
   - Describe new features or components and their interactions with existing parts.

3. **Challenges or Issues**:
   - Document challenges encountered and how they were addressed.
   - Highlight unresolved issues, risks, or dependencies.

4. **Validation Summary**:
   - Summarize validation/testing results.
   - Note any conflicts or adjustments made.

5. **Next Steps**:
   - Propose tasks or refinements for the next iteration.
   - List any outstanding questions or areas requiring clarification.

---

### Improvements Added in This Version:
1. Provide a **summary of the current state** at the start of each iteration, ensuring the AI contextualizes its next task effectively.
2. Include a **risk analysis** step to proactively identify potential issues during integration.
3. Add a **validation summary** section in the progress log to capture testing outcomes and integration results.
4. Emphasize **dependencies and feature interactions** by requiring cross-referencing between multiple documentation files.
5. Propose tasks and explain their importance, keeping the development focused on priorities and milestones.




Create documentation:

Comprehensive Documentation Creation
I want to create the best possible documentation for a fully functional and complex product. Your task is to ensure that the documentation is complete, cohesive, and detailed enough to serve as the foundation for development. Follow these steps:

Step 1: Ask Iterative Questions
At the start, ask detailed questions to collect all necessary information about the product. Ensure the documentation captures all aspects of the project:

Project Overview:

What is the product’s name and purpose?
What is the core problem it solves?
Who is the target audience, and what are their needs?
What are the primary use cases?
Features:

What are the must-have, nice-to-have, and future features?
How should these features interact with each other?
Are there any edge cases or specific scenarios for these features?
System Design:

What architecture will the system use (e.g., monolith, microservices)?
What are the main components (frontend, backend, APIs, database)?
Are there any third-party APIs or integrations involved?
Technical Stack:

What programming languages, frameworks, and tools are required?
Which platforms does the product need to support (web, mobile, desktop)?
Are there constraints or preferences for hosting and deployment?
Data Management:

What kind of data will the application manage?
How should data flow between components?
What security, integrity, and privacy measures are needed?
Step 2: Build the Documentation
Create the following documentation files, ensuring each is highly detailed and interconnected:

/docs/overview.md:

Goals, audience, unique value, and high-level summary.
Primary use cases with examples.
/docs/features.md:

A prioritized list of features with:
Detailed functionality.
Interaction with other features.
Edge cases and user scenarios.
/docs/system_architecture.md:

Architecture diagrams (e.g., flowcharts, system interactions).
Communication flows between components.
/docs/api_specifications.md:

API endpoints: Request/response formats, error handling, and authentication.
Third-party API integration points.
/docs/database_schema.md:

A detailed schema: Tables, fields, relationships, and constraints.
Data integrity and security strategies.
/docs/technical_stack.md:

Programming languages, frameworks, libraries, and tools.
Justification for the technical stack.
/docs/testing_plan.md:

Unit, integration, and end-to-end testing strategies.
Key test cases for verifying functionality.
/docs/deployment_strategy.md:

CI/CD pipelines and hosting setup.
Post-deployment monitoring and scaling plans.
/docs/progress.md:

A progress log for each iteration (template below).
Step 3: Progress Log Template
Maintain this structure in /docs/progress.md for every update:

markdown
Kopier kode
# Project Progress Log

## Date: [YYYY-MM-DD]

### **Task Completed**
- Description of completed tasks.
- Files created, updated, or deleted and their purpose.

### **Key Features/Components Added**
- Detailed list of new features or modules.
- How they interact with existing components.

### **Potential Problems or Challenges**
- Issues encountered and how they were addressed.
- Unresolved dependencies or risks.

### **Best Practices Checklist**
- DRY, SOLID, modularity, scalability, and security standards confirmed.
- Reviewed all feature interactions for conflicts or gaps.

### **Next Steps**
- Outline tasks for the next iteration.
- List questions or areas needing clarification.


## Contributing

Contributions are welcome! Please follow the standard GitHub workflow:
1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Open a pull request

## License

[MIT License](LICENSE)
