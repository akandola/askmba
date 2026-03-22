# askmba — Claude Code Instructions

**Session Bootstrap:** Load and internalize `lessons.md` before starting work. Treat every lesson as a hard constraint.

## Working Principles
1. **Ambiguity → Stop and Ask** — Name specific ambiguities and ask clarifying questions
2. **Non-Trivial Work → State Assumptions First** — Explicitly state assumptions before implementing
3. **Inconsistencies → Surface Them** — Ask which takes precedence when conflicts exist
4. **Bad Ideas → Push Back Directly** — State the problem, downside, and propose alternatives

## Project Overview
Static website for ASK MBA Consulting. Single-page HTML/CSS — no framework, no build step.

Tagline: *where your story becomes your super power*

Contact email: anmol@askmbaconsulting.com (footer added to index.html).

## Running Locally
Open `index.html` directly in a browser — no server required.

For GitHub Pages deployment, push to `main` branch. Custom domain configured via repo settings + CNAME file.

## Project Structure
- `index.html` — entire site (HTML + embedded CSS)
- `CLAUDE.md` — this file
- `lessons.md` — environment lessons and constraints
