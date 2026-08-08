# AI Lead Generation & Email Outreach Automation with n8n 🚀

An AI-powered lead generation and email outreach automation workflow built with **n8n, Apify, Groq/LLaMA, Google Sheets, and Gmail**.

The workflow automates repetitive lead-generation and outreach preparation tasks while keeping the final email-sending decision under human control.

## ✨ What This Automation Does

The workflow:

1. Collects business leads from Google Maps using Apify
2. Extracts business information such as:

   * Business Name
   * Email
   * Phone
   * Website
   * Address
   * City
   * Country
   * Rating
   * Reviews
   * Category
   * Google Maps URL
3. Cleans and structures the collected data
4. Stores leads automatically in Google Sheets
5. Checks whether a lead has contact information
6. Uses AI to generate personalized cold outreach emails
7. Creates email drafts in Gmail
8. Keeps the final sending decision under human control

## 🏗️ Workflow Architecture

```text
Webhook
   ↓
Respond to Webhook
   ↓
Apify Google Maps Scraper
   ↓
Wait
   ↓
Retrieve Lead Data
   ↓
Data Cleaning
   ↓
Lead Qualification
   ↓
Google Sheets
   ↓
Loop Through Leads
   ↓
AI Email Generation
   ↓
Prepare Email Data
   ↓
Gmail Draft
```

## 🛠️ Tech Stack

* **n8n** — Workflow automation
* **Apify** — Google Maps data extraction
* **Groq / LLaMA** — AI-powered email generation
* **Google Sheets** — Lead storage
* **Gmail** — Email draft creation

## 🤖 AI Email Generation

The AI receives information such as:

* Business Name
* Business Category
* City

It then generates a personalized cold outreach email.

The generated email is limited to under 120 words and returned as an email body without a subject.

## 👤 Human-in-the-Loop

This workflow intentionally creates **Gmail drafts instead of automatically sending emails**.

This allows a human to:

* Review the generated message
* Edit the content if necessary
* Verify the recipient
* Decide whether to send the email

The goal is to automate repetitive work without removing human oversight.

## 📊 Lead Data

The collected lead information is stored in Google Sheets for easy review and management.

Example fields:

| Field         | Description             |
| ------------- | ----------------------- |
| Business Name | Name of the business    |
| Email         | Business email          |
| Phone         | Business phone number   |
| Website       | Business website        |
| Address       | Business address        |
| City          | Business city           |
| Country       | Business country        |
| Rating        | Google Maps rating      |
| Reviews       | Number of reviews       |
| Category      | Business category       |
| Google Maps   | Google Maps listing URL |

## 📸 Workflow Preview

### n8n Workflow

Add your workflow screenshot here.

### Google Sheets

Add your Google Sheets screenshot here.

### Gmail Draft

Add your Gmail draft screenshot here.

## 🚀 Current Status

**MVP Completed ✅**

The current version successfully:

* Scrapes business leads
* Processes lead data
* Saves leads to Google Sheets
* Generates AI-powered outreach emails
* Creates Gmail drafts

## 🔮 Future Improvements

Planned improvements include:

* Dynamic country and city input
* Dynamic business category
* Dynamic number of leads
* Automated lead validation
* Duplicate lead detection
* Better email personalization
* Lead status tracking
* Follow-up automation
* Reply detection
* Chatbot interface for requesting leads
* Human approval workflow

## 🔐 Security

**Important:** API keys, access tokens, OAuth credentials, and other secrets should never be committed to this repository.

Before importing or sharing the workflow, replace sensitive credentials with your own n8n credentials or environment variables.

## 👨‍💻 Built By

**Apu Ghosh**

AI Automation Specialist | Frontend Developer

Interested in building AI-powered workflow automation, AI agents, API integrations, and business process automation.

---

⭐ If you find this project useful, feel free to star the repository.
