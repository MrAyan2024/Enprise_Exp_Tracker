# 📊 Enterprise Payroll & Expense Tracker Dashboard

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=for-the-badge&logo=chartdotjs&logoColor=white)

**Live Demo:** [Click here to view the live application](https://mrayan2024.github.io/expense-tracker) *(Replace with your actual link)*

---

## 📖 Overview
The **Enterprise Payroll & Expense Tracker** is a powerful, client-side web application designed to transform raw Excel payroll data into interactive, real-time analytics dashboards. Built entirely with vanilla JavaScript and modern web technologies, it requires **zero backend infrastructure**, ensuring 100% data privacy as all processing happens locally in the browser. 

Perfect for HR and Finance teams, it allows multiple managers to upload their respective team data cumulatively, edit records on the fly, and generate comprehensive visual reports and individual payslips instantly.

---

## ✨ Key Features

- 📂 **Cumulative Multi-Upload**: Uses browser LocalStorage to accumulate data from multiple Excel files (e.g., Media, HR, Acct teams) without overwriting previous uploads.
- ✏️ **Inline Editing & Auto-Recalculation**: Edit any salary component directly in the "Edit Master Data" tab. The app automatically recalculates the `Total` and highlights edited cells in yellow across all dashboards.
- 📊 **11 Interactive Dashboard Tabs**: 
  - Executive Dashboard, Expense Analysis, Employee Directory
  - Month/Year-wise Filtering, Monthly Variable Pay, Attendance & OT
  - Salary Processing, Payslip Generator, Complete Salary Register
  - Employee Salary History, and Edit Master Data
- 📈 **Rich Data Visualization**: Powered by Chart.js for dynamic Pie, Bar, Line, and Doughnut charts.
- 💾 **Persistent Local Storage**: Data remains saved in the browser session until explicitly cleared, preventing data loss on accidental refreshes.
- 📤 **Export to Excel**: Download the modified, combined dataset back to an `.xlsx` file, complete with an "Edited" status column.
- 📱 **Fully Responsive**: Built with Tailwind CSS for a seamless experience on desktops, tablets, and mobile devices.

---

## 🛠️ Tech Stack

- **Frontend**: Vanilla JavaScript (ES6+), HTML5, CSS3
- **Styling**: Tailwind CSS (via CDN)
- **Data Visualization**: Chart.js
- **File Parsing**: SheetJS (`xlsx` library)
- **Storage**: Browser `localStorage` API
- **Typography**: Google Fonts (Inter)

---

## 📥 Expected Excel Data Format

For the application to parse data correctly, your uploaded `.xlsx`, `.xls`, or `.csv` file must contain the following column headers in the first row:

| Emp ID | Name | Project | Basic | TA | FA | NA | OT | IN | Total | Month | Year |
|--------|------|---------|-------|----|----|----|----|----|-------|-------|------|
| E001 | John Doe | Media | 50000 | 5000 | 3000 | 2000 | 4000 | 1000 | 65000 | January | 2026 |

*(Note: Currency symbols like `₹` or `$` and commas in the Excel file are automatically handled and stripped by the parser.)*

---

## 🚀 How to Run Locally

Since this is a purely client-side application, no Node.js, npm, or backend server is required.

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/expense-tracker.git
   cd expense-tracker
