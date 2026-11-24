<div align="center">

# ✨ Frontend Projects

### A curated collection of frontend practice and interactive web applications

[![HTML5](https://img.shields.io/badge/HTML5-markup-orange?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-styling-blue?logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-interactivity-yellow?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![GitHub](https://img.shields.io/badge/GitHub-Repository-181717?logo=github)](https://github.com/shubhamthakur9771/Frontend-Projects)

**Explore the projects, open their live HTML entry points locally, and browse the source code.**

[YouTube Clone Practice](./Youtube-Clone-Practice/README.md) · [Workpeople HRMS](./HRMS_Project/README.md) · [EduFest](./Event_Management_System/README.md)

</div>

---

## 👋 About this repository

This repository brings together three frontend projects built while practising web development fundamentals and creating browser-based interfaces. The collection moves from focused HTML/CSS layout exercises to larger multi-page applications with JavaScript-driven interactions.

The projects are intentionally kept independent: each has its own assets, stylesheets, scripts, and project-level README.

## 🧭 Project gallery

| Project | What you will find | Main technologies | Start here |
|---|---|---|---|
| **▶️ YouTube Clone Practice** | YouTube-inspired video layout exercises implemented with Flexbox and CSS Grid, plus introductory HTML pages. | HTML5, CSS3, Flexbox, Grid | [Open Flexbox](./Youtube-Clone-Practice/Flex/youtube.html) · [Open Grid](./Youtube-Clone-Practice/Grid/youtube.html) |
| **👥 Workpeople HRMS** | A multi-page HR workspace covering dashboard, employee directory, departments, leave management, and reports. | HTML5, CSS3, Vanilla JavaScript, LocalStorage, jQuery, Chart.js | [Open dashboard](./HRMS_Project/Html/index.html) |
| **🎟️ EduFest** | A campus-event portal concept with home, event registration, participant dashboard, and contact pages. | HTML5, CSS3, Vanilla JavaScript, LocalStorage, icon libraries | [Open home](./Event_Management_System/Html/index.html) |

### Project documentation

- [YouTube Clone Practice — detailed guide](./Youtube-Clone-Practice/README.md)
- [Workpeople HRMS — detailed guide](./HRMS_Project/README.md)
- [EduFest — detailed guide](./Event_Management_System/README.md)

## 🗂️ Repository structure

```text
Frontend-Projects/
├── README.md
├── Youtube-Clone-Practice/
│   ├── README.md
│   ├── Flex/                 # Flexbox-focused layout exercises
│   └── Grid/                 # CSS Grid-focused layout exercises
├── HRMS_Project/
│   ├── README.md
│   ├── Html/                 # Dashboard and HR workflow pages
│   ├── css/                  # Shared application styling
│   └── js/                   # Data, validation, and page behavior
└── Event_Management_System/
    ├── README.md
    ├── Html/                 # Home, registration, dashboard, contact
    ├── styles/               # Shared and page-specific stylesheets
    ├── js/                   # Page interactions and theme behavior
    └── images/               # Event cards and branding assets
```

## 🚀 Getting started

### 1. Clone the repository

```bash
git clone https://github.com/shubhamthakur9771/Frontend-Projects.git
cd Frontend-Projects
```

### 2. Choose a project

Open one of the project folders in your editor. These are static frontend projects; no package installation or build step is defined in the repository.

### 3. Run with VS Code Live Server

1. Open the repository in Visual Studio Code.
2. Install the **Live Server** extension if it is not already installed.
3. Open the desired HTML entry page from the links in the project guide.
4. Right-click the HTML file and select **Open with Live Server**.

A local HTTP server is recommended because it provides a consistent way to load local stylesheets, scripts, and images. External CDN resources also require an internet connection.

## 🧰 Technology overview

- **HTML5** — page structure and semantic content.
- **CSS3** — styling, spacing, typography, and layout.
- **Flexbox & CSS Grid** — layout techniques explored in the YouTube practice project.
- **Vanilla JavaScript** — browser-side interactions and page behavior in HRMS and EduFest.
- **LocalStorage** — browser-local sample data and preferences where implemented.
- **jQuery & Chart.js** — used by the HRMS pages for DOM utilities and report visualizations.

## 🔎 Notes and project scope

- The repository contains frontend source code and local assets; it does not provide a production backend or hosted database.
- HRMS sample records and selected preferences are stored in the browser using LocalStorage. They are not shared between browsers or devices.
- EduFest registration data and theme preferences use browser-side storage where implemented; this is a frontend demonstration, not a server-backed registration service.
- Some pages load fonts or icon libraries from CDNs. Keep an internet connection available when testing those pages.
- Do not add private API keys, passwords, access tokens, or other secrets to committed frontend code. Anything shipped to a browser is visible to visitors.

## 🧪 Suggested exploration path

1. Start with **YouTube Clone Practice** to compare Flexbox and Grid layouts.
2. Explore **Workpeople HRMS** to see how shared data and page-specific scripts support a multi-page interface.
3. Explore **EduFest** to review a themed event portal with registration and dashboard flows.

## 🔗 Repository

[View Frontend-Projects on GitHub](https://github.com/shubhamthakur9771/Frontend-Projects)

<div align="center">

**Built for learning, experimentation, and continuous frontend practice.**

</div>
