# CSL Management Console

Visual production-management demonstration built from the CSL Order Management Trello board.

## Demo

GitHub Pages is configured to deploy from main, root. index.html is served directly; .nojekyll disables Jekyll processing.

## Features

- Executive overview with selectable charts and management attention queues
- All 149 captured job cards across 38 exact production phases
- Search, filters, pagination and CSV export
- Job details with direct original Trello card links
- Packing and dispatch queue and explicit data/automation status
- Responsive layout and keyboard-accessible native controls

## Data accuracy

Snapshot captured approximately 20 October 2026 at 04:29 UTC+8. Updates are manual; no live API connection or workflow is active. Card counts are not garment quantities. Archived cards and historical shipment totals are excluded. Empty Shipped list does not establish zero historical shipments. Phase leads are derived from list names, not individual card assignments. Unknown due dates, owners, quantities and next actions remain explicitly unavailable. The DMV Stars detail was individually inspected in Trello earlier in this session.

Two UDDINGSTON sample cards share a title; both are retained. No revenue, staff performance or delivery-risk scores are invented.

## Live integration

Configure a server-side Trello connection after workspace membership/app credentials are available. Keep tokens out of this public repository and the browser. Read lists/cards/custom fields/activity server-side, display last successful sync and stale/error states, and add refresh/webhooks as appropriate. Write-back and email-triggered workflow rules require separate implementation, permissions and testing.

## Deployment / maintenance

No dependencies or build step. index.html embeds the snapshot for a self-contained demo. data.json is the captured source dataset. Updating only data.json does not change the deployed page; replace the snapshot-data JSON block in index.html as part of a deliberate snapshot update. Never display a manual refresh as live sync.

## Validation

Verified 149 source card URLs, aggregate counts and JavaScript syntax. Managed local browser preview was unavailable due to a container mount restriction; hosted visual QA must be performed separately.
