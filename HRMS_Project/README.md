<div align="center">

# 👥 Workpeople — Human Resource Management System

**A multi-page HR management dashboard concept**

[Open Dashboard](./Html/index.html)

</div>

---

## 📖 Overview

Workpeople is a browser-based HRMS frontend project designed around common human resource workflows. It provides separate interfaces for employee records, department management, leave management and reports.

The application uses JavaScript to manage page interactions and browser LocalStorage for its sample data.

## ✨ Features

- **Dashboard:** HR workspace and overview.
- **Employee directory:** employee listing and employee registration interface.
- **Department management:** department-related records and forms.
- **Leave management:** leave application and management interface.
- **Reports & analytics:** summary views and charts.
- **Form validation:** shared validation utilities for input handling.
- **Theme and interface controls:** shared UI behavior across pages.
- **Browser persistence:** sample application data managed through LocalStorage.

## 🧰 Technologies

- HTML5
- CSS3
- JavaScript (Vanilla)
- LocalStorage
- jQuery
- Chart.js
- Tabler Icons

## 🗂️ Project structure

```text
HRMS_Project/
├── README.md
├── Html/
│   ├── index.html
│   ├── employee.html
│   ├── department.html
│   ├── leave.html
│   └── reports.html
├── css/
│   └── style.css
└── js/
    ├── app.js
    ├── data.js
    ├── validation.js
    ├── employee.js
    ├── department.js
    ├── leave.js
    └── reports.js
```

## 🚀 Run locally

1. Open the `HRMS_Project` folder in VS Code.
2. Start Live Server using `Html/index.html`.
3. Open the local URL provided by Live Server.

### Important: fix asset paths before running

The HTML pages are inside `Html/`, while `css/` and `js/` are sibling directories. Paths in the current HTML files need to go up one directory.

Use:

```html
<link rel="stylesheet" href="../css/style.css">

<script src="../js/data.js"></script>
<script src="../js/app.js"></script>
```

Apply the same `../js/` prefix to each page-specific script, such as `employee.js`, `department.js`, `leave.js` and `reports.js`.

## ⚠️ Project scope

This archive contains frontend code and browser-side sample data. It does not include a backend API, server-side authentication, or a production database. LocalStorage data belongs to the browser profile in which the application is opened.

---

[← Back to all frontend projects](../README.md)
