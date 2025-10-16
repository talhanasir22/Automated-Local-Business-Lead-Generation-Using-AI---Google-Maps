# 🛰️ AI-Powered Lead Generation Agent

**Google Maps + Perplexity Sonar API + GPT + Google Sheets**

This AI-powered agent automates **local lead generation** by combining Google Maps data, **Perplexity Sonar API**, and **OpenAI GPT** to collect, enrich, and organize business details directly into **Google Sheets** — turning raw search data into outreach-ready leads in minutes.

---

## 🧠 What the Agent Does

### 🔍 Search Google Maps

Fetches local business information such as:

* Name, address, phone, website
* Operating hours and reviews
  (Uses the **Serper-powered Google Maps API**)

### 🧾 Save Data to Google Sheets

Automatically stores and structures results in a connected **Google Sheet** for easy tracking and automation.

### 📩 Enrich Leads via Perplexity Sonar API

Retrieves detailed company insights — including **emails**, **background data**, and more — to enhance your lead profiles.

### 🧹 Clean & Format Results

Leverages **OpenAI GPT** to refine, validate, and format all data into consistent, outreach-ready records.

### ⚡ Trigger-Based Automation

Executes automatically when:

* A **new row** is added to Google Sheets, or
* A **chat message** triggers a search.
  Perfect for dynamic, hands-free lead workflows.

---

## 🛠️ Tools & APIs Used

| Tool / API                          | Function                         |
| ----------------------------------- | -------------------------------- |
| 🔹 **Google Maps API (via Serper)** | Finds local businesses           |
| 🔹 **Perplexity Sonar API**         | Enriches company data            |
| 🔹 **Google Sheets**                | Stores and updates leads         |
| 🔹 **OpenAI GPT-4**                 | Parses and structures messy data |
| 🔹 **n8n**                          | Handles workflow automation      |

---

## 🧱 Workflow Overview

### 💬 Chat Agent Trigger

```
User Message → AI Agent → Decide Action
    ├─ OpenAI Chat Model (intent recognition)
    ├─ Store to Google Sheet (maps data)
    └─ Map Searcher (via Serper API)
```

### 📍 Google Maps Data Extraction

```
Trigger: Chat or User Input
↓
Call Serper (Google Maps API)
↓
Extract business data (name, address, phone, website, etc.)
↓
Append to Google Sheet
```

### 🔍 Lead Enrichment via Perplexity

```
Trigger: New Row Added in Google Sheet
↓
Filter valid businesses
↓
Loop over each business
↓
Call Perplexity API (with name/domain)
↓
Parse JSON response
↓
Update Sheet with email & company insights
```

### 📄 Output & Save

```
Trigger → Parse Data → Append Row → Confirm Response
```

---

## 🧪 Getting Started

1. **Sign up or log into n8n**
2. **Import this workflow**
3. **Set up credentials:**

   * Serper API (Google Maps)
   * Perplexity API Key
   * OpenAI API Key
   * Google Sheets OAuth
4. **Create or link a Google Sheet** with proper column headers
5. **Run & Test:** Add a business manually or trigger via chat

---

## 📊 Ideal Use Cases

* Local SEO agencies targeting nearby businesses
* B2B SaaS teams for lead scraping & enrichment
* Automated outreach data pipelines
* Google Maps-based prospecting workflows

---

## 🔒 Notes & Best Practices

* Respect **Google Maps** and **LinkedIn** Terms of Service
* Apply **rate limits** to prevent API overload
* Validate collected emails with tools like **NeverBounce** or **ZeroBounce** before outreach
