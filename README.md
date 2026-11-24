<div align="center">

# ✨ Frontend Projects

### A collection of responsive interfaces, frontend experiments, and browser-based applications

[![HTML5](https://img.shields.io/badge/HTML5-Structure-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-Styling-1572B6?logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-Interactivity-F7DF1E?logo=javascript&logoColor=222222)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Vercel](https://img.shields.io/badge/Deployed_on-Vercel-000000?logo=vercel&logoColor=white)](https://vercel.com/)
[![GitHub](https://img.shields.io/badge/Source-GitHub-181717?logo=github&logoColor=white)](https://github.com/shubhamthakur9771/Frontend-Projects)

**Three independent projects. One repository. Two live web applications.**

[Explore Workpeople HRMS](https://work-people.vercel.app/) · [Explore EduFest](https://edu-fest-theta.vercel.app/) · [Browse source code](https://github.com/shubhamthakur9771/Frontend-Projects)

</div>

---

## 👋 About this repository

This repository brings together three frontend projects built to practise web development fundamentals and create interactive browser experiences. It includes focused HTML/CSS layout exercises as well as two larger multi-page applications:

- **YouTube Clone Practice** — layout exercises using Flexbox and CSS Grid.
- **Workpeople HRMS** — a human-resources workspace for employee, department, leave, attendance, and reporting workflows.
- **EduFest** — a campus event portal concept with event discovery, registration, a participant dashboard, and contact/feedback interfaces.

Workpeople HRMS and EduFest are deployed independently on Vercel. The projects share this GitHub repository but have separate folders, assets, and documentation.

## 🚀 Live applications

| Application | Live website | Main capabilities | Project documentation |
|---|---|---|---|
| **Workpeople HRMS** | [Open live HRMS ↗](https://work-people.vercel.app/) | Dashboard, employee directory, departments, leave centre, reports and analytics | [Read HRMS documentation](./HRMS_Project/README.md) |
| **EduFest** | [Open live EduFest ↗](https://edu-fest-theta.vercel.app/) | Event discovery, search and filters, event registration, participant dashboard, contact and FAQs | [Read EduFest documentation](./Event_Management_System/README.md) |

### Direct page links

**Workpeople HRMS**

- [Dashboard](https://work-people.vercel.app/Html/index.html)
- [Employee directory](https://work-people.vercel.app/Html/employee.html)
- [Departments](https://work-people.vercel.app/Html/department.html)
- [Leave centre](https://work-people.vercel.app/Html/leave.html)
- [Reports and analytics](https://work-people.vercel.app/Html/reports.html)

**EduFest**

- [Home and event discovery](https://edu-fest-theta.vercel.app/)
- [Event registration](https://edu-fest-theta.vercel.app/Html/register.html)
- [Participant dashboard](https://edu-fest-theta.vercel.app/Html/dashboard.html)
- [Contact, feedback and FAQs](https://edu-fest-theta.vercel.app/Html/contact.html)

## 🧭 Project gallery

### 1. ▶️ YouTube Clone Practice

A collection of YouTube-inspired page layout exercises focused on recreating a video browsing interface and understanding CSS layout techniques.

**What it covers**

- Video-grid layouts using Flexbox and CSS Grid.
- Header, sidebar, video thumbnail, channel picture, and metadata layout practice.
- Introductory HTML pages and small CSS exercises.
- Separate Flexbox and Grid implementations for comparing layout approaches.

**Technologies:** HTML5, CSS3, Flexbox, CSS Grid.

- [Project guide](./Youtube-Clone-Practice/README.md)
- [Flexbox implementation](./Youtube-Clone-Practice/Flex/youtube.html)
- [Grid implementation](./Youtube-Clone-Practice/Grid/youtube.html)
- [Browse project source](https://github.com/shubhamthakur9771/Frontend-Projects/tree/main/Youtube-Clone-Practice)

<sub>This practice project does not currently have a separate live Vercel deployment.</sub>

### 2. 👥 Workpeople HRMS

A multi-page HR workspace concept that groups common people-operations workflows into a single interface.

**Available modules**

- Dashboard overview with employee, attendance, leave, and payroll summary areas.
- Employee directory with registration, search, department filtering, pagination, and employee status management.
- Department directory with department creation, editing, searching, and alphabetical sorting.
- Leave centre with employee lookup, leave requests, working-day calculation, status filtering, and approval/rejection interactions.
- Reports and analytics with summary metrics, department ratios, attendance and leave charts, and print support.
- Shared theme preference, responsive navigation, form validation, and toast notifications.

**Technologies:** HTML5, CSS3, vanilla JavaScript, LocalStorage, jQuery, Chart.js, and icon/font libraries loaded by the pages.

- [Live application](https://work-people.vercel.app/)
- [Detailed HRMS guide](./HRMS_Project/README.md)
- [Browse HRMS source](https://github.com/shubhamthakur9771/Frontend-Projects/tree/main/HRMS_Project)

### 3. 🎟️ EduFest — Event Management System

A campus event portal concept for discovering technical and non-technical events and exploring a participant registration journey.

**Available modules**

- Event landing page with featured event carousel and event cards.
- Event search, category filtering, and date-based sorting.
- Event countdown displays and theme switching.
- Registration form with field validation and duplicate-registration checks in browser storage.
- Participant dashboard showing registrations associated with the current browser-stored email.
- Contact and feedback forms with client-side validation and success states.
- FAQ search and expandable answers.

**Technologies:** HTML5, CSS3, vanilla JavaScript, LocalStorage, Font Awesome, Tabler Icons, and local image assets.

- [Live application](https://edu-fest-theta.vercel.app/)
- [Detailed EduFest guide](./Event_Management_System/README.md)
- [Browse EduFest source](https://github.com/shubhamthakur9771/Frontend-Projects/tree/main/Event_Management_System)

## 🗂️ Repository structure

```text
Frontend-Projects/
├── README.md
│
├── Youtube-Clone-Practice/
│   ├── README.md
│   ├── Flex/
│   │   ├── youtube.html
│   │   ├── styles/
│   │   ├── thumbnails/
│   │   └── channel-pictures/
│   └── Grid/
│       ├── youtube.html
│       ├── style.css
│       ├── thumbnails/
│       └── channel-pictures/
│
├── HRMS_Project/
│   ├── README.md
│   ├── vercel.json
│   ├── Html/
│   ├── css/
│   └── js/
│
└── Event_Management_System/
    ├── README.md
    ├── vercel.json
    ├── Html/
    ├── styles/
    ├── js/
    └── images/
```

## 🛠️ Run the projects locally

### 1. Clone the repository

```bash
git clone https://github.com/shubhamthakur9771/Frontend-Projects.git
cd Frontend-Projects
```

### 2. Open a project

Open the repository in Visual Studio Code and choose the HTML entry page you want to explore.

### 3. Start a local server

These projects are static frontend applications and do not define a Node.js build step. You can use the **Live Server** extension in VS Code:

1. Install the Live Server extension if needed.
2. Open the required HTML page.
3. Right-click and choose **Open with Live Server**.

Use the project-specific READMEs for exact entry pages and directory details:

- [YouTube Clone Practice setup](./Youtube-Clone-Practice/README.md)
- [Workpeople HRMS setup](./HRMS_Project/README.md)
- [EduFest setup](./Event_Management_System/README.md)

## 🧰 Technology overview

| Technology | How it is used |
|---|---|
| HTML5 | Page structure, forms, and semantic content. |
| CSS3 | Visual styling, responsive layouts, and page-specific presentation. |
| Flexbox | Layout practice in the YouTube clone exercises. |
| CSS Grid | Video-card layout practice in the YouTube clone exercises. |
| JavaScript | Browser-side interactions, validation, filtering, and application behavior. |
| LocalStorage | Local demonstration data and preferences in HRMS and EduFest. |
| jQuery | Included by the HRMS pages. |
| Chart.js | Report visualizations in HRMS. |
| Vercel | Hosting for the HRMS and EduFest static frontends. |

## ⚠️ Important project scope

These are frontend demonstrations, not production-ready business systems.

- HRMS records, attendance, leave data, departments, and theme preferences are stored in the visitor's browser using LocalStorage. They are not synchronized across users or devices.
- EduFest registrations and theme preferences are browser-local. The contact and feedback interfaces validate input and display success states, but the current frontend does not submit the information to a server or send email.
- The repository does not include a backend API, hosted database, production authentication, payment processing, or server-side authorization for these applications.
- Do not enter real employee, student, payment, or other sensitive personal information into the demos.
- Third-party fonts and icon libraries loaded from CDNs require an internet connection.

## 🔗 Repository links

- [GitHub repository](https://github.com/shubhamthakur9771/Frontend-Projects)
- [All project folders](https://github.com/shubhamthakur9771/Frontend-Projects/tree/main)
- [Workpeople HRMS source](https://github.com/shubhamthakur9771/Frontend-Projects/tree/main/HRMS_Project)
- [EduFest source](https://github.com/shubhamthakur9771/Frontend-Projects/tree/main/Event_Management_System)
- [YouTube Clone Practice source](https://github.com/shubhamthakur9771/Frontend-Projects/tree/main/Youtube-Clone-Practice)

<div align="center">

**Built for learning, experimentation, and continuous frontend development.**

</div>
