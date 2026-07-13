# poc

Login and signup forms — proof of concept.

## Preview

Two standalone HTML pages with a terminal-themed, split-screen design:
- Left panel: animated boot-sequence terminal, unique per page
- Right panel: the actual form, with live inline validation

![Login form](login-preview.png)
![Signup form](signup-preview.png)

## Files

- `login.html` — sign-in form (teal accent). Validates email format and password length inline; includes a show/hide password toggle.
- `signup.html` — account creation form (amber accent). Adds full name and confirm-password fields, plus a live password-strength meter.

## Design

- Fonts: Space Grotesk (headings), JetBrains Mono (terminal + labels), Inter (body/inputs)
- Fully self-contained — no build step, no dependencies beyond Google Fonts
- Responsive down to mobile (stacks vertically below 820px)

## Status

Front-end only. Form submission currently shows a confirmation alert — not yet wired to a backend API.

## Next steps

- Connect forms to a backend (FastAPI / Django REST) for real auth
- Add JWT-based session handling
- Add unit/integration tests for validation logic
