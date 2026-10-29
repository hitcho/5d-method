---
name: 5d-method
description: Runs work through the five stage 5D Method (Define, Design, Develop, Deploy, Drive), keeping a record of every run so later changes can find what was built and how. Use when starting or continuing a project, feature or change, or when the person says "use 5D".
---

# The 5D Method for AI

Follow `AGENTS.md` at the project root. It holds the rules and where things live. Use `docs/stages.md` for what each stage must produce and `docs/QUESTIONS.md` for the questions to ask in Define and Design.

Start or resume like this:

1. Read `AGENTS.md`, `5D.md` and the current run folder under `runs/`.
2. For new work, create the next run from `runs/_template/` and add it to the index in `5D.md`.
3. For a change to something already built, find the run that built it in `runs/*/changes.md`, read it, and start a new run that builds on it.
4. Work the current stage. Stop at each gate and wait for the owner's explicit approval where the rules require it.
