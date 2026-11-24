<div align="center">

# 👥 Workpeople — Human Resource Management System

### A multi-page HR workspace for employee, department, leave, attendance, and reporting workflows

[![Live Demo](https://img.shields.io/badge/Live_Demo-Open_Workpeople-0A7F45?logo=vercel&logoColor=white)](https://work-people.vercel.app/)
[![HTML5](https://img.shields.io/badge/HTML5-Structure-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-Styling-1572B6?logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla-F7DF1E?logo=javascript&logoColor=222222)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Chart.js](https://img.shields.io/badge/Charts-Chart.js-FF6384?logo=chartdotjs&logoColor=white)](https://www.chartjs.org/)

[Live Dashboard](https://work-people.vercel.app/) · [Employees](https://work-people.vercel.app/Html/employee.html) · [Departments](https://work-people.vercel.app/Html/department.html) · [Leave Centre](https://work-people.vercel.app/Html/leave.html) · [Reports](https://work-people.vercel.app/Html/reports.html)

[← Back to Frontend Projects](../README.md) · [View GitHub source](https://github.com/shubhamthakur9771/Frontend-Projects/tree/main/HRMS_Project)

</div>

---

## 📌 Project overview

**Workpeople HRMS** is a browser-based Human Resource Management System frontend concept. It brings common HR activities into one multi-page workspace: employee records, department organization, leave requests, attendance summaries, and management reports.

The application uses shared JavaScript modules for browser storage, validation, theme preferences, notifications, and common UI behavior. Each HR module has its own page and page-specific script.

> **Live application:** [https://work-people.vercel.app/](https://work-people.vercel.app/)

## 🖥️ Live application pages

| Module | Live page | Purpose |
|---|---|---|
| Dashboard | [Open dashboard ↗](https://work-people.vercel.app/Html/index.html) | HR overview, quick employee roster, attendance, leave, schedule, and recent-hire sections. |
| Employee directory | [Open employees ↗](https://work-people.vercel.app/Html/employee.html) | Browse, search, filter, register, and update employee status. |
| Department directory | [Open departments ↗](https://work-people.vercel.app/Html/department.html) | Create and edit departments, search the directory, and sort departments. |
| Leave centre | [Open leave centre ↗](https://work-people.vercel.app/Html/leave.html) | Submit leave requests, review the leave log, and demonstrate approval/rejection actions. |
| Reports & analytics | [Open reports ↗](https://work-people.vercel.app/Html/reports.html) | Review HR summary metrics, charts, department ratios, leave allocations, and print reports. |

## ✨ Features and modules

### 1. Overview dashboard

- HR summary cards for employee count, attendance, employees on leave, and monthly payroll totals.
- Employee quick-roster section with search and filtering controls.
- Dedicated areas for daily attendance, pending leave requests, today's schedule, and recent hires.
- Shared navigation and theme controls across the application.

### 2. Employee directory

- Employee registration form with generated employee IDs.
- Input validation for required fields, email format, 10-digit mobile number, joining date, and minimum salary.
- Department options populated from the department records.
- Optional profile image upload with image preview; PNG, JPEG, and WEBP formats are checked in the frontend.
- Employee roster search and department filtering.
- Paginated roster display.
- Employee status can be changed to **Inactive** through the directory action.

### 3. Department management

- Create a department with a department code, name, manager, and extension number.
- Edit existing department details.
- Search by department name, manager, or department code.
- Sort the department list A–Z or Z–A.
- Department employee counts are recalculated from active employee records when employee data is saved.

### 4. Leave management

- Submit a leave request using an employee ID.
- Look up the employee name from the employee directory.
- Choose a leave category and enter start date, end date, and reason.
- Calculate requested working days while excluding Saturdays and Sundays.
- Search the leave log and filter by leave status.
- Demonstrate pending leave approval and rejection through the HR approval-mode interface.

### 5. Reports and analytics

- Summary metrics for active staff, weekly attendance, employees on leave, and monthly payroll totals.
- Daily attendance status visualization.
- Weekly attendance-rate chart.
- Department staff-ratio visualization.
- Leave allocation chart by leave category.
- Print-friendly report action using the browser print dialog.

### 6. Shared application experience

- Light/dark theme preference stored in the browser.
- Responsive sidebar navigation with a mobile menu control.
- Shared form validation utilities.
- Toast notifications for user actions and validation feedback.
- Loading-screen and back-to-top interactions where included in the page markup.

## 🧰 Technology stack

| Technology | Role in this project |
|---|---|
| HTML5 | Multi-page application structure and forms. |
| CSS3 | Shared visual system, responsive layout, and component styling. |
| Vanilla JavaScript | Data operations, form handling, filtering, UI behavior, and calculations. |
| LocalStorage | Browser-local persistence for employees, departments, leaves, attendance, and theme. |
| jQuery | Included by the HTML pages for DOM utilities. |
| Chart.js | Dashboard/report chart visualizations. |
| Tabler Icons and external icon/font resources | Interface iconography. |

## 🗂️ Project structure

```text
HRMS_Project/
├── README.md
│
├── Html/
│   ├── index.html          # Overview dashboard
│   ├── employee.html       # Employee directory and registration
│   ├── department.html     # Department management
│   ├── leave.html          # Leave requests and leave log
│   └── reports.html        # Reports and analytics
│
├── css/
│   └── style.css           # Shared application stylesheet
│
└── js/
    ├── data.js             # Seed data and LocalStorage engine
    ├── app.js              # Shared UI, theme, toast, and navigation behavior
    ├── validation.js       # Reusable validation rules and helpers
    ├── employee.js         # Employee registration and directory behavior
    ├── department.js       # Department create, edit, search, and sort behavior
    ├── leave.js            # Leave request and approval interactions
    └── reports.js          # Summary metrics and chart rendering
```

## 🚀 Run locally

### 1. Clone the repository

```bash
git clone https://github.com/shubhamthakur9771/Frontend-Projects.git
cd Frontend-Projects/HRMS_Project
```

### 2. Open the dashboard

Open `Html/index.html` in Visual Studio Code and start it using the **Live Server** extension.

You can also open each page directly through Live Server:

- [Dashboard HTML](./Html/index.html)
- [Employee directory HTML](./Html/employee.html)
- [Department HTML](./Html/department.html)
- [Leave centre HTML](./Html/leave.html)
- [Reports HTML](./Html/reports.html)

### 3. Asset path convention

The HTML files are inside `Html/`, while `css/` and `js/` are sibling directories. Therefore, references from an HTML page use `../` to reach those folders:

```html
<link rel="stylesheet" href="../css/style.css">

<script src="../js/data.js"></script>
<script src="../js/app.js"></script>
```

Page-to-page navigation links remain relative to the `Html/` directory, such as `employee.html` and `reports.html`.

## ☁️ Deployment

This project is deployed on Vercel and connected to the GitHub repository.

- **Live URL:** [https://work-people.vercel.app/](https://work-people.vercel.app/)
- **GitHub repository:** [Frontend-Projects](https://github.com/shubhamthakur9771/Frontend-Projects)
- **Project folder / Vercel root directory:** `HRMS_Project`
- **Application type:** Static HTML, CSS, and JavaScript.

The project does not require a frontend build command or environment variables in its current implementation. The root route is configured to open the dashboard page.

## 💾 Data storage and persistence

The current implementation uses the browser's **LocalStorage** through the `StorageEngine` in `js/data.js`.

- Employee records are stored under `wp_employees`.
- Department records are stored under `wp_departments`.
- Leave records are stored under `wp_leaves`.
- Attendance records are stored under `wp_attendance`.
- Theme preference is stored under `wp_theme`.

This means the data belongs to the browser profile and website origin where it was created. It is not shared between different users, browsers, or devices. Clearing site data can remove the stored records.

## ⚠️ Scope and limitations

Workpeople is a frontend demonstration, not a production HR platform.

- There is no backend API or shared database in this repository.
- There is no production login, authentication, or server-enforced role-based authorization.
- The HR approval-mode interaction is a client-side demonstration and must not be treated as a security boundary.
- Employee, attendance, leave, and department records are stored in LocalStorage and can be inspected or modified by the browser user.
- The payroll figure is a frontend summary calculation; the project does not process salary payments or generate statutory payroll outputs.
- Do not enter real employee, salary, identity, or other sensitive information.
- External libraries, fonts, and icons may require an internet connection.

## 🔗 Source code and related links

- [Browse the HRMS project folder](https://github.com/shubhamthakur9771/Frontend-Projects/tree/main/HRMS_Project)
- [Dashboard HTML](https://github.com/shubhamthakur9771/Frontend-Projects/blob/main/HRMS_Project/Html/index.html)
- [Employee page HTML](https://github.com/shubhamthakur9771/Frontend-Projects/blob/main/HRMS_Project/Html/employee.html)
- [Department page HTML](https://github.com/shubhamthakur9771/Frontend-Projects/blob/main/HRMS_Project/Html/department.html)
- [Leave page HTML](https://github.com/shubhamthakur9771/Frontend-Projects/blob/main/HRMS_Project/Html/leave.html)
- [Reports page HTML](https://github.com/shubhamthakur9771/Frontend-Projects/blob/main/HRMS_Project/Html/reports.html)
- [JavaScript modules](https://github.com/shubhamthakur9771/Frontend-Projects/tree/main/HRMS_Project/js)
- [Shared stylesheet](https://github.com/shubhamthakur9771/Frontend-Projects/blob/main/HRMS_Project/css/style.css)
- [Main repository README](../README.md)

<div align="center">

**Workpeople HRMS — a frontend exploration of everyday HR workflows.**

[Back to repository](../README.md) · [Open live application](https://work-people.vercel.app/)

</div>
