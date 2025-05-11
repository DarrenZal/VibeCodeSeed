# VibeCodeSeed 🌱

**Bootstrap your software projects with AI, the intuitive way!**

VibeCodeSeed provides a universal starter template, `seed.md`, designed to kickstart any software project using AI-powered development assistants like [Cline](https://cline.bot/), [Cursor](https://cursor.sh/), or similar LLM-based tools. It helps you systematically define your project, create a foundational outline, and establish an efficient, modular task management workflow from day one.

Stop staring at a blank canvas and let your AI partner help you vibe out the structure and initial steps of your next big idea!

## What is VibeCodeSeed?

At its core, VibeCodeSeed is a single Markdown file, `seed.md`. This file contains a set of structured instructions that you feed to your AI assistant. The AI then guides you (or directly assists) through:

1.  **Project Definition:** If you're starting fresh, it asks key questions to understand your project's goals, features, UI, tech stack, and more.
2.  **Outline Ingestion:** If you already have a `project_outline.md`, it reads, analyzes, and helps you clarify and expand upon it.
3.  **Structured Planning:** It helps generate a comprehensive `PROJECT_OUTLINE.md` (if one wasn't provided or needed refinement) and a `PHASE_1_ACTION_PLAN.md` with a detailed checklist for the initial phase.
4.  **Modular Task Management Setup:** It initializes a `CURRENT_TASK.md` file, which becomes the central hub for focused, iterative development on a task-by-task basis. This approach is designed to be token-efficient and keep interactions with your AI clear and concise.

## Key Features & Benefits

* 🚀 **Systematic Project Kickoff:** Provides a structured process for defining and planning new projects.
* 🧠 **Handles Blank Slates & Existing Plans:** Adapts whether you have a detailed outline or just a nascent idea.
* 🧩 **Modular Task Management:** Establishes a `CURRENT_TASK.md` workflow, breaking down large projects into manageable, focused interactions with your AI.
* 💰 **Cost & Context Efficient:** Designed to minimize token usage by providing your AI with concise, relevant context for each task via `CURRENT_TASK.md`.
* 🤖 **AI-Assistant Ready:** Crafted for tools like Cline, enabling them to act as true partners in planning and execution.
* ✍️ **Collaborative Documentation:** Encourages the creation and maintenance of key project documents from the start.
* ✨ **Vibe-Driven Development:** Facilitates a more intuitive and flowing interaction with your AI coding partner.

## Prerequisites

* An AI-assisted development tool (e.g., Cline, Cursor) or a Large Language Model (LLM) interface capable of:
    * Reading local Markdown files.
    * Following complex, multi-step instructions.
    * Engaging in conversational Q&A.
    * Ideally, creating and editing files within your project workspace (or providing you with the content to do so).
* Basic understanding of how to interact with your chosen AI assistant.

## How to Use VibeCodeSeed

1.  **Get the Seed:**
    * Clone this repository: `git clone https://github.com/your-username/VibeCodeSeed.git YourNewProjectName` (Replace `your-username` with your actual GitHub username)
    * Or, simply copy the `seed.md` file into the root directory of your new project.

2.  **(Optional) Prepare Your Own Outline:**
    * If you already have a high-level plan or specific requirements, create a `project_outline.md` file in your project root and populate it with your thoughts. The `seed.md` process will then help you refine it.

3.  **Engage Your AI Assistant (e.g., Cline):**
    * Instruct your AI assistant to process the `seed.md` file. For example, in Cline, you might say:
        ```text
        /chat Please process the instructions in the `seed.md` file located in my project root. Let's use it to bootstrap this new project.
        ```

4.  **Follow the AI's Lead:**
    * Your AI assistant will now follow the instructions within `seed.md`.
    * If no `project_outline.md` was found, it will ask you a series of questions about your project.
    * If `project_outline.md` was found, it will analyze it and may ask clarifying questions.
    * It will then guide the creation or refinement of `PROJECT_OUTLINE.md`, `PHASE_1_ACTION_PLAN.md`, and the initial `CURRENT_TASK.md`.
    * **Review all generated files carefully.** This is a collaborative process!

5.  **Iterative Development with `CURRENT_TASK.md`:**
    * Once the initialization is complete, `CURRENT_TASK.md` will contain your first actionable task.
    * For all subsequent work, point your AI assistant to `CURRENT_TASK.md` as its primary brief for the current session/task.
    * After completing a task, instruct your AI to:
        1.  Summarize its actions in the "Summary of Last Completed Actions" section of `CURRENT_TASK.md`.
        2.  Suggest the next objective (based on `PROJECT_OUTLINE.md` and relevant `PHASE_X_ACTION_PLAN.md`) in the "Suggested Next Objective" section of `CURRENT_TASK.md`.
    * You then review, accept/modify the new objective, update the "Objective" and "Specific Instructions for Cline" sections, and continue the cycle.

## Understanding `seed.md`

The `seed.md` file orchestrates the initial project setup through a few key phases (as detailed within `seed.md` itself):

* **Phase 1: Project Definition & Outline Creation:** Determines if a `project_outline.md` exists. If not, it guides the AI to ask foundational questions to create one. If it exists, the AI analyzes it and asks clarifying questions. It then helps create a `PHASE_1_ACTION_PLAN.md`.
* **Phase 2: Initialize Task Management System:** Guides the AI to create the `CURRENT_TASK.md` file, populating it with the very first task from the action plan.
* **Phase 3: Handover to User:** Informs you that the setup is complete and explains how to use the `CURRENT_TASK.md` workflow.

## The `CURRENT_TASK.md` Workflow

This is the heart of the VibeCodeSeed methodology for ongoing development:

1.  **Define:** You (with AI's suggestion) set a clear, focused **Objective** in `CURRENT_TASK.md`.
2.  **Reference:** Link to broader context in `PROJECT_OUTLINE.md` or other docs.
3.  **Instruct:** Provide **Specific Instructions** for your AI for that objective.
4.  **Execute:** Your AI helps complete the task.
5.  **Summarize & Suggest:** AI updates `CURRENT_TASK.md` with a summary and suggests the next objective.
6.  **Review & Repeat:** You review, set the next objective, and the cycle continues.

This keeps interactions fresh, focused, and cost-effective.

## Fine-Tuning Your AI Assistant (e.g., Cline) for VibeCodeSeed

While `VibeCodeSeed` provides the workflow structure, you can often enhance the performance and experience by configuring your AI assistant. If you're using a tool like Cline, consider exploring its settings for:

* **Custom Instructions:**
    * **For Planning Mode:** When Cline is processing `seed.md`, `PROJECT_OUTLINE.md`, or suggesting next steps for `CURRENT_TASK.md`, you could set custom instructions that encourage it to:
        * "Think step-by-step and be very methodical in planning."
        * "Prioritize creating clear, actionable, and modular tasks."
        * "When generating plans or outlines, refer extensively to any provided context documents like `PROJECT_OUTLINE.md`."
        * "Ensure all necessary files (like `PROJECT_OUTLINE.md`, `PHASE_1_ACTION_PLAN.md`, `CURRENT_TASK.md`) are explicitly mentioned if they need to be created or updated."
    * **For Acting Mode:** When Cline is working on the "Specific Instructions" within `CURRENT_TASK.md` (e.g., writing code, generating commands), custom instructions could be:
        * "Adhere strictly to the coding standards and best practices discussed (if any)."
        * "Provide concise summaries of actions taken."
        * "Before writing files, confirm the file path and structure."

* **Different Models for Plan vs. Act Modes:**
    * **Planning:** You might configure Cline to use a more powerful and capable LLM (e.g., GPT-4 series, Claude 3 series, or a large local model) during planning phases. This can lead to better quality outlines, more insightful questions, and more robust strategic suggestions.
    * **Acting:** For more routine execution of well-defined tasks from `CURRENT_TASK.md` (like generating a boilerplate function or a simple script), you might use a faster, more cost-effective LLM, or one specifically fine-tuned for coding tasks.

* **Context Management Awareness:**
    * While `VibeCodeSeed`'s `CURRENT_TASK.md` approach is designed to help manage context externally, be aware of your AI assistant's own context length limitations and any internal tools it offers for managing conversation history or summarizing previous interactions if needed.

**Important:**
* The specific ways to set custom instructions or assign different models for planning/acting modes are **tool-dependent**.
* **Always refer to the official documentation for your chosen AI assistant (e.g., Cline's documentation) for the most accurate and up-to-date configuration instructions.**
* Experiment with these settings to find what works best for your projects and the LLMs you have access to.

By thoughtfully configuring your AI assistant, you can make the `VibeCodeSeed` workflow even smoother and more powerful.

## Customization

Feel free to modify `seed.md` to better suit your personal workflow or the types of projects you typically work on. You can change the initial questions, the structure of the generated outlines, or the information included in `CURRENT_TASK.md`.

## Contributing

Feedback, suggestions, and contributions are welcome! Please feel free to open an issue or submit a pull request if you have ideas for improving VibeCodeSeed.

## License

This project is licensed under the MIT License - see the `LICENSE` file for details (You'll need to add a `LICENSE` file with the MIT license text if you choose this). Consider creating one on GitHub or copying the text from [opensource.org/licenses/MIT](https://opensource.org/licenses/MIT).

---

Happy Vibe Coding! ✨
