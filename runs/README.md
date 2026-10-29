# Runs

One folder per run, named `NNNN-short-name`, for example `0007-add-contact-form`. Numbers only go up. Start from `_template/`: copy it, rename it, and add the run to the index in `5D.md`.

| File | What it holds |
| --- | --- |
| `run.md` | Status, owners and approvals, `Builds on:`, the brief, answers, objectives, acceptance criteria and exception triggers |
| `build-pack.md` | The design and everything needed to build it from this file alone |
| `changes.md` | Every file added, changed or removed, why, the evidence for each criterion, the commits and how to reverse the run |
| `decisions.csv` | Date, stage, decision, owner, evidence |
| `handoffs.md` | What each stage passed on |
| `drive.md` | How you check it is any good, and what was learned |

## Why keep them

When you ask an AI to change something finished, it usually has no idea how it was built, which files belong together or what the earlier decisions were. These folders give it that. Before changing anything, it finds the run that built it, reads what was decided and which files were touched, and changes only that.

## Rules for the record

- Never rewrite an old run. If something turns out to be wrong, add a dated correction at the end of the file.
- A change to something already built is a new run with `Builds on:` pointing at the old one.
- Commit each run's work with the message prefix `5D 0007:` so `git log --grep "5D 0007"` finds it, and record the commits in `changes.md`.
