# The Six File Context System :memo:

# This idea is far from vibe coding! You need to have a solid understanding of software development and the tools you need in order to build something scalable and maintanable.
# Work in progress! :heavy_exclamation_mark:

## Introduction

The six file context system is a software development strategy. It involves heavy planning and careful use of AI tools in order to achieve the best results with the least amount of propmts, avoiding AI mistakes and creating a workflow that lets you track and monitor the progress of the tasks given to the AI. This helps create a sustainable application with a maintainable codebase and extreme clarity for the developers.

## Goal

The main goal here is to build scalable full-stack applications in a fast and timely manner. The main focus will be on the initial planning and decision making, along with assigning tasks to the AI, via prompts, monitoring its actions and code, as well as tracking the progress of the app development process.

## Prerequisites

As mentioned above, this strategy consists of planning the whole application's purpose, choosing the tech stack, establishing the app's architecture, declaring ai-workflow rules and code standards. Connecting an AI (like Github Copilot, Claude, or other) to your codebase and code editor is essential in order for this to work. I personally use VS Code with Claude. The AI will read the context files and also track its own progress, by writing in the progress-tracker.md file. More information for each file you can find inside them.

## Steps

### 1. Planning

Open up an AI tool. It could be the AI tool in your code editor or from a browser. Start a conversation with them, discussing your application idea, creating a design, choosing a tech-stack, establishing the architecture and overall getting to know exactly what are the best tools for achieving your goal.

### 2. Creating the six file context system

Since you discussed the whole application with the AI from the last step, they already know what you are building, what you need and how to achieve it. Send them the files from this repo (except the AGENTS.md) and tell them to edit them, matching your app idea. The files are templates with surface info, only letting the AI know what they need to write. The AGENTS.md file should not be changed, unless you wish to improve on it.

### 3. Initial work

Move the files in a context folder inside your application's root. You need to split the whole work into small tasks, like implementing a single module, page, or feature. Keep it simple and concise to avoid letting the AI drift away from the strategy and start making mistakes to fix with additional prompts.

### 4. Development process

The development process consists of the following:

- Create an .md for a task, for example "implement-layout.md"
- Inside the file, write what you need the AI to do. For example "Create the header, by following the mobile-first approach.". After that, write down that the AI should follow the ui-context.md and the code-standards.md. Define the goals of a finished task. Tip: you can even use AI to write it down, if you wish.
- Send the file as a prompt and tell the AI to start implementing and update the progress-tracker.md
