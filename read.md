# B2B Lead Generation Automation (n8n)

An automated B2B lead generation system built using n8n that collects, enriches, and stores business leads from multiple sources into Google Sheets / CRM for outreach and sales.

---

## 🚀 Overview

This workflow automates the process of:

- 🔍 Collecting B2B leads from online sources
- 📊 Extracting company & contact information
- 🤖 Enriching data using AI
- 📁 Storing leads in Google Sheets / CRM
- 📩 Preparing leads for email outreach

Designed for freelancers, agencies, and startups.

---

## 🏗️ Architecture

Lead Source (API / Scraper / Form)
        ↓
Webhook Trigger (n8n)
        ↓
Data Cleaning & Formatting
        ↓
AI Enrichment (OpenAI)
        ↓
Google Sheets / CRM Storage
        ↓
(Optional) Email Outreach Automation

---

## 🛠️ Tech Stack

- n8n (Workflow Automation)
- OpenAI API (Lead Qualification & Enrichment)
- Google Sheets (Lead Storage)
- Webhooks
- HTTP Request Nodes
- CRM Integration (Optional)

---

## 📌 Features

- Automated lead collection
- Company data extraction
- AI-based lead qualification
- Contact info formatting
- Duplicate filtering
- Google Sheets integration
- CRM-ready structured output
- JSON API support

---

## ⚙️ Setup Instructions

### 1️⃣ Clone Repository

```bash
git clone https://github.com/yourusername/b2b-lead-generation-n8n.git
cd b2b-lead-generation-n8n
2️⃣ Install n8n
Using npm:

npm install n8n -g
n8n
Or using Docker:

docker run -it --rm \
  -p 5678:5678 \
  -v ~/.n8n:/home/node/.n8n \
  n8nio/n8n
3️⃣ Import Workflow
Open n8n

Click "Import Workflow"

Upload the provided JSON workflow file

4️⃣ Configure Credentials
Set up credentials for:

OpenAI API

Google Sheets

Any external Lead API (if used)

Make sure OpenAI billing is enabled.

📡 Example Lead Output
{
  "company_name": "TechNova Solutions",
  "industry": "Software Development",
  "website": "https://technova.com",
  "contact_email": "info@technova.com",
  "location": "India",
  "lead_score": 82,
  "qualification": "High Potential Client"
}
🧠 How It Works
Leads are collected via webhook or API.

Data is cleaned and standardized.

OpenAI enriches and scores the lead.

Lead is stored in Google Sheets / CRM.

Optional: Trigger email outreach sequence.

🎯 Use Cases
Digital Marketing Agencies

SaaS Startups

Freelancers

Sales Teams

Recruitment Agencies

🔮 Future Improvements
LinkedIn scraping integration

Automated cold email sender

Lead scoring dashboard

CRM integration (HubSpot, Zoho, Salesforce)

Multi-source scraping support

👨‍💻 Author
Shaikh Aaiyub