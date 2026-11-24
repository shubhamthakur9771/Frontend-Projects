<div align="center">

# 👥 Workpeople — Human Resource Management System

### A multi-page HR workspace interface for employee and people operations

[![HTML5](https://img.shields.io/badge/HTML5-structure-orange?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-styling-blue?logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-vanilla-yellow?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

[Open dashboard](./Html/index.html) · [Employee directory](./Html/employee.html) · [Departments](./Html/department.html) · [Leave center](./Html/leave.html) · [Reports](./Html/reports.html)

</div>

---

## 📖 Overview

**Workpeople** is a browser-based Human Resource Management System (HRMS) frontend concept. It organizes common HR workflows into separate pages and uses shared JavaScript utilities and browser storage to support the demonstration experience.

The project is structured as a multi-page application: a common stylesheet provides the visual system, shared scripts handle application data and common behavior, and individual scripts power specific HR sections.

## ✨ Modules and capabilities

| Module | Page | Purpose |
|---|---|---|
| **Dashboard** | [index.html](./Html/index.html) | Landing workspace and HR overview. |
| **Employee directory** | [employee.html](./Html/employee.html) | Employee roster and employee-related form interactions. |
| **Department management** | [department.html](./Html/department.html) | Department records and department management interactions. |
| **Leave center** | [leave.html](./Html/leave.html) | Leave application, lookup, and leave-log interactions. |
| **Reports & analytics** | [reports.html](./Html/reports.html) | Report views and chart-based visualizations. |

Other implementation details visible in the source include shared form-validation helpers, seeded sample records, browser-side persistence, and theme preferences.

## 🧰 Technology stack

- **HTML5** — page structure and forms.
- **CSS3** — shared styling in `css/style.css`.
- **Vanilla JavaScript** — data handling and page-specific interactions.
- **Web Storage API (LocalStorage)** — sample employees, departments, leave data, attendance data, and theme preference are stored in the browser.
- **jQuery 3.7.1** — loaded by the HTML pages.
- **Chart.js** — loaded on the reports page for chart visualizations.
- **Tabler Icons Webfont** — interface icon assets loaded from a CDN.

## 🗂️ Project structure

```text
HRMS_Project/
├── README.md
├── Html/
│   ├── index.html          # Dashboard
│   ├── employee.html       # Employee directory
│   ├── department.html     # Department management
│   ├── leave.html          # Leave center
│   └── reports.html        # Reports and analytics
├── css/
│   └── style.css           # Shared application stylesheet
└── js/
    ├── data.js             # Seed data and LocalStorage helpers
    ├── app.js              # Shared application behavior
    ├── validation.js       # Shared form validation
    ├── employee.js         # Employee page behavior
    ├── department.js       # Department page behavior
    ├── leave.js            # Leave page behavior
    └── reports.js          # Reports and chart rendering
```

## 🚀 Run locally

1. Clone the repository and open the `HRMS_Project` folder in VS Code.
2. Open [`Html/index.html`](./Html/index.html).
3. Start it with the **Live Server** extension.
4. Use the in-app navigation to explore the other HR modules.

The HTML pages live inside `Html/`, while `css/` and `js/` are sibling folders. Therefore, references from the HTML pages must go up one directory. For example:

```html
<link rel="stylesheet" href="../css/style.css">
<script src="../js/data.js"></script>
<script src="../js/app.js"></script>
```

Page-specific scripts should use the same `../js/` prefix. Page-to-page navigation links should remain relative to the `Html/` folder (for example, `employee.html`).

## 💾 Data and persistence

The project seeds and reads demonstration data through `js/data.js` and the browser's LocalStorage. This means:

- Data is stored locally in the browser profile.
- Clearing site data or using another browser/profile may remove or change the visible sample data.
- The project does not include a server API or shared database in this repository.
- LocalStorage is suitable for a frontend demonstration, not for securing real employee or payroll information.

## ⚠️ Scope and limitations

This repository contains the frontend application and its browser-side logic. It does not include production authentication, authorization, a backend service, a hosted database, or secure handling of real HR records. Treat all sample information as demonstration data.

External libraries and icon fonts are loaded from CDNs, so an internet connection may be needed for those resources.

## 🔗 Source on GitHub

- [Browse HRMS project files](https://github.com/shubhamthakur9771/Frontend-Projects/tree/main/HRMS_Project)
- [Dashboard HTML](https://github.com/shubhamthakur9771/Frontend-Projects/blob/main/HRMS_Project/Html/index.html)
- [Shared stylesheet](https://github.com/shubhamthakur9771/Frontend-Projects/blob/main/HRMS_Project/css/style.css)
- [JavaScript modules](https://github.com/shubhamthakur9771/Frontend-Projects/tree/main/HRMS_Project/js)

---

[← Back to all frontend projects](../README.md)
