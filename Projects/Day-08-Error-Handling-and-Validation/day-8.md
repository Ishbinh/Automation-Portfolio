# Day 8 - Error Handling & Validation in n8n

## Objective
Learn how to handle business errors using conditional branching instead of allowing an invalid workflow to continue.

## Workflow

Manual Trigger

→ Edit Fields

→ IF (paymentStatus == "Paid")

TRUE → Send Order Confirmation Email
FALSE → Send Payment Failed Email

## Scenario

Customer places an online order.

- If payment is **Paid**, send an order confirmation.
- If payment **Failed**, notify the customer that the payment was unsuccessful.

## What I Learned

- Built a business validation using the IF node.
- Used expressions to evaluate workflow data.
- Created separate success and failure paths.
- Prevented an invalid workflow from continuing.

## Why Error Handling Matters

Error handling prevents incorrect actions from being executed and ensures workflows respond appropriately when business rules are not met.

<img width="1400" height="767" alt="image" src="https://github.com/user-attachments/assets/4678c3bf-ab7c-4a38-a680-3383db311a03" />

