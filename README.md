# AI Product Development Toolkit (Agnostic Ideation Fork)

Welcome to my personal collection of product development prompt templates! This repository is a fork of the excellent [AI Product Development Toolkit](https://github.com/TechNomadCode/AI-Prompt-Library) by TechNomadCode, and I'm grateful for the solid foundation they provided.

The main idea behind this fork is to make the project as **agnostic as possible**, focusing specifically on the higher-level product ideation and documentation process, independent of any single implementation tool.

## About This Repository

As I use different AI tools, I often find myself designing specific prompts to get desired outputs. This repository is my way of:

*   **Organizing:** Keeping track of prompts that work well.
*   **Reusing:** Quickly finding and adapting prompts for new tasks.
*   **Sharing:** Making useful prompts available (primarily for myself, but maybe helpful to others!).
*   **Learning:** Refining prompts over time and seeing patterns in what works.

## Guided Conversational Approach

What makes these prompts unique is their **user-centered, guided conversational design**:

*   **Interactive Process:** Rather than one-shot prompting, these templates guide AI models through an iterative conversation with you.
*   **Structured Questioning:** The AI asks targeted questions focused on specific aspects of your project, building a comprehensive document piece by piece.
*   **User Confirmation Checkpoints:** The prompts explicitly instruct the AI to verify its understanding and direction with you before moving to new sections or making significant interpretations.
*   **Contextual Analysis:** Many templates use inputs from previous steps (like a PRD for context plus an MVP concept), instructing the AI to cross-reference information for consistency.
*   **Adaptive Guidance:** The templates help you think through aspects you might have missed, while allowing you to maintain control over the final direction.

This approach combines the best of both worlds: AI's ability to provide structure and ask clarifying questions, with your subject matter expertise and decision-making authority.

## How to Use: From Idea to Specification Workflow

This library is designed to be used sequentially to produce a suite of specification documents. My personal workflow with these documents is as follows:

1.  **Define Product Vision (PRD):** Start with your raw ideas and use the `PRD/Guided-PRD-Creation.md` prompt to generate a structured **Product Requirements Document (PRD)**.
2.  **Define User Experience (UX):** Use the `UX-User-Flow/Guided-UX-User-Flow.md` prompt, feeding it the PRD, to create detailed **UX Specifications**.
3.  **Define MVP Concept:** Use the `MVP-Concept/Guided-MVP-Concept-Definition.md` prompt with your PRD (and optionally UX Specs) to define the focused **MVP Concept Description** (scope, hypothesis, features).
4.  **Plan MVP Development:** Use `MVP/Guided-MVP.md` (or `Ultra-Lean-MVP/...` for speed) with the PRD and MVP Concept to create the **MVP Development Plan** or **Build Spec**.
5.  **Plan MVP Testing:** Use the `Testing/Guided-Test-Plan.md` prompt with the MVP features (from Step 3 or 4) to outline the **Test Plan**.
6.  **Generate Implementation Specs:** The generated documents (PRD, MVP, UX, testing) are then processed through a Custom Gemini Gem to generate specs for use with [Github Spec Kit](https://github.com/github/spec-kit).
7.  **Begin Implementation:** I take the output from the previous step into VS Code (or any editor/agent supported by Github Spec Kit) and begin implementation.

## Repository Navigation

This repository is organized into topical folders containing specialized prompts:

*   **PRD**: Template for creating comprehensive Product Requirements Documents.
*   **UX-User-Flow**: Template for translating PRDs into detailed UX Specifications.
*   **MVP-Concept**: Template for defining the focused MVP Concept (scope, hypothesis, features).
*   **MVP**: Template for developing detailed MVP development plans based on the concept.
*   **Ultra-Lean-MVP**: Template focused on rapidly defining core MVP build specifications (alternative to detailed MVP planning).
*   **Testing**: Template for creating thorough test plans for software quality assurance.

```
⚠️ Readme files in each folder contain crucial details – do not ignore them. ⚠️
```

[PRD](PRD/README.md)

[UX-User-Flow](UX-User-Flow/README.md)

[MVP-Concept](MVP-Concept/README.md)

[MVP](MVP/README.md)

[Testing](Testing/README.md)

[Ultra-Lean-MVP](Ultra-Lean-MVP/README.md)

**General Usage Notes:**

*   **Browse:** Navigate to the relevant folder for the step you're on.
*   **Copy & Adapt:** Copy the prompt text from the `.md` file. **Crucially, replace all placeholders** like `[ <<< PASTE ... HERE >>> ]` or `[example]` with your specific project details and inputs from previous steps.
*   **Engage:** Paste the adapted prompt into your AI tool. Answer the AI's questions thoughtfully – your responses guide the process.
*   **Confirm:** Pay attention to the AI's check-in points to ensure the output stays aligned with your vision.
*   **Iterate:** Continue the conversation until the desired document/plan is drafted.

## Model Compatibility

These prompts were developed with large context window models in mind (like Google Gemini, GPT-4, Claude 3), as they need to maintain conversation context throughout potentially lengthy exchanges, often referencing large input documents (like PRDs or UX Specs). For best results when generating final document drafts, consider using a low temperature setting (0.2-0.5) to encourage factual, focused output.

## License

You are generally free to use, adapt, and share these prompts. See the `LICENSE` file for more details.

## Disclaimer

AI models and their outputs can be unpredictable. These prompts are starting points and may require significant modification to achieve your desired results. Always review and verify AI-generated content, especially for accuracy, bias, or appropriateness. Human oversight, strategic decision-making, and technical validation are critical at every step.
