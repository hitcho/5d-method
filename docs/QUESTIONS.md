# Question bank

Questions belong in Define and Design only. After Design is signed off, ask nothing, so the build can run headless.

Ask only what is not already answered. Before asking, read the Answers section of the current run's `run.md` and the standing answers in `5D.md`. Never ask the same thing twice. Ask in small batches of three to five, and record every answer in the current run's `run.md` the moment it is given.

## Standing questions (ask once, reuse everywhere)

Saved under Standing answers in `5D.md`, so every run in the project starts with them already answered. Confirm them on later runs instead of re-asking.

- Who approves Define and Design by default?
- Who is the stakeholder who signs off Deploy?
- Preferred stack, hosting and tools?
- Brand: name, colours, tone, anything that must not change?
- Accessibility, privacy and security rules that always apply?

## Define

- What do you want, in your own words?
- Who is it for, and what do they do today instead?
- What does success look like, and how will we measure it?
- What is out of scope?
- What does good look like at the end? List what must be true, as plain checks. These become the acceptance criteria.
- When must I stop and come back to you instead of carrying on? Examples: cost above a limit, a change to scope, a security risk, a choice only you can make. These become the exception triggers.
- Deadline, budget and constraints?

Website or web app, add: What is the one action a visitor or user must take? Where does the content or data come from? Does it need accounts, payments or personal data?

## Design

Play back what you understood first, then ask only what is still open.

- Do the mock ups, flows or structure match what you pictured?
- Which parts come first, and which wait?
- Who does what: users, roles, owners?
- What are the main risks, and what controls will we use?
- Stack, hosting, domain and integrations?
- Are the acceptance criteria now specific enough to test?
- Is there anything you assumed I already knew?

Website or web app, add: Pages or screens and how people move between them. Look and feel, with an example you like. Data model. Where secrets and keys live. Accessibility and performance targets. Browsers and devices. How errors and empty states should behave.

Finish by asking: Am I missing anything I need to build this on my own? Only when the answer is no does the person sign off.

## Develop

No questions. If an exception trigger fires, stop and report what happened, the options and your recommendation.

## Deploy

Not questions, a sign off. Show the results against the acceptance criteria and ask the stakeholder: Is it ready to go live? If not, what failed?

## Drive

- Which golden hour checks run straight after go live?
- Which measures from Define will we check over time, how often, and who reads them?
- What would make us change course?
- What is the next improvement, ready to enter Define?
