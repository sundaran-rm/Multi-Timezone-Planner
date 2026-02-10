# Multi‑Timezone Meeting Planner

A single‑page HTML app to plan meetings across multiple time zones and participants, with a consolidated participant‑centric schedule.

## Features

- Multiple meeting records (each with its own date, time, and base time zone).
- Shared participant list with editable names and time zones.
- Consolidated table that shows, for each meeting and participant:
  - Meeting number
  - Participant name
  - Participant time zone
  - Local date (with weekday)
  - Local time in 12‑hour AM/PM format
- Daylight saving aware, using IANA time zones via `Intl.DateTimeFormat`.
- Collapsible Participants and Meetings sections to keep the table in view.
- Escape key collapses all sections.

## Getting Started

1. Create a file named `index.html` in your project.
2. Paste the full HTML below into `index.html`.
3. Open the file in any modern browser (Chrome, Edge, Firefox, Safari).

## Usage

1. **Participants section**
   - Expand the Participants panel.
   - Add participants with names and select their home time zones.
   - You can remove participants; the table updates automatically.

2. **Meetings section**
   - Expand the Meetings panel.
   - Add one or more meeting records with:
     - Date
     - Time (24‑hour input, displayed as AM/PM)
     - Base time zone
   - Remove records as needed.

3. **Consolidated table**
   - View all meetings and participants in one table.
   - Each row shows the time converted to the participant’s local time zone, including weekday.

4. **Keyboard shortcut**
   - Press `Esc` to collapse all collapsible sections at once.

## Technologies

- Plain HTML, CSS, and JavaScript (no frameworks).
- `Intl.DateTimeFormat` with IANA time zones for robust date/time and DST handling.
