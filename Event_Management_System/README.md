<div align="center">

# 🎟️ EduFest — Event Management System

### A campus event portal concept for event discovery, student registration, and participant dashboards

[![Live Demo](https://img.shields.io/badge/Live_Demo-Open_EduFest-0A7F45?logo=vercel&logoColor=white)](https://edu-fest-theta.vercel.app/)
[![HTML5](https://img.shields.io/badge/HTML5-Structure-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-Styling-1572B6?logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla-F7DF1E?logo=javascript&logoColor=222222)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

[Live Home](https://edu-fest-theta.vercel.app/) · [Register](https://edu-fest-theta.vercel.app/Html/register.html) · [Dashboard](https://edu-fest-theta.vercel.app/Html/dashboard.html) · [Contact & FAQs](https://edu-fest-theta.vercel.app/Html/contact.html)

[← Back to Frontend Projects](../README.md) · [View GitHub source](https://github.com/shubhamthakur9771/Frontend-Projects/tree/main/Event_Management_System)

</div>

---

## 📌 Project overview

**EduFest** is a campus event discovery and registration portal concept. It presents technical and non-technical events through a featured landing page, event cards, category filters, search, and a registration flow. A participant dashboard displays registrations stored in the current browser, while the contact page includes message, feedback, and FAQ interfaces.

The project is implemented as a multi-page static frontend using HTML, CSS, and vanilla JavaScript. Its registration and preference data are handled in the browser; the current repository does not include a server-side event platform.

> **Live application:** [https://edu-fest-theta.vercel.app/](https://edu-fest-theta.vercel.app/)

## 🖥️ Live application pages

| Page | Live link | Purpose |
|---|---|---|
| Home | [Open home ↗](https://edu-fest-theta.vercel.app/) | Featured events, event discovery, search, filters, and carousel. |
| Registration | [Open registration ↗](https://edu-fest-theta.vercel.app/Html/register.html) | Collect participant details and register for a selected event in browser storage. |
| Participant dashboard | [Open dashboard ↗](https://edu-fest-theta.vercel.app/Html/dashboard.html) | Display registrations associated with the email stored for the current browser session/profile. |
| Contact & feedback | [Open contact page ↗](https://edu-fest-theta.vercel.app/Html/contact.html) | Contact and feedback form interfaces, star rating, and searchable FAQs. |

## ✨ Features and modules

### 1. Event discovery homepage

- Featured event carousel with previous/next controls, slide indicators, autoplay, and touch/keyboard interactions.
- Event cards with event category, date, location, description, and price/seat information as presented in the interface.
- Search events by title.
- Filter event cards by category, including Coding, Workshop, and Seminar.
- Sort event cards by newest or oldest date.
- Countdown display for event dates.
- Event registration links from featured events and event cards.
- Theme toggle with browser-stored preference.

### 2. Event registration

- Registration form for participant name, email, phone, college, event, gender, and date.
- Frontend validation for required fields.
- Event selection can be prefilled when an event was selected from the home page.
- Registration records are stored in LocalStorage.
- Duplicate registration check for the same email and event title.
- After successful registration, the page navigates to the participant dashboard.

### 3. Participant dashboard

- Reads registration records from browser storage.
- Filters records using the current stored participant email.
- Displays participant name and email.
- Shows the total number of registrations for that email.
- Renders cards for the participant's registered events, including event title, category, date, and location.
- Redirects to registration if no matching registration is available in the current browser storage.

### 4. Contact, feedback, and FAQ centre

- Contact form with first name, last name, email, subject, and message validation.
- Feedback form with event selection, written feedback, and a five-star rating interaction.
- Client-side success states after valid form submission.
- FAQ accordion interactions to expand and collapse answers.
- FAQ search to filter questions by text and keywords.
- Contact information and support links presented in the page interface.

### 5. Shared interface behavior

- Theme switching between light and dark presentation, with the preference stored in LocalStorage.
- Shared navigation between the four pages.
- Local event imagery and branding assets.
- Font Awesome and Tabler icon resources referenced by the HTML pages.

## 🧰 Technology stack

| Technology | Role in this project |
|---|---|
| HTML5 | Page structure, navigation, event cards, and forms. |
| CSS3 | Shared design system and page-specific styling. |
| Vanilla JavaScript | Search, filtering, sorting, carousel, validation, registration, dashboard rendering, and FAQ interactions. |
| LocalStorage | Browser-local registrations, selected event data, current participant email, and theme preference. |
| Font Awesome | Interface icons loaded from a CDN. |
| Tabler Icons | Additional icon resources loaded from a CDN. |

## 🗂️ Project structure

```text
Event_Management_System/
├── README.md
│
├── Html/
│   ├── index.html          # Event discovery homepage
│   ├── register.html       # Participant registration form
│   ├── dashboard.html      # Participant registration dashboard
│   └── contact.html        # Contact, feedback, and FAQ page
│
├── styles/
│   ├── style.css           # Shared site styling
│   ├── register.css        # Registration page styling
│   ├── dashboard.css       # Dashboard styling
│   ├── contact.css         # Contact page styling
│   └── carousel.css        # Featured carousel styling
│
├── js/
│   ├── app.js              # Event search, category filter, sort, and timers
│   ├── carousel.js         # Featured event carousel behavior
│   ├── register.js         # Registration validation and LocalStorage
│   ├── dashboard.js        # Participant registration dashboard
│   ├── contact.js          # Contact, feedback, and FAQ interactions
│   └── theme.js            # Theme preference and toggle
│
└── images/
    ├── edufest_icon.svg
    ├── card1.jpg ... card6.jpg
    └── other local event imagery
```

## 🚀 Run locally

### 1. Clone the repository

```bash
git clone https://github.com/shubhamthakur9771/Frontend-Projects.git
cd Frontend-Projects/Event_Management_System
```

### 2. Open the homepage

Open `Html/index.html` in Visual Studio Code and start it using the **Live Server** extension.

You can also open each page directly:

- [Home HTML](./Html/index.html)
- [Registration HTML](./Html/register.html)
- [Dashboard HTML](./Html/dashboard.html)
- [Contact HTML](./Html/contact.html)

### 3. Asset path convention

The HTML pages are inside `Html/`, while `styles/`, `js/`, and `images/` are sibling directories. References from HTML files therefore go up one directory:

```html
<link rel="stylesheet" href="../styles/style.css">
<script src="../js/app.js"></script>
<img src="../images/card1.jpg" alt="Event">
```

Page-to-page links can use the same `Html/` directory, for example `register.html` or `dashboard.html`.

## ☁️ Deployment

EduFest is deployed on Vercel and connected to the GitHub repository.

- **Live URL:** [https://edu-fest-theta.vercel.app/](https://edu-fest-theta.vercel.app/)
- **GitHub repository:** [Frontend-Projects](https://github.com/shubhamthakur9771/Frontend-Projects)
- **Project folder / Vercel root directory:** `Event_Management_System`
- **Application type:** Static HTML, CSS, and JavaScript.

The current implementation does not require a frontend build command or environment variables. The root route opens the homepage under `Html/`.

## 💾 Browser storage and data behavior

EduFest uses the browser's **LocalStorage** for its demonstration flow:

- `registrations` stores submitted registration records.
- `currentUserEmail` identifies which stored registrations the dashboard displays.
- `selectedEvent` can pass a selected event into the registration form.
- `theme` stores the selected light/dark preference.

This information is stored in the visitor's browser for this website origin. It is not a shared registration database and does not automatically transfer to another browser or device. Clearing site data removes locally stored records.

## ⚠️ Scope and limitations

EduFest is a frontend demonstration, not a production event-management service.

- Registration data is stored locally in the browser; it is not sent to a backend or central database.
- The contact and feedback forms perform client-side validation and display success UI states. They do not currently send messages, create support tickets, or deliver email.
- The participant dashboard is based on the browser-stored email and registration records; there is no production account system or authentication.
- Event cards and displayed event details are frontend content, not a live event feed from an API.
- No payment gateway or server-side payment processing is included, even where sample event cards display prices.
- Do not enter real student, contact, or payment information.
- External icon libraries require an internet connection.

## 🔗 Source code and related links

- [Browse the EduFest project folder](https://github.com/shubhamthakur9771/Frontend-Projects/tree/main/Event_Management_System)
- [Home page HTML](https://github.com/shubhamthakur9771/Frontend-Projects/blob/main/Event_Management_System/Html/index.html)
- [Registration page HTML](https://github.com/shubhamthakur9771/Frontend-Projects/blob/main/Event_Management_System/Html/register.html)
- [Dashboard page HTML](https://github.com/shubhamthakur9771/Frontend-Projects/blob/main/Event_Management_System/Html/dashboard.html)
- [Contact page HTML](https://github.com/shubhamthakur9771/Frontend-Projects/blob/main/Event_Management_System/Html/contact.html)
- [Stylesheets](https://github.com/shubhamthakur9771/Frontend-Projects/tree/main/Event_Management_System/styles)
- [JavaScript modules](https://github.com/shubhamthakur9771/Frontend-Projects/tree/main/Event_Management_System/js)
- [Images and branding assets](https://github.com/shubhamthakur9771/Frontend-Projects/tree/main/Event_Management_System/images)
- [Main repository README](../README.md)

<div align="center">

**EduFest — bringing campus event discovery and registration into one interface.**

[Back to repository](../README.md) · [Open live application](https://edu-fest-theta.vercel.app/)

</div>
