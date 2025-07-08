# AI-Scoring-System

# ✨ AI-Powered Writing Evaluation System

This project is a no-code/low-code solution built with [n8n](https://n8n.io) that automates **student essay evaluation** using **AI** and delivers feedback via **email**. It is tailored for use in schools and universities to help educators quickly assess student writing with grammar, creativity, and relevance insights.

---

## 📌 Features

- 📥 Accepts student essay input via a form
- 🤖 Uses AI (like OpenAI or Gemini) to evaluate grammar, structure, creativity, and topic relevance
- 🧠 Extracts structured feedback and scores from AI output
- 💌 Sends a personalized evaluation email to each student
- ⚡ Fully automated and customizable with n8n

---

## 🔧 Tech Stack

- 🔄 [n8n](https://n8n.io) – workflow automation
- 🧠 OpenAI / Gemini – natural language evaluation
- 📬 Gmail API – sends personalized feedback
- 📝 JSON-based form inputs and outputs

---

## 🚀 How It Works

1. **Student submits a form** with their name, grade, topic, and essay
2. The workflow:
   - Sends the essay to an AI agent for evaluation
   - Extracts structured sections like grammar feedback, creativity score, and relevance
   - Formats the output into a clean, readable email
   - Sends the result back to the student via Gmail

---

## 🧩 Workflow Nodes Overview

```plaintext
[Start (Webhook)]
   ↓
[AI Evaluation (OpenAI)]
   ↓
[Information Extractor / Function Node]
   ↓
[Set Node (Formats Email Body)]
   ↓
[Gmail Node (Send Email)]
