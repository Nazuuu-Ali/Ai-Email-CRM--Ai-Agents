# 🤖 Autonomous AI-Powered Email CRM & Smart Notification Agent

An intelligent, multi-platform AI workflow built with **n8n**, **Groq AI (Llama 3)**, **Supabase PostgreSQL**, **Gmail API**, and **WhatsApp Cloud API**. 

This system automatically triages incoming business emails, evaluates urgency scores using Large Language Models, generates intelligent auto-responses, logs interaction histories securely, and dispatches instant WhatsApp notifications for high-priority inquiries.

---

## 🏗️ System Architecture

```text
[ Incoming Email ] 
       │
       ▼
[ Gmail API Trigger ] ──► [ Groq AI Llama-3 Model ]
                               │ (Evaluates Urgency & Sentiment)
                               ├──────────────────────┐
                               ▼                      ▼
                     [ Low/Medium Priority ]   [ High/Urgent Priority ]
                               │                      │
                               ▼                      ▼
                     [ Auto-Draft / Reply ]    [ WhatsApp Cloud Alert ]
                               │                      │
                               └──────────┬───────────┘
                                          ▼
                               [ Supabase PostgreSQL & ]
                               [ Google Sheets Audit Log ]


✨ Key Features
📩 Automated Email Ingestion: Real-time processing of inbound emails via Gmail API.

🧠 Groq AI Sentiment & Urgency Analysis: Sub-second latency LLM evaluation using Groq to categorize emails by priority (Urgent, High, Normal, Low).

📱 Instant WhatsApp Alerts: Immediate notification dispatch via WhatsApp Cloud API for time-sensitive lead or support requests.

✍️ Context-Aware Auto-Drafting: Smart AI response drafting for standard low-priority queries.

💾 Dual Audit Logging: Structured logging into Supabase PostgreSQL for CRM analytics and Google Sheets for real-time tracking.

⚙️ Production-Ready & Modular: Fault-tolerant n8n nodes with customizable conditional routing.

🛠️ Tech Stack
Workflow Orchestration: n8n

AI Model Engine: Groq Cloud API (Llama 3)

Database & CRM Persistence: Supabase (PostgreSQL)

Messaging & Alerts: WhatsApp Cloud API / Green-API

Email & Spreadsheets: Gmail API, Google Sheets API
📂 Repository Structure.
.
├── workflows/
│   └── email_crm_agent.json   # Exported n8n workflow
├── .gitignore
└── README.md

🚀 Quick Setup & Installation
1. Prerequisites
Active n8n instance (Cloud or Self-Hosted)

Groq API Key

Supabase Database project

Gmail API Credentials (OAuth2)

WhatsApp Cloud API credentials

2. Import Workflow
Download the workflows/email_crm_agent.json file from this repository.

Open your n8n canvas.

Click on Workflow Menu > Import from File.

Select email_crm_agent.json.

📬 Contact & Professional Services
Looking to implement custom AI agents, n8n automations, or enterprise CRM workflows for your business?

💼 Fiverr Service: https://www.fiverr.com/s/bkkyP7N

🔗 LinkedIn:https://www.linkedin.com/in/nazakat-ali-ai
lets connect

