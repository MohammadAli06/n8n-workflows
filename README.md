# n8n Workflows 🚀

This repository contains my personal automation workflows built with **[n8n](https://n8n.io)** — a powerful, fair-code workflow automation tool.

---

## 📌 Workflow: Interview Scheduler

### 🔹 Description

This workflow automates the **interview scheduling process**. It helps streamline booking meetings by handling incoming requests, checking availability, creating calendar events, and sending confirmations — saving hours of back-and-forth emails.

Perfect for recruiters, hiring managers, or anyone who regularly schedules technical or HR interviews.

---

### 🧠 Workflow Logic (Simple Explanation)

1. **Trigger** — Receives a new interview request (via webhook, form, email, or chat)
2. **Availability Check** — Checks your calendar for free slots
3. **Processing** — Extracts candidate details and suggests or books a suitable time
4. **Action** — Creates a calendar event + sends confirmation (email or message)
5. **Optional** — Logs the booking or updates a tracker (Google Sheets, etc.)

*(You can expand this section once you add more details about your exact nodes)*

---

### 🖼️ Workflow Preview

![Interview Scheduler Workflow](images/interviewSched-preview.png)

---

### 📊 Simple Flow Diagram
Candidate Request
↓
Webhook / Trigger
↓
Extract Details + Check Availability
↓
Book Slot in Google Calendar (or similar)
↓
Send Confirmation + Log Booking


---

### ⚙️ How to Use / Setup Steps

1. Clone or download this repository
2. Open your n8n instance
3. Go to **Workflows → Import from File**
4. Select the file: `workflows/interview-scheduler.json`
5. Configure credentials:
   - Google Calendar (or your calendar service)
   - Email service (Gmail / SMTP)
   - Any other services used (Webhook, Sheets, etc.)
6. Activate the workflow
7. Test with a sample request

---

### 📂 Project Structure
n8n-workflows/
├── workflows/
│   └── interview-scheduler.json
├── images/
│   └── workflow-preview.png
└── README.md


---

### 🔌 Services / Integrations Used

- **n8n Core**
- Google Calendar (availability + event creation)
- Gmail / Email (confirmations)
- Webhook (for incoming requests)
- *(Add any others you are using, e.g., Google Sheets, OpenAI, Telegram, etc.)*

---

### 🚀 Future Plans

- Add AI-powered slot suggestions (using GPT)
- Support candidate self-booking via a simple form
- Automatic reminders before interviews
- Integration with ATS (Applicant Tracking System)
- Error handling & notifications for failed bookings

---

### 📝 Notes

- This is my first n8n workflow in this repo. More automations will be added soon.
- Feel free to fork, improve, or use it as a base for your own scheduling needs.
- If you face any issues importing or running it, open an issue!

---

Made using **n8n**

---
