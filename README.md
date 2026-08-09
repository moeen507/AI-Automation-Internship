# AI Automation Internship

MATalogics Day 3 assignment covering Git & GitHub, API fundamentals, Postman, n8n webhooks, and Google Sheets-based lead management.

## Day 03 Scope

- Git and GitHub command practice
- Open-source repository exploration and contribution planning
- REST API fundamentals
- HTTP methods: GET, POST, PUT, DELETE
- HTTP status codes and headers
- API authentication basics
- Postman workspace, collection, variables, headers, and authorization
- n8n Lead Management API using webhooks
- Google Sheets as the lead data store

## Lead Management API

| Method | Endpoint | Purpose |
|---|---|---|
| POST | `/create-lead` | Validate input and append a new lead |
| GET | `/get-leads` | Return all stored leads |
| PUT | `/update-lead` | Find a lead by email and update fields |
| DELETE | `/delete-lead` | Find a lead by email and delete it |

## Repository Structure

```text
Day-03/
├── GitHub/
├── Postman/
├── n8n/
├── Google Sheets/
└── Report/
```

## Google Sheet Schema

`Name | Email | Phone | Company | Interest | Created At`

## Setup

1. Import the n8n workflow from `Day-03/n8n/Lead Management Workflow.json`.
2. Configure Google Sheets credentials in n8n.
3. Select your Lead Management spreadsheet in all Google Sheets nodes.
4. Activate the workflow and copy the production webhook base URL.
5. Import the Postman collection and environment.
6. Set `base_url` in Postman to your n8n webhook base URL.
7. Test POST, GET, PUT, and DELETE requests.

## Learning Outcomes

This project demonstrates REST-style CRUD operations, request validation, webhook-driven automation, API testing, structured data storage, and GitHub-based project documentation.
