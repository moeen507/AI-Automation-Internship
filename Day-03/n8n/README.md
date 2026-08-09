# n8n Lead Management Workflow

Import `Lead Management Workflow.json` into n8n.

## Required configuration

- Connect your Google Sheets OAuth2 credential.
- Replace `REPLACE_WITH_GOOGLE_SHEET_ID` in each Google Sheets node with the ID of your Lead Management spreadsheet.
- Use the `Leads` sheet tab.
- Required columns: `Name`, `Email`, `Phone`, `Company`, `Interest`, `Created At`.
- Activate the workflow before using production webhook URLs.

## Endpoints

- `POST /create-lead`
- `GET /get-leads`
- `PUT /update-lead`
- `DELETE /delete-lead`

All four endpoint branches are contained inside one workflow, as required by the Day-03 assignment.
