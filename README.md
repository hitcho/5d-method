# The 5D Method for AI

Take the 5D Method. Build your process. Direct your AI.

5D provides the five stages and the structure. You and your AI then build the process together, agreeing the instructions, evidence, stage gates and human approvals.

The method is universal. The process is yours. AI follows your process, not just your prompts.

## The five stages

| Stage | Gate question |
| --- | --- |
| 1. Define | Is this the right problem to solve? |
| 2. Design | Is the design ready to build? |
| 3. Develop | Does it meet the acceptance criteria? |
| 4. Deploy | Is it ready to go live? |
| 5. Drive | Is it delivering the expected value? |

Three rules hold it together. Every gate has one owner. Every handoff says what is passed on. Go as fast as you like, skip none.

## Start in two minutes

Clone this repository, or use it as a template on GitHub, and open it with your AI coding tool. Claude Code, Codex, Cursor, Copilot and Windsurf all pick up the rules from `AGENTS.md` on their own. Then say:

> Use 5D. Here is what I want to achieve: ...

Using a chat assistant with no access to files? Paste [prompts/00-start-here.md](prompts/00-start-here.md) instead.

## What is in here

| Path | What it is |
| --- | --- |
| `AGENTS.md` | The rules, and the one source for them. `CLAUDE.md` points to it. |
| `5D.md` | Your standing answers and an index of every run |
| `runs/` | One folder per run: the brief, build pack, decisions, files changed and how to reverse it |
| `docs/` | How it works, what each stage must produce, and the question bank |
| `prompts/` | A prompt for each stage, for chat assistants |
| `examples/` | A filled in sample run |
| `.claude/skills/` | The same method as a Claude Code skill |

## A record of every run

Each piece of work leaves a folder under `runs/` that says what was asked, what was decided, which files were added, changed or removed, and how to undo it. When you later ask for a change, your AI reads the run that built the thing first, so it changes what you asked for and leaves the rest alone. Read [docs/how-it-works.md](docs/how-it-works.md), then look at [examples/0001-contact-form](examples/0001-contact-form).

## Manifesto

Why 5D exists, what I believe about it, and how we talk about it: [5d.tjhitchens.com/manifesto.html](https://5d.tjhitchens.com/manifesto.html).

## Licence

Prompts, templates and docs are CC BY 4.0. See [LICENSE](LICENSE) and [NOTICE.md](NOTICE.md). The name, logo and artwork are not licensed for reuse.

By Timothy J. Hitchens, Techshin Partners.
