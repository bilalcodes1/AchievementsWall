# AchievementsWall 🏆

Arabic student achievements wall for Computer Science students.

This project is a web-based achievement and weekly task tracking system designed for students. It allows each student to log in, write their achievements, complete weekly tasks, and track the overall progress of the group through a clean Arabic interface.

---

## Live Demo

```txt
https://bilalzamilahmed.page/AchievementsWall/
```

If the project is still hosted under the original GitHub Pages domain, use:

```txt
https://bilalcodes1.github.io/AchievementsWall/
```

---

## Project Overview

**AchievementsWall** is an Arabic web application created to help students document their weekly achievements and track assigned tasks.

The project is designed as a simple student dashboard where each student has a personal card. Students can write their achievements, complete weekly tasks, and see the general completion percentage for the whole group.

The system also includes an admin panel for managing weekly tasks.

---

## Main Purpose

The purpose of this project is to encourage students to:

* Write their weekly achievements
* Follow assigned tasks
* Track their progress
* Build consistency
* Share progress in a simple organized way
* Create a motivating student environment

---

## Features

* Arabic RTL interface
* Login system
* Student achievement cards
* Weekly task checklist
* Global progress bar
* Automatic progress percentage calculation
* Save achievement text automatically
* Admin task management panel
* Add weekly tasks
* Edit tasks
* Delete tasks
* Password change modal
* Developer information modal
* Local session storage using `localStorage`
* Google Sheets backend through Google Apps Script
* JSONP-based communication with the backend
* Celebration effect when all tasks are completed
* Confetti animation
* Celebration sound support
* Responsive card layout
* Clean UI using custom CSS
* Arabic font using Google Fonts Tajawal

---

## User Roles

| Role    | Description                                               |
| ------- | --------------------------------------------------------- |
| Student | Can write achievements and complete personal weekly tasks |
| Admin   | Can manage weekly tasks and view/manage the board         |

---

## Main Sections

### Login Screen

The login screen allows students and admins to access the achievement wall using a username and password.

### Achievement Board

The main board displays student cards. Each card contains:

* Student name
* Profile circle
* Achievement text area
* Weekly task checklist
* Save status indicator

### Global Progress Bar

A sticky progress bar shows the overall completion percentage for all weekly tasks across all students.

### Admin Sidebar

The admin sidebar allows the admin to:

* Add new weekly tasks
* Edit existing tasks
* Delete tasks
* Manage the task list for all students

### Password Modal

Users can change their password using the password change modal.

### About Developer Modal

A simple modal that shows information about the developer and social links.

---

## Tech Stack

| Category           | Technology             |
| ------------------ | ---------------------- |
| Frontend           | HTML, CSS, JavaScript  |
| Styling            | Custom CSS             |
| Font               | Google Fonts – Tajawal |
| Backend            | Google Apps Script     |
| Database           | Google Sheets          |
| Data Communication | JSONP                  |
| Storage            | Browser localStorage   |
| Effects            | canvas-confetti        |
| Hosting            | GitHub Pages           |

---

## Backend Integration

The application connects to a Google Apps Script endpoint that works as the backend API.

The backend is responsible for:

* User login
* Loading board data
* Saving achievements
* Updating task completion status
* Managing weekly tasks
* Changing passwords

The frontend communicates with the backend using JSONP.

---

## Main Functionalities

### Login

Users log in with their username and password. After successful login, user data is stored locally in the browser using `localStorage`.

### Auto Save

When a user writes inside the achievement text area, the system waits briefly and then saves the achievement automatically.

### Task Completion

Students can check or uncheck their weekly tasks. The task status is saved to the backend and reflected in the global progress bar.

### Admin Task Management

Admins can add, edit, or delete weekly tasks from the sidebar. These tasks appear for students in their achievement cards.

### Progress Tracking

The system calculates the overall progress percentage by comparing completed tasks with total tasks across all users.

### Celebration

When a student completes all assigned tasks, the app triggers a celebration effect using confetti and an optional sound.

---

## Project Structure

```txt
AchievementsWall/
├── index.html
├── sounds/
│   └── celebration.mp3
└── README.md
```

The current version is built mainly as a single-page static web application.

---

## How to Run Locally

1. Clone the repository:

```bash
git clone https://github.com/bilalcodes1/AchievementsWall.git
```

2. Open the project folder:

```bash
cd AchievementsWall
```

3. Open `index.html` in your browser.

The interface will open normally, but backend features require a valid Google Apps Script endpoint.

---

## Configuration

The project uses a Google Apps Script URL inside the JavaScript code:

```js
const GOOGLE_SHEET_URL = "YOUR_GOOGLE_APPS_SCRIPT_URL";
```

To use your own backend:

1. Create a Google Sheet.
2. Create a Google Apps Script project.
3. Deploy it as a web app.
4. Replace the URL in the project with your Apps Script URL.

---

## Security Notes

This project is designed for educational and internal student use.

Important notes:

* Do not expose sensitive student information publicly.
* Avoid storing real passwords in plain text.
* If the project is used seriously, improve authentication and backend security.
* Google Apps Script URLs should be handled carefully.
* Public GitHub Pages projects can expose frontend code to visitors.

---

## Suggested Repository Topics

```txt
html
css
javascript
arabic-website
rtl
student-dashboard
achievements-wall
google-sheets
google-apps-script
university-project
anbar-university
```

---

## Future Improvements

* Improve authentication security
* Add password hashing in the backend
* Add user profile images
* Add weekly reports
* Add export to PDF
* Add task categories
* Add admin dashboard statistics
* Add mobile UI improvements
* Add dark mode
* Add better backend error handling
* Replace JSONP with a safer API method if possible

---

## Purpose

This repository was created as a student productivity and motivation tool.

It can be used for:

* Tracking weekly student progress
* Sharing achievements
* Managing weekly tasks
* Encouraging consistency
* Supporting classroom or student group activity

---

## Author

**Bilal Zamil Ahmed**
Computer Science Student
University of Anbar

GitHub: [@bilalcodes1](https://github.com/bilalcodes1)
YouTube: [Bilal Codes](https://www.youtube.com/@bilalcodes1)

---

## License

Educational project — All rights reserved © 2026 Bilal Zamil Ahmed.
