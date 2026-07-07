# Day 2 - Bakery Order Automation with Conditional Paths

## Project Overview

Built a bakery order processing workflow using Zapier that automatically stores customer orders and processes them differently based on the selected fulfillment method.

---

## Business Scenario

A bakery receives cake orders through a Google Form.

Every order should:

- Be stored in a central Google Sheet.
- Send a confirmation email to the customer.

However, if the customer selects **Delivery**, the bakery owner should also receive a notification to arrange delivery.

---

## Workflow

Google Forms

↓

Google Sheets (Store Order)

↓

Paths


Pickup
→ Customer Confirmation Email

Delivery
→ Customer Confirmation Email
→ Bakery Owner Notification Email

---

## Tools Used

- Google Forms
- Google Sheets
- Gmail
- Zapier Paths

---

## Trigger

New Google Form Response

---

## Actions

1. Create Spreadsheet Row
2. Evaluate Order Type
3. Pickup Path
    - Send Pickup Confirmation Email
4. Delivery Path
    - Send Delivery Confirmation Email
    - Notify Bakery Owner

---

## Business Logic

IF Order Type = Pickup

→ Send pickup confirmation

ELSE IF Order Type = Delivery

→ Send delivery confirmation

→ Notify bakery owner

---

## Concepts Learned

- Trigger vs Action
- Data Mapping
- Google Sheets Integration
- Conditional Branching (Paths)
- Multiple Actions in a Single Workflow
- Business Workflow Design

---

## Challenges Faced

- Mapping Google Form fields to Google Sheets.
- Understanding when to place Paths in the workflow.
- Designing different business processes for Pickup and Delivery.

---

## Outcome

Successfully automated bakery order processing with conditional business logic.

Orders are automatically:

- Stored in Google Sheets.
- Routed based on order type.
- Sent to the appropriate recipients.

---

## Proof

See the attached workflow screenshot.
<img width="1281" height="817" alt="image" src="https://github.com/user-attachments/assets/c9377e93-2644-416b-a11b-0666b228640c" />
