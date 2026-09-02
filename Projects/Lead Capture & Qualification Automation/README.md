# Typeform → n8n Lead Capture & Qualification Automation

An end-to-end lead automation workflow built with **Typeform, n8n, HubSpot API, and Excel**.

## Workflow

**Typeform → Webhook → Data Processing → Budget Qualification → Routing**

* Captures lead information through a Typeform webhook
* Extracts and processes submitted form data
* Classifies leads based on their budget
* Sends qualified/high-budget leads to **HubSpot** via HTTP API
* Triggers a notification for qualified leads
* Stores lower-budget leads in **Excel** for later follow-up

## Tech Stack

* n8n
* Typeform
* HubSpot REST API
* Microsoft Excel
* Webhooks
* JSON & conditional logic

## Key Learning

* Webhook-based integrations
* Data transformation in n8n
* Conditional branching
* REST API integration
* End-to-end workflow testing and deployment

## Workflow Preview

<img width="1572" height="782" alt="image" src="https://github.com/user-attachments/assets/ed3e8cdc-375b-4a26-a524-97daaa7bfc5a" />
<img width="1600" height="596" alt="image" src="https://github.com/user-attachments/assets/47eb59b5-53a7-4404-8aee-5b1d8d3ff8ae" />


> Built and tested with multiple Typeform submissions to validate both qualification paths.
