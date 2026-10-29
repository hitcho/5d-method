# Directing your AI with 5D

Most agent workflows have two modes: plan, then act. Five stages is closer to how real work goes, and it keeps you in the driving seat.

| Plan and act | The 5D Method |
| --- | --- |
| Plan | Define, then Design (you are in the room) |
| Act | Develop (the AI alone, headless) |
| Nothing | Deploy (you sign off), then Drive (you measure) |

The two stages people skip are the ones after the build: getting it live safely, and checking it delivers value. The two before it are where the agent most often runs off in the wrong direction.

Moving from doing to directing means you decide at each gate. The agent does the work between gates. You are not removed from the process, and you are not buried in it either.

## Start from this repository

Clone it, or use it as a template on GitHub, and work inside it. `AGENTS.md` is read automatically by Codex, Cursor, Copilot, Windsurf and most coding agents, and `CLAUDE.md` hands the same file to Claude Code. Nothing to copy, and one set of rules.

Already have a project? Bring in `AGENTS.md`, `CLAUDE.md`, `5D.md`, `docs/` and `runs/`. They have no dependencies.

Then say: "Use 5D. Here is what I want to achieve: ..."

## How a run goes

1. The agent reads `AGENTS.md`, `5D.md` and the current run under `runs/`, so a new session, a new tool or a new teammate picks up exactly where things stand.
2. In Define and Design it asks questions, designs, plays it back and builds a single build pack. You sign off when it has understood you.
3. Develop runs headless. The agent asks nothing and returns only on an exception you agreed, or when every acceptance criterion has evidence.
4. The stakeholder signs off at Deploy, and a failed deploy goes back to Define.
5. The agent cannot approve Define, Design or Deploy itself. Sub agents cannot either.
6. Everything is kept in a folder for that run, and the work is committed with the run number, so the history shows every gate, who approved it and when.

## Changing something later

Ask an AI to change something finished and it usually has no idea how it was built, which files belong together or what was decided. Here, a change is a new run that builds on the old one. Before touching anything, the agent searches `runs/*/changes.md` for the file or feature, reads what the earlier run decided and which files it touched, and changes only what the new brief covers. Because each run records its commits and how to reverse it, you can also undo a run without untangling the rest. See `examples/0001-contact-form/` for what that record looks like.

## No repository?

If you are in a chat assistant with no access to your files, paste the prompt in `prompts/00-start-here.md`. It is a short version of the rules, and the assistant keeps a running record that you save yourself.

## What this is and is not

It is instructions plus a written record, so the agent and the human share one picture of the work. It is not a technical lock. A determined agent or a rushed human can still ignore it. The record makes that visible, and reviewing `runs/` in a pull request catches it.
