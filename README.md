# Cash-Flow Dashboard — Salary & Expense Tracker (Sprint 02)

A responsive and dynamic financial dashboard built to track salaries and manage expenses. This project was developed as part of Sprint 02 to demonstrate core JavaScript concepts including DOM manipulation, event handling, state management, and data persistence using Vanilla JavaScript without relying on frontend frameworks.

## Live Deployment

**Live Demo:** [Add Deployment URL Here]

---

## Features

### Core MVP

* Dedicated forms for capturing salary and expense information.
* Real-time calculation of:

  * Total Salary
  * Total Expenses
  * Remaining Balance
* Input validation to prevent empty submissions and invalid values.
* Dynamic rendering of expense items directly to the DOM.

### Data Persistence & State Management

* Complete application state persistence using LocalStorage.
* Automatic restoration of salary, expenses, and user preferences after page reloads.
* Instant recalculation of balances after any state update.
* Dynamic expense deletion with synchronized LocalStorage updates.

### Visualization & Alerts

* Interactive Doughnut Chart displaying Remaining Balance versus Total Expenses.
* Threshold-based financial alerts:

  * Warning state when balance falls below 10% of total salary.
  * Critical alert state when expenses exceed available funds.
* Real-time visual feedback as financial data changes.

### Currency Management

* Integrated global currency support using live exchange rates.
* Searchable currency selection modal for improved usability.
* Alphabetically sorted currency list with frequently used currencies prioritized.
* Real-time currency conversion throughout the dashboard.

### Report Generation

* Export financial reports directly as PDF documents.
* Unicode-compatible currency rendering including symbols such as ₹, $, €, and £.
* Professionally formatted reports for record keeping and sharing.

---

## Technical Highlights

### Vanilla JavaScript State Management

The dashboard updates multiple UI components in real time using native JavaScript, demonstrating manual state management without frameworks such as React or Angular.

### LocalStorage Integration

Application data is serialized using `JSON.stringify()` and restored using `JSON.parse()` to maintain state persistence across browser sessions.

### Chart Lifecycle Management

Chart.js instances are properly updated and destroyed before re-rendering to prevent duplicate canvas instances and unnecessary memory usage.

### Array Manipulation

The application utilizes native array methods including:

* `.sort()`
* `.findIndex()`
* `.splice()`
* `.unshift()`

to manage expense records and currency ordering efficiently.

---

## APIs Used

### ExchangeRate-API

* Fetches live exchange rates for global currencies.
* Enables real-time currency conversion.
* Supports international financial calculations without requiring API keys.

### Google Fonts API

* Dynamically loads fonts required for Unicode-compatible PDF generation.
* Ensures proper rendering of international currency symbols within exported reports.

---

## Technologies Used

* HTML5
* Tailwind CSS
* Vanilla JavaScript (ES6+)
* Chart.js
* jsPDF
* Lucide Icons
* LocalStorage API

---

## Testing

To verify functionality:

1. Add a salary value and multiple expenses.
2. Verify that calculations update correctly.
3. Test threshold warnings by reducing the available balance.
4. Refresh the page and confirm LocalStorage persistence.
5. Export a PDF report and verify formatting.
6. Test currency switching and exchange rate updates.

---

## Conclusion

The final implementation combines financial tracking, state persistence, data visualization, PDF generation, and live currency conversion into a single self-contained application while demonstrating strong proficiency in Vanilla JavaScript and frontend engineering fundamentals.
