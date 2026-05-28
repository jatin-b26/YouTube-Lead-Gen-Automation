# YouTube Lead Generation System

Automated workflow system for discovering, filtering, and contacting YouTube creators for video editing outreach.

**Status:** 🧪 Testing Phase

* ✅ WF1 Complete
* 🧪 WF2 In Testing
* ⏸️ WF3 Planned

---

# 📋 Overview

This system automates the lead generation and outreach pipeline using n8n workflows.

## Workflows

### WF1 — Channel Discovery

Searches YouTube for creators across selected niches and generates qualified leads.

### WF2 — Email Campaign Manager

Sends automated cold emails with rate limiting and status tracking.

### WF3 — Reply Monitor & Alerts *(Planned)*

Monitors replies and sends notifications.

---

# 🎯 Core Features

## Lead Discovery

* Searches 750+ videos per run
* Extracts ~50 qualified leads
* Uses YouTube Data API

## Email Extraction

* Multi-pattern regex extraction
* Obfuscated email detection
* Social handle fallback
* ~70–80% extraction rate

## Lead Filtering

* Subscriber threshold filtering
* Engagement ratio filtering
* Language detection
* Activity verification

## AI Email Generation

* AI-generated cold emails
* Niche-specific customization
* Professional tone enforcement
* Phrase filtering

## Outreach Automation

* Gmail API integration
* Daily sending limits
* Delayed sending intervals
* Automatic status updates
* Retry handling

---

# 🛠️ Tech Stack

| Component     | Technology               |
| ------------- | ------------------------ |
| Automation    | n8n                      |
| Lead Search   | YouTube Data API         |
| AI Generation | Groq API                 |
| Email Sending | Gmail API                |
| Data Storage  | Google Sheets            |
| Deployment    | Docker                   |
| Notifications | Telegram Bot *(planned)* |

---

# 📊 Metrics

| Metric              | Value          |
| ------------------- | -------------- |
| Leads Generated     | 60+            |
| Emails Generated    | 60+            |
| Daily Sends         | 10             |
| Search Volume       | 750 videos/run |
| Extraction Success  | 70–80%         |
| Runtime             | 15–20 min      |
| Infrastructure Cost | $0             |

---

# 📁 Project Structure

```text
project/
├── workflows/
├── scripts/
├── config/
├── docs/
└── README.md
```

---

# 🚀 Workflow Logic

```text
Trigger
  ↓
Fetch Leads
  ↓
Filter Qualified Leads
  ↓
Generate Email
  ↓
Send Email
  ↓
Update Status
  ↓
Wait / Rate Limit
```

---

# 📧 Sending Configuration

| Setting        | Value      |
| -------------- | ---------- |
| Daily Limit    | 10 Emails  |
| Delay          | 45 Seconds |
| Status Update  | Enabled    |
| Sending Method | Gmail API  |

---

# 🎯 Supported Niches

* Real Estate
* Finance
* Business
* AI
* Law

---

# 📊 Lead Status System

| Status    | Meaning           |
| --------- | ----------------- |
| New       | Not contacted     |
| Contacted | Email sent        |
| Replied   | Response received |
| Closed    | Completed         |
| Blacklist | Ignored lead      |

---

# ⚙️ Filtering Logic

```json
{
  "minSubscribers": 5000,
  "minEngagementRatio": 3,
  "maxEngagementRatio": 40
}
```

---

# 🔍 Email Extraction Patterns

Supported formats:

* `name@domain.com`
* `name[at]domain[dot]com`
* `name @ domain . com`
* Footer emails
* Social handle fallback

---

# 📈 KPIs

## Lead Quality

* 5K–392K subscriber range
* 3–35% engagement range

## Outreach Targets

* Bounce Rate: <2%
* Open Rate: >15%
* Reply Rate: >3%

---

# 🚦 Roadmap

## Current

* Finish WF2 testing
* Verify deliverability
* Improve error handling

## Planned

* Reply monitoring
* Telegram alerts
* Analytics dashboard
* A/B testing
* CRM integration

---

# 📌 Current Status

**Last Updated:** May 28, 2026
**Project Status:** 🧪 Testing Phase
