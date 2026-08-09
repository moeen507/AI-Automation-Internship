# MATalogics AI Automation Internship - Day 03 Report

**Student Name:** Moeen Ahmad Butt  
**GitHub Repository:** https://github.com/moeen507/AI-Automation-Internship  
**Open Source Repository:** https://github.com/enescingoz/awesome-n8n-templates  
**Date:** 9 August 2026

## Assignment Overview

Day 03 covers Git and GitHub fundamentals, REST API concepts, HTTP methods and status codes, Postman, and a Lead Management API built with n8n webhooks and Google Sheets.

## Git & GitHub

Commands covered: `git config`, `git init`, `git clone`, `git add .`, `git commit`, `git push`, `git pull`, and feature-branch workflow commands.

Open-source project selected: `enescingoz/awesome-n8n-templates`, which is relevant to n8n, AI automation, workflow orchestration, Google Sheets, RAG, and API-driven automation.

## API Fundamentals

- **API:** an interface that lets software systems request data or actions from each other.
- **REST API:** an HTTP-based resource-oriented API style.
- **GET:** retrieve data.
- **POST:** create data.
- **PUT:** update data.
- **DELETE:** remove data.
- **Status codes:** 200, 201, 400, 401, 404, 500.
- **Headers:** Content-Type, Authorization, Accept.
- **Authentication:** API Keys and Bearer Tokens.

## APIs Implemented

| Method | Endpoint | Purpose |
|---|---|---|
| POST | `/create-lead` | Validate and create a lead |
| GET | `/get-leads` | Return all leads |
| PUT | `/update-lead` | Update a lead using email as the matching field |
| DELETE | `/delete-lead` | Delete a lead using email as the matching field |

## Workflow Overview

All sub-workflows are contained in one n8n workflow.

1. Create Lead: Webhook -> Validate Data -> Google Sheets Append Row -> Respond to Webhook.
2. Get Leads: Webhook -> Google Sheets Read Rows -> Respond to Webhook.
3. Update Lead: Webhook -> Validate Email -> Google Sheets Update by Email -> Respond to Webhook.
4. Delete Lead: Webhook -> Validate Email -> Google Sheets Delete by Email -> Respond to Webhook.

## Google Sheets Structure

`Name | Email | Phone | Company | Interest | Created At`

## Postman

The repository includes an importable Postman collection with all four requests and an environment file using the `base_url` variable.

## Learning Outcomes

- Git/GitHub project organization and command workflow.
- REST API request/response concepts.
- HTTP methods, headers, status codes, and authentication basics.
- n8n webhook-based CRUD API architecture.
- Google Sheets persistence for lead data.
- Postman variables and CRUD endpoint testing.
- Data validation and email-based record matching.

## Evidence Status

Execution screenshots must be captured from the live Postman, n8n, and Google Sheets interfaces after credentials are connected and the webhooks are executed. No fake execution screenshots or fake pull-request evidence are included.
