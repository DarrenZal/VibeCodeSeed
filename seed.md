# Cline Project Bootstrapper (seed.md)

## Objective:
To systematically initialize a new project by defining its scope, creating a foundational outline, and setting up a modular task management system for iterative development with Cline.

## Instructions for Cline:

**Phase 1: Project Definition & Outline Creation**

1.  **Check for Existing Project Outline:**
    * Look for a file named `project_outline.md` in the root of the current project directory.

2.  **Scenario A: `project_outline.md` DOES NOT Exist:**
    * **Action:** Inform the user that no existing outline was found.
    * **Action:** Proceed to ask the user the following questions to gather initial project requirements. Explain that their answers will be used to create a new `project_outline.md`.
        * "What is the primary goal or purpose of this project? What problem are you trying to solve?"
        * "Who are the target users for this project?"
        * "What are the key features and functionalities you envision for the first version?" (Ask for a brief list)
        * "Are there any specific technologies, programming languages, or frameworks you prefer or need to use? (e.g., Python, JavaScript, React, Docker, specific APIs)"
        * "Describe the user interface (UI) and user experience (UX) if applicable. Will it be a web app, mobile app, CLI tool, API, etc.?"
        * "How will data be managed in this project? (e.g., databases, local files, external APIs, no persistent data)"
        * "What are the main deliverables or success criteria for the project?"
        * "Are there any known constraints, non-goals (things explicitly not to be included), or existing systems this project needs to integrate with?"
    * **Action:** Once you have the answers, synthesize them into a structured document. Create a new file named `PROJECT_OUTLINE.md`. This outline should be organized into logical phases and modular, actionable steps (similar to the structure we've used previously, e.g., Setup, Data Processing, Core Logic, Testing, Deployment).
    * **Action:** After creating `PROJECT_OUTLINE.md`, inform the user.

3.  **Scenario B: `project_outline.md` DOES Exist:**
    * **Action:** Inform the user that an existing `project_outline.md` was found.
    * **Action:** Read and analyze the content of `project_outline.md`.
    * **Action:** Identify any potential ambiguities, gaps in detail, missing prerequisites, or areas where more clarification would be beneficial for planning the initial development phase.
    * **Action:** Ask the user clarifying questions to fill these gaps. For example:
        * "The outline mentions [specific feature X]. Could you elaborate on [specific aspect of X]?"
        * "Regarding [Phase Y], are there any specific sub-steps or dependencies I should be aware of that aren't listed?"
        * "To ensure the first phase is actionable, could you provide more detail on [a high-level step in the outline]?"
    * **Action:** Based on the user's responses, ask for confirmation if you should update the existing `PROJECT_OUTLINE.md` with these clarifications, or if they prefer to do it manually. If confirmed, make the updates.

4.  **Create Initial Action Plan:**
    * **Action:** Whether the `PROJECT_OUTLINE.md` was newly created or pre-existing (and potentially updated), now create a more detailed, actionable checklist for the *very first phase* outlined in `PROJECT_OUTLINE.md`.
    * **Action:** Save this checklist into a new file named `PHASE_1_ACTION_PLAN.md`. Use Markdown checkboxes for each task.

**Phase 2: Initialize Task Management System**

1.  **Create `CURRENT_TASK.md`:**
    * **Action:** Create a new file named `CURRENT_TASK.md`.
    * **Action:** Populate `CURRENT_TASK.md` with the *very first actionable task* from `PHASE_1_ACTION_PLAN.md`. The structure should be:

        ```markdown
        # CURRENT TASK

        ## Objective:
        ## Background & Key References:
        - See `PROJECT_OUTLINE.md` (relevant section: [Specify section, e.g., Phase 1.1])
        - See `PHASE_1_ACTION_PLAN.md` (this is the first task)

        ## Specific Instructions for Cline:
        ---
        ## Summary of Last Completed Actions (by Cline):
        ## Suggested Next Objective (by Cline):
        ```

**Phase 3: Handover to User**

1.  **Inform User:**
    * **Action:** Notify the user that the project initialization is complete.
    * **Action:** Explain that `PROJECT_OUTLINE.md` contains the overall plan, `PHASE_1_ACTION_PLAN.md` contains the checklist for the current phase, and `CURRENT_TASK.md` contains the immediate next step.
    * **Action:** Instruct the user that for subsequent work, they should:
        1.  Review `CURRENT_TASK.md`.
        2.  Start a new focused session/task with Cline (if Cline supports this, or just a new clear prompt), pointing it to `CURRENT_TASK.md` as the brief.
        3.  After completing the objective in `CURRENT_TASK.md`, ask Cline to summarize its actions and suggest the next objective (from `PHASE_1_ACTION_PLAN.md` or `PROJECT_OUTLINE.md`) directly in `CURRENT_TASK.md` (or provide text for the user to update it).

---
This `seed.md` is now a comprehensive set of instructions for Cline to bootstrap your projects.
