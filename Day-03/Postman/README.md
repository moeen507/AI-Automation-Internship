# Postman Setup

1. Import `MATalogics Lead Management API.postman_collection.json`.
2. Import `Environment.postman_environment.json`.
3. Select the environment.
4. Replace `base_url` with the production n8n webhook base URL, for example `https://your-n8n-host/webhook`.
5. Run requests in this order for a complete CRUD test:
   - POST - Create Lead
   - GET - Get All Leads
   - PUT - Update Lead
   - GET - Get All Leads
   - DELETE - Delete Lead
   - GET - Get All Leads

Required header for JSON request bodies: `Content-Type: application/json`.
