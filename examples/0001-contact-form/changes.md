# Changes

## Files

| File | Added, changed or removed | Why | Criterion |
| --- | --- | --- | --- |
| `contact.html` | changed | Added the form markup below the address block | 1, 2, 4 |
| `css/contact.css` | added | Form styles, with a 375px layout | 4 |
| `api/contact.js` | added | Validates the fields, drops honeypot submissions, sends the email | 1, 2, 3 |
| `.env.example` | changed | Added `CONTACT_TO` and `MAIL_API_KEY` names, no values | 1 |

## Evidence

| # | Criterion | Result | Evidence |
| --- | --- | --- | --- |
| 1 | Valid submission emails sales | pass | Test email received at 10:14, message id in the mail log |
| 2 | Empty email shows an error | pass | Screenshot `evidence/empty-email.png`, no email sent |
| 3 | Honeypot sends nothing | pass | Mail log shows no send for the test submission |
| 4 | Works at 375px | pass | Screenshot `evidence/phone.png` |

Exceptions raised: none.

## What depends on this

The recipient comes from the `CONTACT_TO` environment variable, not from the code. Anything that changes the Contact page layout should keep the form's `id="contact-form"`, because `css/contact.css` and `api/contact.js` both rely on it.

## Commits

`a1b2c3d` 5D 0001: add contact form markup and styles
`e4f5a6b` 5D 0001: add contact API function

## How to reverse this run

`git revert e4f5a6b a1b2c3d`, then remove `CONTACT_TO` and `MAIL_API_KEY` from the hosting environment.

## Corrections

2026-03-20: the sales inbox moved to hello@example.com. Changed only the `CONTACT_TO` value in the hosting environment. No files changed.
