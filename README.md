# 17n8n-ai-customer-support-triage

# Project 17: Advanced AI-Powered Customer Support Ticket Triage & Telegram Escalation

## 📋 Business Problem
Support teams face constant bottlenecks dealing with high volumes of angry or frustrated customers. Delayed responses to critical issues (such as locked accounts or billing failures) lead directly to customer churn and brand damage.

## 💡 Proposed Solution
Engineered an **Advanced AI Support Triage Engine** in n8n powered by Google Gemini. The system automatically ingests support tickets, performs deep sentiment and urgency analysis, evaluates conditional routing rules, and instantly dispatches emergency escalation alerts directly to management via Telegram.

## 🛠️ Architecture & Flow
1. **Trigger & Payload Ingestion:** Captures incoming support complaints.
2. **AI Analysis Layer (`Basic LLM Chain` + `Google Gemini`):** Deploys specialized system instructions to parse unstructured text into structured diagnostics (Executive Summary, Sentiment Level, and Urgency).
3. **Conditional Routing (`IF Node`):** Isolates tickets marked with negative sentiment and high frustration.
4. **Automated Escalation (`Telegram Node`):** Dispatches real-time emergency alerts containing AI diagnostics directly to the support team's communication channel.

<img width="1098" height="461" alt="image" src="https://github.com/user-attachments/assets/2ebb977b-b490-4b0e-b612-fa829ecebfd6" />


## 🧰 Tools & Nodes Used
- **Platform:** n8n
- **AI Model:** Google Gemini Chat Model (`models/gemini-3-flash-preview`)
- **n8n Nodes:** Manual Trigger, Edit Fields (Set), Basic LLM Chain, IF Node, Telegram (Send Message).
