<div align="center">

# 🎟️ EduFest — Event Management System

**A multi-page campus event portal concept**

[Open EduFest Home](./Html/index.html)

</div>

---

## 📖 Overview

EduFest is a frontend event management portal concept for discovering campus activities such as workshops, hackathons, seminars, coding contests and technology festivals.

The project includes dedicated pages for the home experience, event registration, a personal dashboard and contact information.

## ✨ Features

- **Home page:** event portal landing page and event discovery content.
- **Registration page:** event registration interface and client-side form interactions.
- **Dashboard:** personal dashboard concept for registered events and participation details.
- **Contact page:** contact information and interactive page elements.
- **Theme toggle:** light/dark theme interaction.
- **Visual components:** event cards, carousel-related styles and image assets.

## 🧰 Technologies

- HTML5
- CSS3
- JavaScript (Vanilla)
- Font Awesome
- Tabler Icons
- Local browser storage (where used by the frontend scripts)

## 🗂️ Project structure

```text
Event_Management_System/
├── README.md
├── Html/
│   ├── index.html
│   ├── register.html
│   ├── dashboard.html
│   └── contact.html
├── styles/
│   ├── style.css
│   ├── register.css
│   ├── dashboard.css
│   ├── contact.css
│   └── carousel.css
├── js/
│   ├── app.js
│   ├── theme.js
│   ├── register.js
│   ├── dashboard.js
│   ├── contact.js
│   └── carousel.js
└── images/
```

## 🚀 Run locally

1. Open the `Event_Management_System` folder in VS Code.
2. Start Live Server using `Html/index.html`.
3. Open the local URL provided by Live Server.

### Important: fix asset paths before running

The HTML pages are inside `Html/`, while `styles/`, `js/` and `images/` are sibling directories. References such as:

```html
<link rel="stylesheet" href="./styles/style.css">
```

should use:

```html
<link rel="stylesheet" href="../styles/style.css">
```

Likewise, update local image and script references to `../images/...` and `../js/...`. Keep page-to-page navigation links such as `register.html` and `dashboard.html` relative to the `Html/` directory.

## ⚠️ Project scope

This is a frontend project archive. A production-ready event backend, payment integration or hosted database is not included in the provided files.

---

[← Back to all frontend projects](../README.md)
