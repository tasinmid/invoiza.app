# Frontend Blueprint: Invoiza API Tester (Current State)

This document outlines the current architecture and components of the Invoiza frontend application. It reflects the latest design iterations, including the template selection, month tag input, and robust validation.

## 1. Architecture

The frontend is built on a clean, modern stack:

-   **Layout:** A responsive two-pane layout separates configuration (left) from dynamic data entry and results (right).
-   **Frameworks:** Bootstrap 5 for the grid system and base components, with Bootstrap Icons for clear iconography.
-   **Styling:** A modular, dark-theme-first CSS architecture. Styles are split into `base.css` (theme variables, global styles), `form.css` (custom form controls, conditional UI animations), and `components.css` (specific UI components).
-   **JavaScript (ES6+):** Vanilla JS is used for all client-side interactivity. Logic is separated into `script.js` (UI logic) and `api.js` (backend communication).

## 2. Key Features & Functionality

-   **Template Selection**: Users can select an invoice template from a dropdown menu, with a live preview image.
-   **Dynamic Payment Fields**: Input fields for different payment methods (Bank Details, PayPal, Payment Link, Other) dynamically appear/disappear with smooth transitions based on user selection.
-   **Frontend Validation**: Real-time validation for Swift Code (8-11 letters), PayPal Email (valid email format), and Payment Link (valid URL format).
-   **Monthly Invoice Item Selector**: For monthly invoices, users can select months using a tag-based input with a dropdown, allowing up to 12 months to be added.
-   **Invoice Item Management**: Users can add and remove invoice items dynamically.
-   **Send Type Options**: Users can choose to download a PDF, email a PDF, or email HTML, with conditional display of a recipient email field.

## 3. File Structure

```
frontend/
├── css/
│   ├── base.css
│   ├── components.css
│   └── form.css
├── api.js               # Handles all communication with the backend API
├── index.html           # The main HTML file
└── script.js            # Core application logic and UI interaction
└── BLUEPRINT.md         # This file
```

## 4. Current State

The frontend is fully functional with all the features described above. All known issues have been addressed.
