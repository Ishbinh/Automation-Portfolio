## 📌 Objective
Learn how Webhooks work by receiving data from an external application (Postman) and triggering different actions based on the payment status.


## 🛠️ Workflow Built

Webhook → Switch → Gmail

The workflow receives a POST request through a Webhook. Based on the **payment_status** received, the Switch node routes the execution to one of three Gmail nodes:

- ✅ Paid → Order Confirmation Email
- ⏳ Pending → Payment Pending Email
- ❌ Failed → Payment Failed Email


## 📚 Concepts Learned

- What a **Webhook** is and how it receives data.
- Difference between **HTTP Request** (sending data) and **Webhook** (receiving data).
- Sending a **POST request** from Postman.
- Using a **Switch** node to route workflows based on incoming data.
- Difference between **Test URL** and **Production URL**.
- Webhooks make workflows **event-driven**. Instead of repeatedly checking whether something has happened, another application sends data to the workflow whenever an event occurs, allowing automations to run instantly.

<img width="1626" height="796" alt="image" src="https://github.com/user-attachments/assets/74570616-219d-4c3e-9219-8bbd4f6a8203" />

