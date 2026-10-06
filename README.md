# ClassFlow

Smart Classroom Management System. **Smart classroom. Better learning.**

## Overview
ClassFlow is a responsive static classroom management prototype for teachers. It runs in the browser and stores its data locally, with no server or account required.

## Features
- Classroom dashboard with attendance trends, classes, quick actions, and student attention indicators
- Student directory with search, status filtering, sorting, profile view, add, edit, and delete
- Date based attendance marking with present, absent, and late statuses
- Assignment creation and tracking with due dates, priorities, and submission progress
- Weekly schedule, analytics charts, and announcement management
- Profile and class settings, persistent light/dark mode, keyboard searchable global search, notifications, and toast feedback
- Responsive navigation for desktop, tablet, and mobile

## Screenshots
Open `index.html` to view the dashboard. Screenshots can be added here when publishing.

## Technology
HTML5, CSS3, vanilla JavaScript, localStorage, and Chart.js via CDN. Google Fonts Inter is also loaded via CDN.

## Project Structure
```
index.html, students.html, attendance.html, assignments.html
schedule.html, analytics.html, announcements.html, settings.html
css/  style.css, dashboard.css, responsive.css
js/   app.js, dashboard.js, students.js, attendance.js, assignments.js, analytics.js
assets/images/  assets/icons/
```

## Installation
No install or build step is required. Clone or download the repository.

## Running Locally
Open `index.html` directly, or use VS Code Live Server. Internet access is needed for Chart.js and Google Fonts; the core application works without those CDN resources.

## GitHub Pages Deployment
Push the project to a GitHub repository, then choose **Settings → Pages**, select the branch and root folder, and save. The site entry point is `index.html`.

## Data Architecture
On first load, ClassFlow seeds realistic demo data. It persists data under `classflow_students`, `classflow_attendance`, `classflow_assignments`, `classflow_announcements`, `classflow_schedule`, and `classflow_settings`. Existing stored records are retained across reloads. Data is specific to the browser and device; clearing site storage removes it.

## Future Enhancements
- CSV student import/export
- Editable schedule builder and attendance history reporting
- Assignment submission workflows and configurable notification preferences
- Optional synchronization with a hosted service
