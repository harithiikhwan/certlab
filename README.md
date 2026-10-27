# CertLab

CertLab is a mobile-first educational web application prototype for learning, practising, and tracking certification-related content. The project is built as a static front-end using HTML, CSS, and vanilla JavaScript.

## Startup screen

[`startup.html`](./startup.html) is the application's initial loading screen. It:

- Displays the CertLab logo and a loading progress bar.
- Animates progress from `0%` to `100%` over five seconds.
- Stores `startupDone` in `sessionStorage` when loading finishes.
- Redirects the user to [`login.html`](./login.html?from=startup).
- Uses accessible status text through `role="status"` and `aria-live="polite"`.

The screen's visual styling is defined in [`startup.css`](./startup.css).

## Features

The wider prototype includes pages for:

- User login, registration, password recovery, and password reset.
- Course information and course enrolment.
- Notes, video notes, self-notes, and a learning library.
- Exercises and tests.
- Certificates and user profile management.
- Terms and conditions.

## Project structure

| File or group | Purpose |
| --- | --- |
| `startup.html` | Initial loading screen and redirect logic |
| `startup.css` | Loading screen layout and styling |
| `login.html` | Login page shown after startup |
| `*.html` | Static application pages and screens |
| `*.css` | Page-specific stylesheets |
| `exercise.js` | Exercise page interactions |
| `test.js` | Test page interactions |
| `CTU.mp4`, `1.jpg` | Multimedia and image assets |

## How to run

Because this is a static web prototype, no build step or package installation is required.

### Option 1: Open the file directly

Open [`startup.html`](./startup.html) in a modern web browser.

### Option 2: Use a local development server

Running a local server is recommended so that all pages and assets behave consistently. For example, with VS Code, install the **Live Server** extension, right-click `startup.html`, and select **Open with Live Server**.

The application will load the startup screen and then navigate to the login page automatically.

## Technologies

- HTML5
- CSS3
- Vanilla JavaScript
- Browser `sessionStorage` API

## Browser support

Use a current version of Chrome, Edge, Firefox, or Safari with JavaScript enabled.

## Notes

This repository is a front-end prototype for a Human-Computer Interaction group project. Authentication, form submission, data persistence, and backend services are not connected to a production system.

## License

This project is intended for educational and demonstration purposes.
