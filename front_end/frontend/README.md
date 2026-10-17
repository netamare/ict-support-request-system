# OBN ICT Support Request System

Frontend-only academic service desk demonstration built with HTML, CSS, vanilla JavaScript and Bootstrap 5. The interface uses sample people and ticket records only.

## Run locally

Open `index.html` in a modern browser, or run `python -m http.server 8000` from the `frontend` folder and open `http://localhost:8000`. Bootstrap styling is loaded from its CDN and needs an internet connection; the application logic and custom styles are local.

## Demonstration features

- Responsive OBN-branded workspace with Overview, Requests, Technicians, Activity history and Reports.
- Dashboard summaries and status/priority charts calculated from stored tickets.
- Request creation, editing, assignment, status workflow, comments, cancellation confirmation and status history.
- Ticket search, combined status/priority/category filters, sorting, filter reset and detail views.
- Sample technician directory, skill/availability filters and open-ticket workload.
- In-app notifications with read/unread state and links to related tickets.
- Report date ranges, CSV download with spreadsheet-formula protection, and print layout.
- Persistent light/dark theme and confirmed reset of demo data.
- Existing request records under the previous prototype storage key are migrated when possible.

## Data and security limits

Requests, activity, notifications, sample technicians and theme preferences are saved in this browser's `localStorage`. Data is not synchronized between people or devices, is not encrypted, and can be cleared by the browser. This prototype does not provide secure authentication, server-side authorization, centralized multi-user access, email, push notifications or real-time technician availability. Do not store real employee, contact or confidential support information here.

Use **Reset demonstration data** in the profile menu to restore the illustrative sample tickets, activity and notifications. This permanently replaces this browser's current demo records after confirmation.

## Files

```text
frontend/
├── index.html       # App shell, navigation, forms and accessible dialogs
├── css/styles.css   # Theme, responsive layout, charts and print styles
├── js/app.js        # Data model, views, workflow, storage and reports
└── README.md        # Run instructions and prototype limitations
```
