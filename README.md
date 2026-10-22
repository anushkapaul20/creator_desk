# Creator Desk

Creator Desk is a local-first workspace for creator discovery, outreach, campaign planning, deliverable tracking, and personalized DM and email templates.

## Run locally

No API keys or paid services are required. Serve this folder with any static HTTP server. For example:

```powershell
python -m http.server 4173
```

Then open [http://localhost:4173](http://localhost:4173).

## Features

- Dashboard metrics and charts are calculated from workspace records.
- Creator profiles with search, filters, CRUD forms, profile links, and CSV export.
- Outreach status tracking, follow-up dates, and response-rate calculation.
- Campaign planning with progress based on published deliverables.
- Deliverable deadlines, approvals, publication links, and payment statuses.
- Ten editable outreach templates with creator and campaign personalization.
- Local browser storage, JSON backup and restore, and sample demo records.

## Data and privacy

Workspace records are stored in the current browser using `localStorage`. They are not sent to a backend. Use **Settings → Download backup** to keep a portable copy of your workspace.

The response rate is the number of contacted outreach records with a reply or subsequent response status divided by the total number of contacted outreach records. Records with **Not Contacted** status are excluded.

Campaign progress is the number of published deliverables divided by the total number of deliverables recorded for that campaign. Campaigns with no deliverables have no calculated progress percentage.
