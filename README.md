# 🎙️ Kural (குரல்)
### ✨ IT help that listens, sees and understands

**Kural** means *voice* in Tamil 🗣️. It is a multilingual, emotion-aware IT helpdesk that lets employees describe IT problems naturally, by 🎤 voice, ⌨️ text or 🖼️ screenshot, in their own language. Kural classifies each issue, sets a fair priority, suggests a fix, and routes anything unresolved to the right IT team.

> 🏆 Built for **IEEE Day 2026 · Vibe Coding**
> 📌 Problem Statement 02: *AI-Powered IT Ticket Classification & Resolution System*

🔗 **Live demo:** https://9050poojaap-cmyk.github.io/kural/

---

## 😩 The problem

- 📝 Employees must fill long IT forms, usually in English and full of technical terms.
- ❓ Most tickets are vague ("it's not working"), so IT spends time asking follow-up questions.
- 🐢 Every ticket is read and sorted by hand, and urgent issues wait in the same queue as minor ones.
- 📚 When many people hit the same issue, IT receives dozens of duplicate tickets.

## 💡 Our solution

| Feature | Description |
|---|---|
| 🌐 **Multilingual input** | Type or speak in English, Tamil or Hindi, including mixed Tanglish and Hinglish |
| 🖼️ **Screenshot support** | Paste (Ctrl+V) or upload a screenshot of the error |
| 🧠 **Automatic classification** | Detects category, assigns priority (P1–P4) and routes to the correct team |
| 💛 **Emotion awareness** | Detects calm, confused, anxious, frustrated or angry users and adapts the tone of the reply |
| ⚖️ **Fair prioritisation** | Emotion changes only the tone; priority is based on business impact and urgency |
| ✅ **Guided resolution** | Step-by-step fix instructions; one click marks the issue resolved or raises a ticket |
| 👥 **Role-based views** | Separate views for Employee, IT Agent and IT Manager |
| 📡 **Outage radar** | Groups 3+ similar tickets within 60 minutes into one incident and notifies all affected users at once |

## ⚙️ How it works

```
🎤 Input (voice / text / screenshot)
        ↓
🧠 Understanding (language · category · urgency · emotion)
        ↓
🎯 Output (fix steps → self-resolved  |  ticket → right IT team  |  outage alert → manager)
```

## 🛠️ Tech stack

| Layer | Technology |
|---|---|
| 💻 Frontend | HTML5, CSS3, JavaScript (ES6+), single-page application |
| 🎨 UI | CSS Grid, Flexbox, design tokens, responsive layout |
| 🎤 Voice | Web Speech API (en-IN, ta-IN, hi-IN) |
| 🖼️ Images | Clipboard API, FileReader API, HTML5 Canvas (client-side compression) |
| 🧠 Intelligence | LLM with structured JSON output (AI mode) + rule-based NLP engine (offline mode) |
| 🔤 NLP techniques | Keyword intent classification, regex urgency extraction, Unicode-based language detection, lexicon-based sentiment analysis |
| 💾 Storage | Browser localStorage (demo) · real-time document database (AI mode) |
| 🚀 Hosting | GitHub Pages (HTTPS) |

⚡ **Why no framework?** A zero-dependency build loads instantly, needs no installation, and keeps working without an internet connection.

## 🚀 Getting started

No installation needed. 🎉

1. 🌍 Open the live demo link, **or** download `index.html` and open it in **Google Chrome**.
2. 👤 Choose a demo user on the login screen.

> 🎙️ Voice input requires Google Chrome and microphone permission.

## 👥 Demo users

| Role | Users |
|---|---|
| 🧑‍💼 Employees | Priya Sharma, Karthik Raman, Meena Iyer |
| 🛠️ IT Agents | Arjun (Network), Divya (Access & Identity), Rahul (Devices & Software) |
| 📊 IT Manager | Sanjay (all teams, Outage Radar) |

## 🎬 Demo walkthrough

1. 🧑‍💼 **Employee:** Log in as **Priya** and type *"VPN connect aagala!! client call in 10 mins"*. Kural replies in Tanglish, flags the user as 😤 frustrated, detects the ⏰ deadline and sets priority 🔴 P1. Click **Still broken · raise ticket**.
2. 🛠️ **IT Agent:** Switch to **Arjun**. The ticket appears at the top of the queue with the user's original words, an English summary and a mood badge. Reply and resolve it ✅.
3. 📊 **IT Manager:** Switch to **Sanjay** and click **Simulate VPN outage**. Eight reports are grouped into one incident on the 📡 radar. Click **Notify all affected users** 📢.

## 📁 Project structure

```
kural/
├── index.html   # complete application (HTML, CSS, JavaScript)
└── README.md
```

## 🗺️ Roadmap

- 🔑 One-click automated fixes (password reset, VPN profile refresh)
- 📚 Knowledge base that learns from every resolved ticket
- 💬 Microsoft Teams and WhatsApp integration
- 🏗️ Production backend: React, Node.js, PostgreSQL, single sign-on
- 📈 Accuracy reporting on classification

## 🌟 Impact

- 🧑‍💼 **Employees:** help in their own language, faster resolution, no forms
- 🛠️ **IT teams:** complete tickets, urgent issues first, fewer duplicates
- 🏢 **Organisations:** less downtime and clear insight into recurring problems

---

💙 *In the spirit of IEEE's mission of advancing technology for the benefit of humanity: every person, heard in their own voice.* 🎙️
