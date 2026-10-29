# Stage by stage

What each stage must produce, and where it goes. Every output lives in the current run's folder under `runs/`. The rules are in `AGENTS.md`.

## 1. Define

Use `docs/QUESTIONS.md`. Ask in small batches, only what is not already answered, and record each answer in `run.md` straight away.

Produce, in `run.md`:
- The brief in plain words
- `Builds on:` the earlier run or runs this changes, or none
- Objectives and success measures
- What is out of scope
- Draft acceptance criteria (what good looks like)
- Exception triggers (what makes you come back instead of carrying on)

Gate: is this the right problem to solve? The owner approves.

## 2. Design

Design what you will build and play it back in the person's own words. Use mock ups, flows or structure where they help. Do not build the product, but mock ups and sketches are fine. Make the acceptance criteria final, concrete and testable. Propose the work split.

Produce `build-pack.md`: everything needed in one place so a single agent, or several agents each with their own part, could build from it alone. This is the last stage where you ask questions.

Gate: is the design ready to build? The person signs off that you have understood them and have everything you need.

## 3. Develop

Build from the build pack. Do not ask questions. Create the code, graphics, content and configuration the pack calls for and test as you go. If an agreed exception trigger fires, stop and come back with what happened and the options. Otherwise carry on.

When finished, fill in `changes.md`:
- Every file added, changed or removed, why, and which criterion it serves
- Each acceptance criterion as pass or fail with its evidence
- What depends on what you built, and what to be careful of when changing it later
- The commit or commits, and how to reverse the run

Gate: does it meet the acceptance criteria? If every criterion passes, it is done and moves to Deploy. If any fails, say so plainly and fix it, or raise it as an exception. Done means it matches the criteria, no more and no less.

## 4. Deploy

Show the stakeholder the results against the criteria. Roll out only after they sign off by name. Have a way to roll back. If they refuse, or it does not match or does not work, abort, record what failed and why, and start again from Define. When it is live and working, declare done done and record the date in `run.md`.

Gate: is it ready to go live? The stakeholder approves.

## 5. Drive

Start only after done done. Fill in `drive.md`: a checklist of how we check this is any good. Include golden hour checks straight after go live (is it working, are people getting through, are there errors) and measures over time against the Define objectives (what, how often, who reads them). Record what was learned, and write the next improvement ready to enter Define as a new run.

Gate: is it delivering the expected value?

When all five stages are complete, close in this order:

1. Set the current run's status in its `run.md` to `done done`
2. Update `5D.md`: change that run's Stage column to "Drive" and Status to `done done`
3. If this was the latest/current run, update the header line under "Project:"
4. Add: "All five stages complete - ready for next task or review."
5. Never skip step 2. The central index is how every future run knows what exists.

Status values (use exactly these): not started, in progress, awaiting approval, approved, changes requested, stopped, aborted, done done. No synonyms.

## Handoffs

Before moving on, add the handoff to `handoffs.md`: the output, the decisions made, and what the next stage can rely on. Add the decision to `decisions.csv`: date, stage, decision, owner, evidence.

## Be a partner, not a gatekeeper

Keep it light. One short summary at each gate. Ask the fewest questions that remove real risk, and ask them early, so the person can step back while you build. When new information breaks an earlier decision, say which stage it belongs to and ask whether to reopen it. Do not quietly patch it.
