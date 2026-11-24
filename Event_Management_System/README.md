<div align="center">

# 🎟️ EduFest — Event Management System

### A campus event discovery and registration portal concept

[![HTML5](https://img.shields.io/badge/HTML5-structure-orange?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-styling-blue?logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-vanilla-yellow?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

[Home](./Html/index.html) · [Register](./Html/register.html) · [Dashboard](./Html/dashboard.html) · [Contact](./Html/contact.html)

</div>

---

## 📖 Overview

**EduFest** is a frontend concept for a campus event portal. Its pages present an event-focused landing experience and separate interfaces for registration, a participant dashboard, and contact/feedback interactions. The source includes local event imagery, page-specific stylesheets, and JavaScript for browser-side interactions.

This repository contains the frontend implementation only. It is not connected to a production event service or backend API.

## ✨ Pages and features

| Page | Link | What it covers |
|---|---|---|
| **Home** | [index.html](./Html/index.html) | Event portal landing page, event cards, search/filter interactions, carousel behavior, and theme controls. |
| **Registration** | [register.html](./Html/register.html) | Event registration form and browser-side registration handling. |
| **Dashboard** | [dashboard.html](./Html/dashboard.html) | Participant-facing dashboard view that reads browser-stored registration data. |
| **Contact** | [contact.html](./Html/contact.html) | Contact/feedback forms and FAQ search interactions. |

### Interface details

- Event card imagery stored in the local `images/` directory.
- Carousel behavior implemented in `js/carousel.js`.
- Theme preference handling implemented in `js/theme.js`.
- Registration and dashboard scripts use browser LocalStorage for the demonstration flow.
- Font Awesome and Tabler icon assets are referenced by the HTML pages.

## 🧰 Technology stack

- **HTML5** — page structure and forms.
- **CSS3** — shared styles and page-specific styling.
- **Vanilla JavaScript** — search, carousel, theme, form, and dashboard interactions.
- **LocalStorage** — browser-local registration and theme data where implemented.
- **Font Awesome / Tabler Icons** — iconography loaded from external resources.

## 🗂️ Project structure

```text
Event_Management_System/
├── README.md
├── Html/
│   ├── index.html          # Event portal home
│   ├── register.html       # Registration form
│   ├── dashboard.html     # Participant dashboard
│   └── contact.html        # Contact and feedback
├── styles/
│   ├── style.css           # Shared styling
│   ├── register.css        # Registration page styles
│   ├── dashboard.css       # Dashboard page styles
│   ├── contact.css         # Contact page styles
│   └── carousel.css        # Carousel styles
├── js/
│   ├── app.js              # Home page interactions
│   ├── carousel.js         # Carousel behavior
│   ├── register.js         # Registration behavior
│   ├── dashboard.js        # Dashboard behavior
│   ├── contact.js          # Contact and FAQ behavior
│   └── theme.js            # Theme preference behavior
└── images/                 # Event cards, logo, and visual assets
```

## 🚀 Run locally

1. Clone the repository and open `Event_Management_System` in VS Code.
2. Open [`Html/index.html`](./Html/index.html).
3. Start the page with the **Live Server** extension.
4. Navigate to registration, dashboard, and contact pages using the site's navigation.

Because the HTML files are inside `Html/` and the asset folders are siblings, local asset references from those pages should begin with `../`. For example:

```html
<link rel="stylesheet" href="../styles/style.css">
<script src="../js/app.js"></script>
<img src="../images/card1.jpg" alt="Event">
```

Keep links between pages in the same `Html/` directory relative to that directory, such as `register.html` or `dashboard.html`.

## 💾 Browser storage and data scope

Registration and theme behavior use browser-side storage where implemented. Stored values are local to the browser profile and are not synchronized to a server. The repository does not include an event API, authentication service, payment gateway, or production database. Do not use this demo to collect real personal or payment information.

## ⚠️ Known implementation note

The current `Html/register.html` source references `js/script.js`, but the project’s `js/` directory does not contain a `script.js` file. The registration-specific script present in the project is `js/register.js`. If the browser Network or Console panel reports a 404 for `script.js`, remove that unused script tag from `register.html` or add the intended file before relying on the page.

External icon libraries are loaded from CDNs, so an internet connection may be required for those icons.

## 🔗 Source on GitHub

- [Browse EduFest project files](https://github.com/shubhamthakur9771/Frontend-Projects/tree/main/Event_Management_System)
- [Home page HTML](https://github.com/shubhamthakur9771/Frontend-Projects/blob/main/Event_Management_System/Html/index.html)
- [Registration page HTML](https://github.com/shubhamthakur9771/Frontend-Projects/blob/main/Event_Management_System/Html/register.html)
- [Stylesheets](https://github.com/shubhamthakur9771/Frontend-Projects/tree/main/Event_Management_System/styles)
- [JavaScript modules](https://github.com/shubhamthakur9771/Frontend-Projects/tree/main/Event_Management_System/js)

---

[← Back to all frontend projects](../README.md)
