```markdown
## PRIMARY OBJECTIVE:
Generate a GitHub Copilot Agent scaffold prompt that will create the project's initial files, folder structure, and minimal boilerplate based on the chosen tech stack and MVP feature scope. The scaffold should be stack-agnostic, focus on the MVP surface area, and include clear instructions the Copilot Agent can follow to produce a runnable starter.

---

## MODULE 1: TECH STACK & RUNTIME
* Ask which frontend/backend stack the user prefers (examples):
  - Frontend: React, Next.js, Remix, Vue, Svelte, Solid, Vanilla JS
  - Backend: Node/Express, Fastify, Flask, Django, Rails, Phoenix, Serverless functions
* Language/variants: TypeScript or JavaScript, Python (3.x), Ruby, etc.
* Target runtime/platform: Browser-only SPA, SSR (Next/Remix), Jamstack, Server-rendered, or API-only.
* Deployment target or hosting preferences (Vercel, Netlify, Heroku, Docker, self-host).

---

## MODULE 2: PROJECT METADATA & TOOLING
* Project name and brief description.
* Package manager and build tooling: npm / yarn / pnpm / pip / bundler.
* Repo layout preferences: monorepo (pnpm/workspaces), single repo, or microservices.
* Folder conventions (src/, app/, components/, services/, api/), code style (Prettier/ESLint), license.

---

## MODULE 3: MVP FEATURES, PAGES & ENDPOINTS
* Ask the user to list the minimal set of features, pages, and API endpoints required for the MVP (route + brief purpose). Example:
  - / (Landing): marketing + CTA
  - /dashboard: overview of user data
  - /auth/login, /auth/signup
  - API: POST /api/login, GET /api/items
* For each route/page, ask for the key components or data elements (e.g., list, form, profile card).
* Ask for any required data models (attributes) or minimal fixtures needed for placeholders.

---

## MODULE 4: STYLING & COMPONENT PREFERENCES
* Styling choices: plain CSS, Tailwind, Bootstrap, Chakra, Material, custom design system.
* Component library preferences (if any): shadcn, Radix, Chakra, Vuetify, Headless UI, component-less.
* Global layout conventions: header/footer/sidebar, responsive breakpoints.
* Accessibility baseline expectations (WCAG level), if any.

---

## MODULE 5: TESTING, CI & DEV WORKFLOWS
* Testing framework preferences: Jest, Vitest, React Testing Library, PyTest, RSpec.
* Basic CI expectations: run tests on push, linting, basic build step, optional deployment action.
* Local dev script expectations: start, build, test, lint commands.

---

## MODULE 6: FINAL SCAFFOLD PROMPT & EXAMPLE
* After collecting the answers above, synthesize them into a single Copilot Agent scaffold prompt. The prompt should instruct Copilot to:
  - Create the project using the chosen stack and language.
  - Generate a minimal folder structure and key files for each in-scope route/page and API endpoint.
  - Add example components/views with placeholder data and simple styles per the chosen styling option.
  - Add minimal tests and a CI workflow that runs tests and lints.
  - Create a README with usage instructions (how to run, test, build).

Example scaffold prompt template (fill placeholders from Modules 15):

```
Scaffold a [STACK] project named "[PROJECT_NAME]" using [LANGUAGE] and [PACKAGE_MANAGER]. Target runtime: [RUNTIME].

Include the following pages/endpoints for the MVP:
- [ROUTE 1]: [brief purpose and key components]
- [ROUTE 2]: [brief purpose and key components]

Create a minimal folder structure: [list folders]. For each page, add presentational components in a `components/` folder and simple placeholder data.

Styling: use [STYLING_CHOICE] and apply a simple global layout with [HEADER/FOOTER/SIDEBAR as chosen].

Add basic tests using [TEST_FRAMEWORK] and a CI workflow that runs `install`, `lint`, and `test` on push.

Provide a README with instructions: how to install, run dev server, run tests, and build for production.

Do not implement complex business logic or external integrations; use placeholder data and TODO comments where appropriate. Keep the code minimal but runnable.
```

---

## HOW TO USE
* Run the `copilot-scaffold-prompt-filler.md` interactive filler to collect answers module-by-module.
* Paste the completed scaffold prompt into GitHub Copilot Agent (or the Copilot CLI/IDE integration you use) to generate the initial project scaffold.
* Review generated code, replace placeholders, and iterate.
```
