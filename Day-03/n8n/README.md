# n8n Lead Management Workflow

Import `Lead Management Workflow.json` into n8n.

## Live Google Sheet

The workflow is already configured to use the live **Lead Management** spreadsheet:

https://docs.google.com/spreadsheets/d/1liSm00d1WfLrNkpwPvpr0K-kqcLuwMvtU5xC7VP_hD0/edit

Sheet tab: `Leads`

Required columns: `Name`, `Email`, `Phone`, `Company`, `Interest`, `Created At`.

## Remaining n8n configuration

- Select your authorized Google Sheets OAuth2 credential on each Google Sheets node after import.
- Activate the workflow before using production webhook URLs.
- Copy the production webhook base URL into the Postman `base_url` environment variable.

## Endpoints

- `POST /create-lead`
- `GET /get-leads`
- `PUT /update-lead`
- `DELETE /delete-lead`

All four endpoint branches are contained inside one workflow, as required by the Day-03 assignment.
