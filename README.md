# Enrollment Ledger — Student Registration System

A responsive Student Registration System built with **HTML, CSS, Bootstrap 5, and vanilla JavaScript** for Task 08 (JavaScript DOM & Form Validation Project).

## Features

- Registration form for Full Name, Email Address, Phone Number, and Course Name
- Real-time client-side validation with inline error messages
- Submission blocked until every field is valid
- New students are added to a table ("the ledger") with an auto-generated roll number
- **Edit** button loads a record back into the form for updating
- **Delete** button removes a record (with a confirmation prompt)
- Data persists across page reloads via `localStorage`
- Fully responsive layout (Bootstrap grid + custom CSS), down to mobile widths

## Project Structure

```
├── index.html        # Markup for the form and records table
├── css/
│   └── style.css      # Custom "registrar's ledger" visual design
├── js/
│   └── script.js       # Validation, state management, rendering
└── README.md
```

## Running Locally

No build step is required. Either:

1. Open `index.html` directly in a browser, or
2. Serve the folder locally, e.g.:
   ```bash
   npx serve .
   ```

## Validation Rules

| Field | Rule |
|---|---|
| Full Name | Required, 3+ characters, letters/spaces/`.'-` only |
| Email | Required, standard `name@domain.tld` format |
| Phone | Required, 7–15 digits, optional leading `+` |
| Course Name | Required, 2+ characters |

## Deployment

This is a static site, so it deploys directly to **Netlify** or **Vercel** with no build command:

- **Netlify:** Drag-and-drop the project folder onto [app.netlify.com/drop](https://app.netlify.com/drop), or connect the GitHub repo (build command: none, publish directory: `/`).
- **Vercel:** Import the GitHub repo at [vercel.com/new](https://vercel.com/new) and deploy with the default static settings.

## Live Links

- GitHub Repository: _add link here_
- Live Deployment: _add link here_
