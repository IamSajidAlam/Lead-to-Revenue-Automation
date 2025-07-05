# 🔁 Lead-to-Revenue Automation (n8n Workflow)

This project provides an automated **Lead-to-Revenue** workflow built with [n8n](https://n8n.io). It streamlines the process from lead capture to nurturing, scoring, qualification, and monetization.

---

## 📌 Features

- 🌐 Captures incoming leads via webhook
- 🧹 Cleans and standardizes lead data
- 📊 Scores leads based on job title, company, and email domain
- 🔄 Prevents duplicate entries
- ✅ Automatically qualifies and nurtures high-quality leads
- 📬 Sends personalized emails via Gmail
- 💰 Generates Stripe payment links
- 📈 Logs all activities in Google Sheets for analytics

---

## 🗂 Folder Structure

```
lead-to-revenue-automation/
│
├── workflows/
│   └── Lead-to-Revenue-Automation.json  # n8n exported workflow
│
├── assets/
│
├── README.md
└── LICENSE
```

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/lead-to-revenue-automation.git
cd lead-to-revenue-automation
```

### 2. Import Workflow into n8n

- Open your n8n instance
- Go to **Workflows → Import from File**
- Select `workflows/Lead-to-Revenue-Automation.json`

### 3. Set Up Required Credentials

> ⚠️ This workflow uses the following integrations. Ensure these are configured in your n8n credentials:

- **Google Sheets OAuth2** — for storing leads and logs
- **Gmail OAuth2** — for sending follow-up emails
- **Stripe API** — for creating payment links

### 4. Define Webhook Endpoint

Webhook will be triggered by sending a POST request to:

```
https://your-n8n-domain/webhook/lead-capture
```
