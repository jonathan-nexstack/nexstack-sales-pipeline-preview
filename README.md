# SalesFlow Tracker

A browser-based sales pipeline tracker for monitoring personal and team sales progress.

## How to use

1. Open `index.html` in Chrome, Edge, or Safari.
2. Click **+ Add Deal** to add a sales opportunity.
3. Use **Pipeline Board** for stage tracking.
4. Use **Activities** to log calls, WhatsApp, meetings, demos, and proposal updates.
5. Use **Dashboard** and **Team Performance** for sales reviews.
6. Click **Export CSV** to download the deal list.

## Data storage

This MVP stores data in the browser's `localStorage`. It works offline and requires no server.

For a team-shared version, the next upgrade should connect this same UI to Supabase/PostgreSQL with login roles.

## Built-in features

- Deal management
- Owner assignment
- Pipeline stages
- Dashboard metrics
- Weighted sales forecast
- Follow-up reminders and overdue flags
- Kanban pipeline board
- Activity log
- Team performance cards
- Monthly manager summary
- CSV export

## Upgrade notes

- Deal cards can now be moved by drag-and-drop between Pipeline Board columns.
- Drag-and-drop changes the stage only; probability is preserved for normal stages and only auto-set for Won (100%) or Lost (0%).
- Add Deal supports Prospecting by leaving Deal Value and/or Probability % blank. Blank values are excluded from pipeline value/forecast until updated.
- Lead Source now includes Others.
- First meeting status/date and qualification status were added for early-stage leads where sales has not met the client yet.
