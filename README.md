# My AI Product Development Toolkit

Welcome! This is my personal collection of product development prompt templates, designed to help me think, plan, and create better product documentation from a Product Manager's point of view.

This project started as a fork of the excellent [AI Product Development Toolkit](https://github.com/TechNomadCode/AI-Prompt-Library) by TechNomadCode. I'm grateful for the solid foundation they provided, and I've adapted it to fit my specific workflow.

## About This Repository

As a Product Manager, I'm always looking for ways to streamline the process of turning a raw idea into a set of clear, actionable documents. I created this toolkit to help me:

*   **Structure My Thinking:** These prompts guide me through the critical questions needed to define a product.
*   **Create a Consistent Workflow:** I can move from a high-level idea to a detailed spec in a repeatable way.
*   **Generate Foundational Documents:** The output gives me the PRDs, UX flows, and MVP plans I need to kick off a project.
*   **Stay Tool-Agnostic:** The goal is to produce great documentation first. The generated documents can then be used by any team, in any tool, to start building.

## The Guided Conversational Approach

What I love about these prompts is their **user-centered, guided conversational design**:

*   **An Interactive Process:** Instead of trying to get everything in one shot, these templates guide an AI model through an iterative conversation with me.
*   **Structured Questioning:** The AI asks targeted questions about specific parts of the project, helping me build a comprehensive document piece by piece.
*   **Built-in Checkpoints:** The prompts instruct the AI to check in with me regularly, making sure its understanding is aligned with my vision before moving on.
*   **Contextual Analysis:** The workflow is designed so that later steps use the documents from earlier steps (like using a PRD to define an MVP), ensuring consistency.
*   **Adaptive Guidance:** The prompts help me think through aspects I might have missed, while letting me keep full control over the final direction.

This approach gives me the best of both worlds: the AI's power to provide structure and ask smart questions, combined with my own subject matter expertise and final say.

## My Workflow: From Idea to Specification

I use this library sequentially to produce a full suite of specification documents. My typical workflow looks like this:

1.  **Define the Product Vision (PRD):** I start with my raw ideas and use the `PRD/Guided-PRD-Creation.md` prompt to generate a structured **Product Requirements Document (PRD)**.
2.  **Define the User Experience (UX):** With the PRD in hand, I use the `UX-User-Flow/Guided-UX-User-Flow.md` prompt to create detailed **UX Specifications**.
3.  **Define the MVP Concept:** Next, I use the `MVP-Concept/Guided-MVP-Concept-Definition.md` prompt with my PRD (and optionally UX Specs) to define a focused **MVP Concept Description**.
4.  **Plan the MVP Development:** I use `MVP/Guided-MVP.md` (or the `Ultra-Lean-MVP/...` version for speed) with the PRD and MVP Concept to create a detailed **MVP Development Plan**.
5.  **Plan the Testing:** Finally, I use the `Testing/Guided-Test-Plan.md` prompt with the MVP features to outline a comprehensive **Test Plan**.
6.  **Hand-off to the Team:** With these documents, I have a solid foundation to bring to my design and engineering teams. They have the clarity they need to start prototyping, designing, and building.

## Repository Navigation

This repository is organized into topical folders containing the specialized prompts:

*   **PRD**: Template for creating comprehensive Product Requirements Documents.
*   **UX-User-Flow**: Template for translating PRDs into detailed UX Specifications.
*   **MVP-Concept**: Template for defining the focused MVP Concept (scope, hypothesis, features).
*   **MVP**: Template for developing detailed MVP development plans based on the concept.
*   **Ultra-Lean-MVP**: A faster alternative for defining core MVP build specifications.
*   **Testing**: Template for creating thorough test plans for software quality assurance.

```
⚠️ The readme files in each folder contain crucial details on how to use each specific prompt – don't ignore them! ⚠️
```

[PRD](PRD/README.md)

[UX-User-Flow](UX-User-Flow/README.md)

[MVP-Concept](MVP-Concept/README.md)

[MVP](MVP/README.md)

[Testing](Testing/README.md)

[Ultra-Lean-MVP](Ultra-Lean-MVP/README.md)

**General Usage Notes:**

*   **Browse:** Head to the folder for the step you're on.
*   **Copy & Adapt:** Copy the prompt text from the `.md` file. It's crucial to replace all placeholders like `[ <<< PASTE ... HERE >>> ]` or `[example]` with your project details.
*   **Engage:** Paste your adapted prompt into your AI tool of choice. Answer the AI's questions thoughtfully—your responses are key.
*   **Confirm:** Keep an eye out for the AI's check-in points to make sure the output is on track.
*   **Iterate:** Continue the conversation until you have a solid draft of the document you need.

## Model Compatibility

These prompts were developed with large context window models in mind (like Google Gemini, GPT-4, Claude 3), as they need to maintain context through long conversations. For best results when generating final document drafts, I've found it helps to use a low temperature setting (0.2-0.5) to get a more factual, focused output.

## License

You are generally free to use, adapt, and share these prompts. See the `LICENSE` file for more details.

## Disclaimer

AI models and their outputs can be unpredictable. These prompts are starting points and will likely require some tweaking to get exactly what you want. Always review and verify AI-generated content. Your own expertise and strategic decision-making are the most important part of the process!