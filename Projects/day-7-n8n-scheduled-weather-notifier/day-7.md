Scheduled Weather Notification (n8n)

## Overview

Built an automated weather notification workflow using **n8n**.

The workflow runs on a schedule, fetches live weather data from the Open-Meteo API, formats the response, and sends it as an email.

## Workflow

Schedule Trigger
→ HTTP Request (Open-Meteo API)
→ Edit Fields
→ Gmail

## Concepts Learned

- Schedule Trigger
- HTTP Request
- Working with REST APIs
- Reading JSON responses
- Expressions (`{{ }}`)
- Gmail OAuth Authentication

## Tech Stack

- n8n
- Gmail
- Open-Meteo API

## What I Learned

- Schedule Trigger runs workflows automatically at a specified time.
- HTTP Request nodes can fetch live data from external APIs.
- JSON values can be accessed using expressions.
- Gmail OAuth setup requires Google Cloud OAuth credentials (Client ID & Client Secret).
- Dynamic email content can be generated using expressions.

<img width="1452" height="652" alt="image" src="https://github.com/user-attachments/assets/1939cea8-55cd-4b5e-9ee6-e2735e93c87e" />
