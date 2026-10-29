# Run 0001: add a contact form

Status: done done
Current stage: Drive
Builds on: none
Started: 2026-03-02

## Owners and approvals

| Stage | Gate owner | Status | Approved on |
| --- | --- | --- | --- |
| 1. Define | Sam Rivera | approved | 2026-03-02 |
| 2. Design | Sam Rivera | approved | 2026-03-03 |
| 3. Develop | evidence | approved | 2026-03-03 |
| 4. Deploy | Priya Shah | approved | 2026-03-04 |
| 5. Drive | Sam Rivera | in progress | |

## 1. Define

### Brief

Visitors to the site have no way to ask a question. Add a contact form to the Contact page that emails the sales inbox.

### Answers

- Where does it go: the existing Contact page, below the address.
- Who receives it: sales@example.com.
- Spam: a hidden honeypot field is enough for now.
- Does it keep a copy: no, email only.

### Objectives and how success is measured

Sales receives an email for every genuine submission, within one minute.

### Out of scope

A CRM connection, file uploads, a thank you email to the visitor.

### Acceptance criteria

| # | Criterion | How it is checked |
| --- | --- | --- |
| 1 | A valid submission sends an email to sales@example.com | Submit on staging, check the inbox |
| 2 | An empty email field shows an error and sends nothing | Submit empty on staging |
| 3 | A submission with the honeypot filled sends nothing | Submit with the hidden field set |
| 4 | The form works on a phone width screen | Check at 375px wide |

### Exception triggers

- The mail service rejects the sender address.
- Anything on the Contact page other than the form would need to change.

## Open items

None.

## Corrections

2026-03-20: the sales inbox moved to hello@example.com. See `changes.md`.
