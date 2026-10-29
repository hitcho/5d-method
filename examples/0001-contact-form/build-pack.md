# Build pack

## Playback

A form on the Contact page with name, email and message. It posts to a small server function that sends one email to the sales inbox. A hidden field catches bots.

## Design

Form below the address block on `contact.html`, same styles as the footer signup. The server function lives in `api/contact.js` and reads the recipient from an environment variable.

## Acceptance criteria (final)

As in `run.md`, criteria 1 to 4.

## Exception triggers (final)

As in `run.md`.

## Work split

One agent builds all of it.

## Risks and controls

Mail credentials stay in environment variables, never in the repository.
