# Sydney Law School Cogniti Agent Hub

A self-contained GitHub Pages site bringing together Sydney Law School Cogniti agents and practical resources for legal education.

## Public site

https://staffordlumsden.github.io/sydney-law-cogniti-agents/

## Current tools represented

- **LexiDraft** — legal-writing feedback and revision for Honours and selected capstone contexts.
- **ChatGPT 5.4 for Sydney Law School** — the current general-purpose staff Cogniti agent for low-risk teaching, curriculum and administrative tasks.
- **Unit Outline Helper** — ULO, assessment-summary and curriculum-alignment support for Sydney Curriculum (AKARI).
- **AI Student Support Chatbot** — a related staff-support navigation tool.

## Local resource library

All supporting guidance is stored within this repository and has a matching web-readable page under `resources/`.

- `resources/lexidraft.html`
- `resources/chatgpt-5-4-quick-start.html`
- `resources/build-a-rubric.html`
- `resources/creating-legal-scenarios.html`
- `resources/canvas-qti-quiz.html`
- `resources/unit-outline-helper.html`
- `resources/curriculum-mapping-methodologies.html`
- `resources/ai-student-support-chatbot.html`

Markdown source versions are stored alongside the HTML pages so the guidance is readable directly in GitHub as well as on GitHub Pages.

## Current-version policy

Earlier supplied materials referred to **ChatGPT4o** and, in places, **o3-mini**. The current general-purpose staff guidance has been updated to **ChatGPT 5.4 for Sydney Law School** while preserving the useful workflows in the source material.

The supplied Unit Outline Helper guide also identified an earlier ChatGPT4o configuration. Because the current underlying model for Unit Outline Helper is not stated in the supplied materials, the updated resource does **not** invent a replacement model name; it refers to the current tool as **Unit Outline Helper**.

## External-link policy

Documentation and supporting resources do not depend on Notion, Canvas, SharePoint or other external resource pages. The only outbound links intentionally retained on the main site are links that **launch the actual Cogniti tools** (and the Student Support chatbot), rather than links to supporting documentation.

## Theme

The site uses **light mode by default** with an accessible light/dark toggle in the header. A user-selected theme is persisted locally in the browser and is shared across the hub and local resource pages.

## Site structure

- `index.html` — responsive hub page
- `assets/` — supplied agent artwork
- `resources/` — current local HTML and Markdown guidance
- `DESIGN.md` — design-system specification
- `.nojekyll` — serves the site as plain static content

## GitHub Pages

The repository publishes directly from the `main` branch, root folder (`/(root)`). No custom build step is required.
