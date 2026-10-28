<div align="center">

<img src="./credwise-banner.svg" alt="CredWise — Credit Intelligence Platform" width="100%" />

### Your credit life, brought into focus.

**An early fintech prototype exploring credit tracking, debt visibility, and AI-assisted spending insights.**

[![Live Demo](https://img.shields.io/badge/OPEN-LIVE_DEMO-9B8CFF?style=for-the-badge&logo=googlechrome&logoColor=white)](https://adityakhannaa.github.io/pbl_Credwise/)
[![JavaScript](https://img.shields.io/badge/BUILT_WITH-JAVASCRIPT-F7DF1E?style=for-the-badge&logo=javascript&logoColor=111111)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Firebase](https://img.shields.io/badge/BACKEND-FIREBASE-FFCA28?style=for-the-badge&logo=firebase&logoColor=111111)](https://firebase.google.com/)

*Prototype • Personal/academic project • Not a financial product*

</div>

---

## ◈ The idea

Credit information is easy to lose track of when cards, EMIs, and pay-later balances live in different places. **CredWise** is an early attempt at bringing those numbers into one dashboard, with a few tools that turn raw figures into something easier to understand.

This repository contains an early version of the project—not a production-ready financial platform. It is preserved as a snapshot of the product idea and its first implementation.

## ✦ What you can explore

<table>
<tr>
<td width="50%">

### ◉ Credit overview
View a combined snapshot of credit limits, outstanding balances, utilisation, estimated EMI burden, debt-to-income ratio, and post-EMI cash.

</td>
<td width="50%">

### ▤ Card wallet
Add and manage credit-card details, including limits, outstanding balances, due dates, reward categories, and reward rates.

</td>
</tr>
<tr>
<td width="50%">

### ◷ EMI & BNPL tracking
Record recurring EMI commitments and Buy Now, Pay Later balances to get a clearer picture of monthly obligations.

</td>
<td width="50%">

### ✧ Statement AI
Upload a text-based PDF statement for text extraction and an attempted Gemini-powered summary, with a basic local fallback if the AI request fails.

</td>
</tr>
<tr>
<td width="50%">

### ⌁ Rewards optimiser
Compare the reward-rate information entered for your own cards against estimated shopping, travel, and fuel spending.

</td>
<td width="50%">

### ◌ Charts & insights
Explore charts, due-date reminders, calculated metrics, and generated credit insights based on the data entered.

</td>
</tr>
</table>

> **Important:** Values such as the displayed CIBIL score and AI-generated insights are prototype estimates or generated outputs. They are not official credit-bureau data, verified financial advice, or a guarantee of financial outcomes.

## 🧪 Under the hood

| Part | Technology | Role |
|---|---|---|
| Interface | HTML, CSS | Login screen, dashboard layout, responsive visual components |
| App logic | Vanilla JavaScript | Data processing, form workflows, calculations, navigation |
| Authentication | Firebase Authentication | Account registration and login |
| Data store | Cloud Firestore | Stores card, EMI, and BNPL records associated with a user ID |
| Visualisation | Chart.js | Dashboard charts |
| PDF text extraction | PDF.js | Reads selectable text from uploaded PDF statements in the browser |
| AI requests | Google Gemini API | Attempts to summarise extracted statement text and generate insights |

## 🚀 Run it locally

### 1. Get the code

```bash
git clone https://github.com/adityakhannaa/pbl_Credwise.git
cd pbl_Credwise
```

### 2. Serve the folder

The project is a static HTML/CSS/JavaScript app. Open the folder in VS Code and run `index.html` with a local server extension such as **Live Server**. You can also use another simple static HTTP server.

### 3. Configure your own services

The current prototype expects Firebase Authentication, Cloud Firestore, and a Gemini API key. Before running your own copy:

- Create your own Firebase project and configure Authentication and Firestore.
- Update the Firebase client configuration in `index.html` and `dashboard.js` to use your own project.
- Do **not** put a Gemini API key in browser JavaScript for a public deployment. Route AI requests through a server-side endpoint or another secure backend.
- Review and configure Firestore security rules so each signed-in user can access only their own records.

Without valid service configuration, login, saved records, and AI features may not work.

## 🗂️ Project map

```text
pbl_Credwise/
├── index.html          # Login and account creation screen
├── dashboard.html      # Dashboard sections and user interface
├── style.css           # Dashboard styling and theme
├── dashboard.js        # Firebase setup, calculations, charts, and app workflows
├── credwise-banner.svg # README visual header
└── README.md           # Project overview and setup notes
```

## 🔐 Security & privacy — read before using

This is a **demonstration project only**. Do not enter real bank statements, account credentials, card details, or other sensitive financial information into the public demo.

The source archive currently contains a Gemini API key embedded in client-side JavaScript. A key shipped to a browser must be treated as exposed. **Before making this repository public or continuing to use the key, revoke/rotate it, remove it from the source, and move Gemini calls behind a backend.** If the key was previously committed, removing it from the latest file does not erase it from Git history. Review Firebase security rules and API restrictions as well.

This project has not been presented as a security-audited or production-ready financial service.

## 🧭 Why keep an early version?

CredWise started as a project to explore a practical question: *Could credit cards, instalments, and spending patterns be made easier to understand from one place?*

This first version is a record of that exploration—bringing together interface design, browser-side calculations, Firebase integration, charts, PDF parsing, and an AI API experiment. It is a starting point, not the final word on the idea.

---

<div align="center">

**Made as an experiment. Kept as a milestone.**

[↗ Try the live prototype](https://adityakhannaa.github.io/pbl_Credwise/)

<sub>CredWise · Early prototype by Aditya Khanna</sub>

</div>
