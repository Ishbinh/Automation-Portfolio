# AI-Powered Telegram Support Agent

An n8n workflow that turns a Telegram bot into a lightweight AI support agent — classifying incoming messages by intent and routing each one to the right action, backed by a custom FastAPI + SQLite service.

## 📌 What It Does

Every message sent to the bot is classified into one of three intents using few-shot prompting with the Gemini API, then routed automatically:

- 🎫 **SUPPORT_REQUEST** → logs a new ticket to a custom FastAPI + SQLite backend and sends the user a confirmation.
- 🔍 **DATA_LOOKUP** → extracts a ticket ID from the message and retrieves its current status from the same backend.
- ❓ **FAQ_QUESTION** → answers directly using a Gemini LLM call grounded in a provided FAQ context.

Each path replies back to the user on Telegram, so the whole loop — message in, classification, action, response — runs without manual intervention.

## 🧩 Architecture

```text
Telegram Trigger
      │
      ▼
HTTP Request (Gemini — intent classification, few-shot prompt)
      │
      ▼
Code Node (parses model output into {intent, entity} JSON)
      │
      ▼
   Switch Node
   ┌────────┼────────┐
   ▼        ▼         ▼
SUPPORT  DATA_LOOKUP  FAQ_QUESTION
REQUEST      │            │
   │         ▼            ▼
   ▼    GET /tickets/{id}  HTTP Request (Gemini — FAQ-grounded answer)
POST /tickets  │            │
   │         │            │
   ▼         ▼            ▼
        Telegram reply (per branch)


```



# Technologies
n8n (workflow orchestration)

Google Gemini API (intent classification + FAQ answering)

FastAPI (custom backend service)

SQLite (ticket storage)

Telegram Bot API

# Workflow

<img width="1603" height="756" alt="image" src="https://github.com/user-attachments/assets/bb292299-7c82-4be6-9ba0-94631b91a9ca" />
