Automated Lead Capture & CRM Routing System

## Objective

Built an end-to-end business automation workflow in n8n that receives customer leads through a webhook, processes the incoming data, routes high-value leads to a CRM, and handles API failures gracefully.


## Workflow

Webhook

Parse Lead Data

IF (Budget > Threshold?)

YES
 
HTTP Request (HubSpot CRM API)
  
--Success → Gmail Notification

--Failure → Error Email

NO

Google Sheets (Store Standard Leads)


## Technologies Used

- n8n
- HubSpot CRM REST API
- HTTP Request Node
- Gmail Node
- Webhook
- IF Node
- Edit Fields
- JSON


## Workflow Explanation

### 1. Webhook

Receives incoming lead information as JSON.


### 2. Edit Fields

Extracted only the required information from the incoming payload.


### 3. IF Node

Business rule:

If Budget > 50000

Route to CRM.

Else

Store as a standard lead.


### 4. HTTP Request

Instead of using the built-in HubSpot connector, integrated directly with the HubSpot REST API.


### 5. Success Path

If the contact is successfully created:

Send a confirmation email using Gmail.


### 6. Error Handling

Implemented real-world error handling.

If the CRM API fails because of:

- Invalid Authentication
- Bad Request
- Missing Required Fields
- API Errors

The workflow follows the Error output and sends an error notification email instead of silently failing.

This improves reliability and makes troubleshooting easier.


### 7. Standard Leads

Leads below the budget threshold are routed to Google Sheets for future follow-up.

<img width="1672" height="866" alt="image" src="https://github.com/user-attachments/assets/7f9ad0fe-655f-4e3c-a1ec-9556fb88dcd4" />
