# 🤖 n8n AI Workflow Automation  
Client Pre-Screening & Meeting Intelligence

This repository contains three n8n workflows designed to automate a full client interaction pipeline using AI agents, RAG database, smart email responses, and meeting preparation intelligence.

---

## 🔧 Overview

This project uses n8n to orchestrate:

- **RAG Database Construction** — Convert internal PDFs into a vector store for document-grounded responses
- **Client Budget Filtering** — Classify form submissions based on client budget to determine follow-up strategy
- **Smart Email Responses** — Generate AI replies and auto-embed Cal.com meeting links
- **Webhook Triggered Summary** — Analyze client intent using Tavily Web Search and send pre-meeting briefings

---

## 📂 Included Workflows

| File Name | Description |
|-----------|-------------|
| `Tavily Agent Tool (Web Search).json` | 🔍 A basic **Tavily HTTP request agent** used for external knowledge enrichment |
| `Form_sheet_Schedule_meeting_AI Agent.json` | 📌 Main flow responsible for: <br>– RAG vector store creation <br>– Client budget filtering <br>– AI-generated email responses <br>– Cal.com meeting link embedding |
| `Form_sheet_Schedule_meeting_AI Agent_web search (Using Tavily Agent Tool).json` | 🔁 Handles **Webhook-triggered summary creation** using: <br>– Tavily Web Search <br>– AI summarization before meetings |

---

## 📎 Note on Credentials

These workflows contain only **references** to credentials (e.g., `credential ID`, `name`) but **no actual API keys or secrets**.  
You will need to reassign your own credentials in n8n after import.

---
