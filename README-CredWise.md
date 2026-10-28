
# 💳 CredWise — Your Credit Life, Decoded.

### One dashboard. A clearer picture of your money.

**What if your credit cards, EMIs, outstanding balances, and spending insights could live in one place?**

CredWise is an early fintech prototype built around that idea — bringing scattered credit information together and experimenting with tools that make personal finances easier to understand.

<p align="center">
  <b>Track smarter. Understand better. Spend with clarity.</b>
</p>

🔗 **[Explore the Live Demo](https://adityakhannaa.github.io/pbl_Credwise/)**

> 🧪 **Project status:** Early-stage academic prototype. Built to explore an idea, experiment with technology, and learn by making something real.

---

## ◈ The Problem

Your credit card has one balance. Your EMIs have another schedule. Your pay-later purchases are somewhere else.

Individually, these numbers might make sense. Together, they tell a much more useful story about your financial commitments.

**CredWise explores a simple question: what if you could see more of that story in one place?**

The goal is to turn scattered financial information into a clearer overview of credit utilisation, upcoming obligations, and spending patterns.

## ✦ Inside CredWise

### ◉ 01 — Your Credit Snapshot

Get a combined view of credit limits, outstanding balances, utilisation, estimated EMI burden, debt-to-income ratio, and post-EMI cash.

The idea is simple: understand the bigger picture, not just individual numbers.

### 💳 02 — The Card Wallet

Keep track of your credit cards, entered limits, outstanding balances, due dates, and reward rates.

Instead of juggling disconnected details, explore them from one dashboard.

### ◷ 03 — EMI & BNPL Tracker

Recurring instalments and Buy Now, Pay Later balances can quietly add up.

This module explores how recording those commitments can make monthly obligations easier to see.

### ✧ 04 — Statement AI

Experiment with extracting selectable text from PDF statements and generating summaries using Google's Gemini API.

The prototype also includes a basic local fallback when an AI request fails.

### 🎯 05 — Rewards Optimiser

Compare the reward-rate information entered for your cards against estimated spending across categories such as shopping, travel, and fuel.

The output depends on the accuracy of the information entered — it isn't a guarantee of maximum savings.

### 📊 06 — Charts & Insights

Explore charts, due-date reminders, calculated metrics, and generated insights based on the data entered into the application.

The aim is to make financial information easier to interpret, rather than leaving it as a collection of numbers.

---

## ⚙️ The Technology Behind It

CredWise brings together several technologies to turn a browser-based idea into an interactive prototype.

| Technology | What it does |
|---|---|
| HTML & CSS | Build and style the interface |
| Vanilla JavaScript | Power interactions, calculations, and application logic |
| Firebase Authentication | Handle account registration and login |
| Cloud Firestore | Store application records |
| Chart.js | Visualise dashboard metrics |
| PDF.js | Extract selectable text from PDF statements |
| Google Gemini API | Experiment with AI-generated summaries and insights |

No elaborate framework is required for the core interface. The project uses JavaScript to connect the different parts of the experience.

## 🚀 Run It Yourself

Want to explore the code rather than just the demo?

### 1. Clone the repository

```bash
git clone https://github.com/adityakhannaa/pbl_Credwise.git
cd pbl_Credwise
```

### 2. Open it in VS Code

Open the project folder and run `index.html` using the **Live Server** extension.

### 3. Configure the backend

To use the full application, configure your own Firebase Authentication and Cloud Firestore project.

- Update the Firebase configuration in `index.html` and `dashboard.js`.
- Configure appropriate Firestore security rules.
- Route Gemini API requests through a secure backend instead of exposing an API key in browser JavaScript.

Some features will not work without valid service configuration.

## 🗂️ Project Structure

```text
pbl_Credwise/
├── index.html       # Login and account creation
├── dashboard.html   # Main dashboard interface
├── style.css        # Styling and layout
├── dashboard.js     # Application logic and integrations
└── README.md        # You're reading it right now
```

## 🔐 A Note on Security

CredWise is a learning prototype, not a production-ready financial service.

- Do not enter real bank statements, account credentials, or sensitive financial details into the public demo.
- The original source contains a Gemini API key in client-side JavaScript. Treat that key as exposed, revoke or rotate it, and remove it from the source.
- Move AI requests behind a secure backend before deploying publicly.
- Review Firebase security rules to ensure users cannot access one another's records.
- Remember that removing a key from the latest source does not remove it from Git history.

Displayed credit scores and generated insights are not verified credit-bureau data or professional financial advice. The application has not been security-audited.

---

## 🧠 What This Project Represents

CredWise was an opportunity to explore more than just a dashboard.

It brought together interface design, financial calculations, authentication, database integration, data visualisation, PDF text extraction, and an experiment with generative AI.

Not every idea in an early prototype becomes a finished product. That isn't the point.

**The point is to take an idea, turn it into something tangible, discover what works, and learn what needs to improve.**

This repository preserves one of those early attempts.

## 🛣️ From Idea to Implementation

Every project starts somewhere: a question, a rough concept, or a problem that seems worth solving.

CredWise is an early attempt at answering one such question — how could everyday credit information become easier to understand?

It's not the final version of that vision. It's a milestone in learning how to build it.

---

**Built with curiosity. Improved through experimentation.**

💳 **[Try CredWise](https://adityakhannaa.github.io/pbl_Credwise/)**

*CredWise · An early project by Aditya Khanna*
