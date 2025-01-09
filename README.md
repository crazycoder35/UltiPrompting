
# **UltiPrompting**

**UltiPrompting** is an engineered prompting architecture designed to streamline the creation of comprehensive documentation and support the iterative development of complex applications. It provides a dual-prompt system: one for creating robust documentation and another for working on the program based on that documentation. 

This approach ensures that projects are thoroughly planned, systematically developed, and rigorously validated.

---

## **Core Features**

### **1. Comprehensive Documentation Creation**
UltiPrompting provides a structured workflow for generating high-quality documentation that serves as the foundation for building complex applications. It guides users through:
- Defining the project’s goals, audience, and unique value.
- Identifying key features, system architecture, and technical requirements.
- Mapping dependencies, data flows, and testing strategies.

### **2. Iterative Development**
A secondary prompt ensures continuous progress by:
- Analyzing existing documentation and progress logs.
- Planning and executing the next logical task (coding, testing, or refining documentation).
- Validating changes and updating the progress log.

---

## **Quick Start**

### **Prompt 1: Comprehensive Documentation Creation**

Use the following workflow to create detailed documentation for your project:

#### **Step 1: Ask Iterative Questions**
Collect all necessary information by answering questions in these categories:

- **Project Overview**:
  - What is the product’s name and purpose?
  - What problem does it solve?
  - Who is the target audience, and what are their needs?
  - What are the primary use cases?

- **Features**:
  - What are the must-have, nice-to-have, and future features?
  - How should these features interact with each other?
  - Are there edge cases or specific scenarios?

- **System Design**:
  - What architecture will the system use (e.g., monolith, microservices)?
  - What are the main components (frontend, backend, APIs, database)?
  - Are there any third-party APIs or integrations?

- **Technical Stack**:
  - What programming languages, frameworks, and tools are required?
  - Which platforms should it support (web, mobile, desktop)?
  - Are there constraints or preferences for hosting and deployment?

- **Data Management**:
  - What data will the application manage?
  - How should data flow between components?
  - What security, integrity, and privacy measures are required?

#### **Step 2: Build the Documentation**
Generate the following files to create a solid foundation for development:
- `/docs/overview.md`: Goals, audience, and high-level summary.
- `/docs/features.md`: Detailed feature list, functionality, and dependencies.
- `/docs/system_architecture.md`: Architecture diagrams and communication flows.
- `/docs/api_specifications.md`: API endpoints, request/response formats, and error handling.
- `/docs/database_schema.md`: Detailed database schema with relationships and constraints.
- `/docs/technical_stack.md`: Programming languages, frameworks, and tools used.
- `/docs/testing_plan.md`: Testing strategies and key test cases.
- `/docs/deployment_strategy.md`: CI/CD pipelines, hosting, and scaling plans.
- `/docs/progress.md`: Progress log for iterative updates.

#### **Step 3: Progress Log Template**
Maintain a clear progress log for every update in `/docs/progress.md`:

```markdown
# Project Progress Log

## Date: [YYYY-MM-DD]

### **Tasks Completed**
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
```

---

### **Prompt 2: Iterative Development and Testing**

Use this structured prompt to iteratively develop the application:

#### **Step 1: Analyze and Understand the Current State**
1. Review `/docs/progress.md` for:
   - Tasks completed in the last iteration.
   - Issues encountered and next steps proposed.
2. Cross-reference `/docs/features.md`, `/docs/system_architecture.md`, `/docs/api_specifications.md`, and `/docs/database_schema.md` to ensure all dependencies and interactions are clear.

#### **Step 2: Plan the Next Task**
- Identify and prioritize tasks that:
  - Have dependencies on previously completed work.
  - Are required for core functionality or milestones.
  - Resolve existing gaps or issues.
- Propose coding, testing, or (if necessary) documentation tasks.

#### **Step 3: Execute the Task**
- **Code**: Write clean, modular, maintainable code. Follow best practices (DRY, SOLID, security, scalability).
- **Test**: Write and run unit, integration, and end-to-end tests to validate functionality.

#### **Step 4: Validate Changes**
- Check compatibility with existing components.
- Execute regression tests to ensure no functionality is broken.
- Highlight risks, edge cases, or limitations.

#### **Step 5: Update the Progress Log**
Log all tasks, testing results, and proposed next steps in `/docs/progress.md`.

---

## **Contributing**

Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Push to your branch.
5. Open a pull request.

---

## **License**

This project is licensed under the [MIT License](LICENSE).

---

## **Why UltiPrompting?**
UltiPrompting ensures:
- **Seamless Development**: Comprehensive documentation and structured prompts eliminate ambiguity.
- **Robust Testing**: Integrated testing strategies guarantee quality and reliability.
- **Iterative Refinement**: Continuous updates keep the project aligned with its goals.
