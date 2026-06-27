Cash-Flow Dashboard — Salary & Expense Tracker (Sprint 02)

A responsive and dynamic financial dashboard built to track salaries and log expenses. This project was developed as part of Sprint 02 to demonstrate core engineering logic, Vanilla JavaScript mastery, manual DOM manipulation, and data persistence without relying on modern abstraction layers like React.

Live Deployment

Live Demo: []

Features

Core MVP

Input Architecture: Dedicated forms to capture base salary and individual line-item expenses.

Logic Engine: Real-time mathematical calculation of Total Salary, Total Expenses, and Remaining Balance.

Validation Protocols: Prevents negative number injections and empty string submissions natively.

UI/UX Enhancements

Custom Toast Notifications: Replaced default browser alerts() with a modern, animated notification system.

Data Visualization: Dynamic Doughnut chart rendering Remaining Balance vs. Total Expenses.

Threshold Alerts: A reactive UI warning banner that triggers immediately when the remaining balance drops below 10% of the base salary.

Smart Search Modal: A custom modal with a search bar allowing users to find and select currencies (alphabetically sorted, with INR strategically pinned to the top).

Data Persistence & Export

Persistent Memory: Complete state retention across browser reloads using LocalStorage.

Dynamic Deletion: Trash icon functionality that instantly removes items from the DOM, updates LocalStorage, and recalculates the dashboard.

PDF Report Generation: One-click download of a formatted financial ledger containing the user's current state.

Technical Highlights

Vanilla State Management

The interface updates dynamically across multiple components using strict Vanilla JavaScript (ES6+), bypassing the need for frameworks like React or Angular.

Data Persistence (LocalStorage)

Data arrays and current currency states are serialized via JSON.stringify and saved to the browser's LocalStorage, ensuring user data survives page reloads.

Memory Leak Prevention

Chart.js instances are programmatically destroyed (.destroy()) before re-rendering, preventing canvas duplication bugs and browser memory leaks.

Native Array Manipulation

The application fetches 160+ global currencies, dynamically sorts them alphabetically using .sort(), and utilizes .findIndex() and .splice() to prioritize specific currencies (like INR) to the top of the UI list.

APIs Used

ExchangeRate-API (open.er-api.com): Fetches live global exchange rates using USD as the base anchor to facilitate real-time, accurate financial conversions across 160+ world currencies without requiring an API key.

Technologies Used

HTML5

Tailwind CSS (via CDN)

JavaScript (Vanilla JS)

Chart.js (Data Visualization)

jsPDF (Report Generation)

Lucide Icons

Testing

To evaluate functionality and persistence:

Open the application and input a base salary and multiple expenses.

Verify the mathematical logic and the pie chart distribution.

Refresh the page (Ctrl+R or Cmd+R) to verify that all data successfully loads from LocalStorage.
