Perfect — you’ve already done the hardest part (workflow + video). Now I’ll give you a **ready-to-use professional README.md + GitHub structure** exactly as companies expect.

---

# ✅ 1. README.md (Copy–Paste Ready)

```markdown
# 🧠 AI Health Coach Chatbot (Telegram + n8n + A/B Testing)

## 🎥 Intro Video
Loom Video: https://www.loom.com/share/278f51b20e094e07998a2e5ab680c776

---

## 🚀 Project Overview

This project is an AI-powered Health Coach chatbot built using Telegram, n8n, and Supabase. It includes:

- A/B Testing using Statsig
- AI-driven meal tracking
- Real-time database integration
- Conversational onboarding experience

The goal is to improve user engagement and retention through structured onboarding and intelligent health tracking.

---
## 📸 Demo

![App Screenshot](assets/screenshot.png)
<img width="1612" height="694" alt="image" src="https://github.com/user-attachments/assets/b10cd52b-a066-4bd5-92bc-1274bca6eda6" />
<img width="1014" height="1013" alt="image" src="https://github.com/user-attachments/assets/be17414e-2e09-4e57-af79-fdbf90f01b1a" />


## 🧩 Features

### ✅ Primary Task: A/B Testing Chatbot
- Users are automatically assigned to:
  - **Control Group** → Simple welcome message
  - **Test Group** → 3-step onboarding flow
- Implemented using **Statsig**
- Event logging for:
  - Group assignment
  - Onboarding steps
  - User interactions

---

### 🥗 Secondary Task: Health Chatbot

Users can:

- 🍽️ Add meals
- 📋 View meals
- ✏️ Edit meals
- 🗑️ Delete meals

All data is stored in **Supabase** and accessed dynamically using AI tools.

---

## 🏗️ Architecture Overview

```

Telegram Bot → n8n Workflow → AI Agent → Supabase DB
↘ Statsig (A/B Testing)

````

### Workflow Highlights:
- Command routing (`/start`, `/addmeal`, etc.)
- AI agent handles dynamic conversations
- Supabase stores users, meals, events
- Statsig assigns experiment groups

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|--------|
| n8n | Workflow automation |
| Telegram Bot API | User interaction |
| Supabase | Database (users, meals, events) |
| Statsig | A/B testing |
| OpenRouter / LLM | AI responses |
| JavaScript | Logic inside n8n |

---

## ⚙️ Setup Instructions

### 1. Clone Repository
```bash
git clone https://github.com/your-username/ai-health-chatbot.git
cd ai-health-chatbot
````

### 2. Setup n8n

* Import workflow JSON
* Configure credentials:

  * Telegram API
  * Supabase
  * Statsig
  * OpenRouter

### 3. Environment Variables

```
SUPABASE_URL=
SUPABASE_KEY=
STATSIG_SERVER_KEY=
TELEGRAM_BOT_TOKEN=
OPENROUTER_API_KEY=
```

### 4. Run n8n

```bash
n8n start
```

---

## 📊 Evaluation Plan

### 🎯 Primary Metric

* Onboarding Completion Rate (Leading Indicator of Retention)

### 🛡️ Guardrail Metrics

* Bot block rate
* Drop-off during onboarding

### 📈 Secondary Metrics

* Day 1 retention
* Day 7 retention
* Meals logged per user

### 🧠 Decision Framework

* If onboarding completion ↑ → rollout to all users
* If drop-off ↑ → optimize onboarding steps

---

## ⚖️ Assumptions & Trade-offs

* Used Supabase for simplicity and speed
* AI handles flexible input instead of strict validation
* Focused more on backend automation than UI

---

## ⏱️ Time Breakdown

| Task            | Time  |
| --------------- | ----- |
| Primary Task    | X hrs |
| Secondary Task  | X hrs |
| Bonus Tasks     | X hrs |
| Video Recording | X hrs |

---

## 📌 Future Improvements

* Mobile App (Expo)
* Real-time sync
* Analytics dashboard
* Better personalization using AI

---

## 💡 Key Highlights

* Fully AI-integrated chatbot
* Scalable architecture
* Clean modular workflow
* Real-world product thinking

---

## 🙌 Author

Manpreet Singh
Full Stack Developer | AI Automation Engineer

GitHub: [https://github.com/manpreet1singh2](https://github.com/manpreet1singh2)
LinkedIn: [https://www.linkedin.com/in/manpreet-singh-84750627a/](https://www.linkedin.com/in/manpreet-singh-84750627a/)

---

```

---

# ✅ 2. GitHub Repository Structure

Create repo like this:

```

ai-health-chatbot/
│
├── README.md
├── workflow/
│   └── n8n-workflow.json   <-- export your workflow
│
├── docs/
│   ├── architecture.png (optional)
│   └── notes.md
│
├── .env.example
└── assets/
└── screenshots (optional)

Workflow → Export → JSON → Save in repo

````

---

# ✅  GitHub Steps (Very Simple)

```bash
git init
git add .
git commit -m "Initial commit - AI Health Chatbot"
git branch -M main
git remote add origin https://github.com/your-username/ai-health-chatbot.git
git push -u origin main
````
