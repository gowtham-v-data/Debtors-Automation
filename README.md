# 📞 Debt Collection Automation System  
### (n8n + VAPI Voice AI + Pinecone + Google Gemini)

An advanced automation system that manages **AI voice calling**, **debtor classification**, **RAG-based product support**, **Google Sheets updates**, **PDF ingestion**, and **automated HTML reporting** — powered by **n8n**, **VAPI.ai**, **Google Gemini**, and **Pinecone Vector DB**.

---

## 📘 About the Project

This project automates the entire **debt collection workflow**, including:

🔊 Automated outbound voice calls using VAPI Voice AI  
💬 Personalized call prompts for each debtor  
📝 Transcript, call summary & recording extraction  
🧠 Call intent detection (Paid, Callback, Wrong Number, etc.)  
📊 Automatic Google Sheet updates  
📄 Product PDF ingestion for RAG  
🧩 Pinecone vector embeddings  
🤖 Gemini RAG chatbot for product Q&A  
📧 Daily HTML manager report via Gmail  

---

## 🖼️ Workflow Screenshots

<img width="1247" height="310" src="https://github.com/user-attachments/assets/2ff7628c-cf12-4cf5-a8b6-e3572d6fb6ef" />

<img width="953" height="481" src="https://github.com/user-attachments/assets/4a10d37f-6dea-4306-a0fd-f187f6403586" />

---

## 🛠️ Built With

- ⚙️ n8n Automation Engine  
- 📞 VAPI.ai Voice Calling  
- 📑 Google Sheets / Drive / Gmail APIs  
- 🧠 Google Gemini LLM  
- 🗃️ Pinecone Vector Store  
- 🐘 PostgreSQL (Memory)  
- 🟨 JavaScript (Custom Logic)  

---

## 🚀 Getting Started

### 🧰 Prerequisites

You will need:

- n8n (Cloud or Self-Hosted)  
- Google Cloud OAuth credentials  
- Gmail OAuth2  
- VAPI Assistant ID + Phone Number ID  
- Pinecone Index  
- Gemini API Key  
- Postgres (optional)  

---

## 📥 Installation

### **1️⃣ Clone the Repository**

git clone https://github.com/gowtham-v-data/Debtors-Automation

### **2️⃣ Import the Workflow into n8n**

Go to: n8n Editor → Workflows → Import from File

Then upload: Debtors.json


This will load the **entire voice automation + RAG chatbot + reporting system** into your n8n instance.

---

## 3️⃣ Configure Required Credentials in n8n

You must configure the following credentials for the workflow to function correctly:

- **Google Sheets OAuth2**
- **Google Drive OAuth2**
- **Gmail OAuth2**
- **VAPI API Key**
- **Gemini API Key**
- **Pinecone API Key**
- **PostgreSQL connection** (optional, if using memory persistence)

---

# 📘 Usage

## 📞 1. Automated Calling Flow (VAPI Voice AI)

- Reads pending debtors from **Google Sheets**
- Generates a **personalized voice call script**
- Initiates a **VAPI.ai voice call**
- AI agent can answer customer questions such as:
  - “**When did I buy this?**”
  - “**What product did I buy?**”
  - “**Why are you calling me?**”
  - “**Call me later.**”

- Retrieves:
  - **Call transcript**
  - **Call summary**
  - **Analysis**

- Classifies the call as:
  - ✔️ **PAID**
  - 🔄 **CALL_LATER**
  - 🚫 **REFUSED**
  - ❌ **WRONG_NUMBER**
  - 🔃 **NEED_EXTENSION**
  - 💸 **ALREADY_PAID**
  - ❓ **UNCLEAR**

- Automatically updates **Google Sheets**
- Schedules the **next callback** if required

---

## 💬 2. RAG Product Chatbot (Gemini + Pinecone)

- Downloads product **PDFs** from Google Drive
- Extracts and chunks all text
- Generates **embeddings using Google Gemini**
- Stores vector embeddings in **Pinecone**
- AI agent uses **vector search (RAG)** to answer customer questions
- Ensures **0 hallucinations** by grounding answers in the PDF

---

## 📧 3. Manager Report (HTML Email)

The workflow automatically generates a daily HTML report showing:

- 📈 **Total calls**
- 📋 **Outcome summary**
- ⏳ **Next callback schedule**
- 📝 **Customer notes**
- ✉️ Report is emailed using **Gmail API**

---

👉 **Demo Video (Google Drive Link):**  
https://drive.google.com/drive/u/1/folders/1L_sKVN4YjKPKmWqGBhpebW9CwED52FRV


# 🗺️ Roadmap

- [x] Automated Voice Calling  
- [x] RAG Integration  
- [x] HTML Manager Report  
- [ ] Dashboard UI  
- [ ] Multi-language voice support  
- [ ] WhatsApp reminders  

---

# 🙏 Acknowledgments

- **n8n Documentation**
- **VAPI.ai API Docs**
- **Pinecone Documentation**
- **Google Gemini Documentation**





