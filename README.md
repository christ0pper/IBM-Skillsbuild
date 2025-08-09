# AI-Powered Job Search Assistant using n8n & Telegram

## 📌 Overview
This project is an **AI-powered job search assistant** built using **n8n workflow automation** and **Telegram Bot API**, designed to make job discovery faster, simpler, and more accessible — especially for users in **rural and underserved areas**.  
The bot accepts **voice or text job queries**, scrapes **real-time job listings from WorkIndia**, filters them according to user preferences, and delivers curated results directly in Telegram.  

By integrating **OpenAI Whisper** for speech-to-text, **NLP for query processing**, and **Google Calendar** for scheduling, the system offers an **end-to-end, automated job application experience**.

---

## 🚀 Features
- **Voice & Text Input** – Users can search for jobs by typing or speaking in their preferred language.
- **Real-Time Job Scraping** – Fetches up-to-date listings from WorkIndia.
- **Smart Filtering** – Filters jobs by location, role, work type, and experience.
- **Formatted Telegram Output** – Presents results in clean, numbered Markdown format.
- **One-Click Scheduling** – Schedule interviews directly into Google Calendar.
- **Multi-Language Support** – Accessible for non-English speakers.
- **Low-Tech Accessibility** – Works within the familiar Telegram environment.

---

## 🛠️ Tech Stack
- **[n8n](https://n8n.io/)** – Workflow automation platform.
- **Telegram Bot API** – User interaction and messaging.
- **OpenAI Whisper API** – Speech-to-text transcription.
- **OpenAI GPT Models** – NLP for understanding and formatting.
- **HTTP Request / Web Scraping** – Fetching job listings from WorkIndia.
- **Google Calendar API** – Interview scheduling.
- **Cloud Hosting** – Oracle Cloud / Render for deployment.

---

## 📂 Project Workflow

### 1. **Data Collection**
- Collect real-time job listings from WorkIndia based on user query (role, location, keywords).

### 2. **Preprocessing**
- Classify listings by type (full-time, part-time, remote, internships).
- Remove incomplete or duplicate postings.
- Sanitize data for scams.

### 3. **Feature Selection**
- Job type, location, work mode, user language, and metadata.

### 4. **Feature Engineering**
- Normalize queries, extract keywords using NLP, and create filtering rules.

### 5. **Workflow Automation in n8n**
- **Telegram Trigger → Voice/Text Detection → (If Voice) Transcribe → NLP Processing → Scraping → Filtering → Formatting → Send to Telegram → Schedule in Calendar**

---

## 📊 Sustainable Development Goals (SDGs) Covered
- **SDG 8 – Decent Work and Economic Growth** – Increases access to employment opportunities.
- **SDG 10 – Reduced Inequalities** – Bridges digital and language barriers.
- **SDG 4 – Quality Education (Indirect)** – Recommends skill-building opportunities.

---

## 🖥️ Installation & Setup

### 1. **Clone the Repository**
```bash
git clone https://github.com/yourusername/job-search-ai-assistant.git
cd job-search-ai-assistant
