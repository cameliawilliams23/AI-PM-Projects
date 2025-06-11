# AI-PM-Projects
AI Dev Tasks for Cursor 🤖
Welcome to AI Dev Tasks! This repository provides a collection of .mdc (Markdown Command) files designed to supercharge your feature development workflow within the Cursor editor. By leveraging these commands with Cursor's AI Agent, you can systematically approach building features, from ideation to implementation, with built-in checkpoints for verification.

Stop wrestling with monolithic AI requests and start guiding your AI collaborator step-by-step!

✨ The Core Idea
Building complex features with AI can sometimes feel like a black box. This workflow aims to bring structure, clarity, and control to the process by:

Defining Scope: Clearly outlining what needs to be built with a Product Requirement Document (PRD).
Detailed Planning: Breaking down the PRD into a granular, actionable task list.
Iterative Implementation: Guiding the AI to tackle one task at a time, allowing you to review and approve each change.
This structured approach helps ensure the AI stays on track, makes it easier to debug issues, and gives you confidence in the generated code.

Workflow: From Idea to Implemented Feature 💡➡️💻
Here's the step-by-step process using the .mdc files in this repository:

1️⃣ Create a Product Requirement Document (PRD)
First, lay out the blueprint for your feature. A PRD clarifies what you're building, for whom, and why.

You can create a lightweight PRD directly within Cursor:

Ensure you have the create-prd.mdc file from this repository accessible.

In Cursor's Agent chat, initiate PRD creation:

Use @create-prd.mdc
Here's the feature I want to build: [Describe your feature in detail]
Reference these files to help you: [Optional: @file1.py @file2.ts]
(Pro Tip: For complex PRDs, using MAX mode in Cursor is highly recommended if your budget allows for more comprehensive generation.)

Example of initiating PRD creation

2️⃣ Generate Your Task List from the PRD
With your PRD drafted (e.g., MyFeature-PRD.md), the next step is to generate a detailed, step-by-step implementation plan for your AI Developer.

Ensure you have generate-tasks-from-prd.mdc accessible.

In Cursor's Agent chat, use the PRD to create tasks:

Now take @MyFeature-PRD.md and create tasks using @generate-tasks-from-prd.mdc
(Note: Replace @MyFeature-PRD.md with the actual filename of the PRD you generated in step 1.)

Example of generating tasks from PRD

3️⃣ Examine Your Task List
You'll now have a well-structured task list, often with tasks and sub-tasks, ready for the AI to start working on. This provides a clear roadmap for implementation.

Example of a generated task list

4️⃣ Instruct the AI to Work Through Tasks (and Mark Completion)
To ensure methodical progress and allow for verification, we'll use process-task-list.mdc. This command instructs the AI to focus on one task at a time and wait for your go-ahead before moving to the next.

Create or ensure you have the process-task-list.mdc file accessible.

In Cursor's Agent chat, tell the AI to start with the first task (e.g., 1.1):

Please start on task 1.1 and use @process-task-list.mdc
(Important: You only need to reference @process-task-list.mdc for the first task. The instructions within it guide the AI for subsequent tasks.)

The AI will attempt the task and then prompt you to review.

Example of starting on a task with process-task-list.mdc

5️⃣ Review, Approve, and Progress ✅
As the AI completes each task, you review the changes.

If the changes are good, simply reply with "yes" (or a similar affirmative) to instruct the AI to mark the task complete and move to the next one.
If changes are needed, provide feedback to the AI to correct the current task before moving on.
You'll see a satisfying list of completed items grow, providing a clear visual of your feature coming to life!

Example of a progressing task list with completed items

While it's not always perfect, this method has proven to be a very reliable way to build out larger features with AI assistance.
