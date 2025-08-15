```markdown
# AI Prompts for Copilot Agent Scaffold Prompt

This folder contains prompts to help you generate a scaffold prompt for GitHub Copilot Agent. The goal is to turn your detailed User Experience (UX) plans and MVP scope into a starting point for your application's codebase.

## The Prompts

There are two main files here:

1.  **`copilot-scaffold-prompt.md` (The Target)**
    *   **What it is:** This is a detailed blueprint that tells GitHub Copilot Agent exactly what kind of project to create.
    *   **How it's used:** You don't usually fill this out manually. Instead, you use the "Prompt Filler" (see below) to create a completed version of this template, which you then copy and paste into GitHub Copilot Agent.

2.  **`copilot-scaffold-prompt-filler.md` (The Interactive Filler)**
    *   **What it is:** This is an interactive chat prompt you use with a general AI assistant (like Gemini, ChatGPT, Claude).
    *   **What it does:** It guides you through a conversation to automatically fill out the "Target" above. It uses two key pieces of information you provide:
        *   Your detailed **UX Specifications** document (which describes how the whole app should look and work).
        *   Your **MVP Scope Definition** (which lists exactly which features or pages are needed for the *first version* of your app).
    *   **How it's used:** You start a chat with an AI using this prompt, providing your UX Specs and MVP Scope. The AI will ask you questions, referencing your documents, to gather all the details needed for the Target, focusing only on the MVP parts. The final output of this chat is the completed Target, ready for GitHub Copilot Agent.

## How to Use These Prompts

1.  **Have your UX specs & MVP scope ready**
2.  **Use the filler prompt with an LLM to collect your stack choice + feature/pages list**
3.  **Paste the completed scaffold prompt into GitHub Copilot Agent to generate your initial code**
```
