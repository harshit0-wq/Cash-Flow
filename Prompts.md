AI Prompt Engineering & Development Log

This document records the major prompts and development decisions used during the implementation of the Cash-Flow Dashboard for Sprint 02.

Prompt 01: Project Objective

Purpose:

Understand the Sprint 02 requirements and deliverables

Design and develop a functional financial dashboard using Vanilla JavaScript

Implement core logic, DOM manipulation, and data persistence

Consolidate all features into a single-file implementation

Prompt 02: Theme Selection & Interface Design

Purpose:

Define the website colour palette (Tailwind Slate, Blue, and Green for financial tracking)

Maintain brand consistency and trust throughout the interface

Create a visually appealing and professional dashboard layout

Ensure readability and accessibility across all input forms and data visualizations

Apply consistent styling to buttons, expense cards, and navigation elements

Prompt 03: Global Currency API Integration

Purpose:

Identify a reliable, free, and keyless API (open.er-api.com) to fetch live global exchange rates

Expand the currency conversion feature to support 161 world national currencies

Ensure accurate mathematical conversions across the dashboard using USD as a base anchor

Prompt 04: Array Manipulation & UI Sorting

Purpose:

Enhance the user experience of the currency search modal

Utilize Vanilla JavaScript native array methods (.sort(), .findIndex(), .splice(), .unshift())

Alphabetize the global currency list dynamically while strategically pinning INR (Indian Rupee) to the top for quick access

Prompt 05: Professional Presentation & User Experience Refinement

Purpose:

Enhance the overall visual presentation of the dashboard (e.g., Chart.js styling, custom Toast notifications)

Establish a professional and modern design language

Improve layout consistency, spacing, and typography

Refine user interactions, including the PDF export generation and warning threshold alerts

Ensure the final deliverable aligns with industry-standard web engineering practices

Outcome:

Improved visual hierarchy and readability of financial data

More polished and professional user interface without relying on default browser alerts

Better user engagement through interactive visual feedback (pie charts and smooth transitions)

Consistent presentation and state persistence across all browser sessions

Summary

The final implementation evolved through multiple development iterations focused on project planning, core JavaScript logic design, external API integration, single-file architecture, and professional user interface refinement. The resulting solution is a responsive, self-contained dashboard built using HTML, Tailwind CSS, Vanilla JavaScript, Chart.js, and jsPDF, maintaining seamless data persistence and an exceptional user experience.
