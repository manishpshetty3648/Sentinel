# Sentinel
Silent loss detector/ intelligence for small business

<div align="center">

# 🛡️ Sentinel

### Silent-Loss Intelligence for Small Business

*Stop losing money you can't see.*

[![AWS](https://img.shields.io/badge/Deployed%20on-AWS-FF9900?logo=amazonaws&logoColor=white)](https://aws.amazon.com/)
[![Amplify](https://img.shields.io/badge/Hosted%20on-AWS%20Amplify-FF9900?logo=awsamplify&logoColor=white)](https://aws.amazon.com/amplify/)
[![Bedrock](https://img.shields.io/badge/Powered%20by-Amazon%20Bedrock-232F3E?logo=amazonaws&logoColor=white)](https://aws.amazon.com/bedrock/)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

**Built for the Bharat Builds Tour · Ship It Track**

</div>

---

## 📖 Table of Contents

- [The Problem](#-the-problem)
- [The Solution](#-the-solution)
- [What Makes Sentinel Different](#-what-makes-sentinel-different)
- [Features](#-features)
- [Architecture](#-architecture)
- [AWS Services Used](#-aws-services-used)
- [Tech Stack](#-tech-stack)
- [Getting Started](#-getting-started)
- [Deployment](#-deployment)
- [Project Structure](#-project-structure)
- [How the Detection Engine Works](#-how-the-detection-engine-works)
- [Roadmap](#-roadmap)
- [Team](#-team)
- [License](#-license)

---

## 🎯 The Problem

Small businesses don't lose money in one big mistake. **They lose small amounts, repeatedly, through problems they never notice.**

A typical shop owner sees this at the end of the month:


This is something a standard analytics tool physically cannot do, because the signal spans four separate datasets.

### 2. **"Explain Why" on Every Finding**
Every flagged finding has an audit trail. Click any card and you see:
- The **headline reason** it was flagged
- The **exact evidence** (stock levels, dates, PO history, return reasons)
- The **possible financial impact**
- A **suggested investigation** step
- The **source records** used

Sentinel never asserts causation as fact. It flags **statistically abnormal patterns worth human investigation.**

### 3. **Detects Unmet Demand — Invisible in Sales Data**
When a product goes out of stock, no transaction happens. No return. No complaint. The demand simply *disappears* from every report.

Sentinel estimates unmet demand by comparing the demand rate on in-stock days against sell-through on stockout days, surfacing a loss that literally does not appear anywhere else.

### 4. **A Real Conversational AI Agent**
The chatbot isn't a scripted if-else tree. It's powered by **Amazon Bedrock** with **Strands Agents**, reasoning over your actual business data to answer questions like:

> *"What should I investigate first, and why?"*

---

## 🚀 Features

<table>
<tr>
<td width="50%" valign="top">

### 🔍 Detection Engine
- **8 detectors** covering the full operational surface
- Dead/slow-moving inventory detection
- Stockout & missed-sales estimation
- Supplier delivery degradation tracking
- Return rate concentration analysis
- Supplier price-creep detection
- Overdue receivables & chronic late-payer detection
- Root-cause chain discovery
- Unmet-demand signal estimation

</td>
<td width="50%" valign="top">

### 🎨 Experience
- **Liquid Glass UI** — Apple-inspired refraction, blur, and depth
- **Dual themes** — dark & light, both with glass aesthetics
- **Professional motion** — spring-based micro-interactions, staggered entrances, animated counters
- **Fully responsive** — desktop, tablet, mobile
- **Explain Why drawer** — full evidence trail on every finding

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🛠️ Data Management
- Add / edit / delete products, sales, purchase orders, returns, and invoices
- **Undo support** — every deletion is reversible
- **Live re-scan** — detection re-runs instantly on any data change
- Full CRUD on all operational records

</td>
<td width="50%" valign="top">

### 🤖 AI Assistant
- Natural-language chat over your business data
- Powered by Amazon Bedrock (Claude)
- Session memory — remembers your name, last topic
- Handles small talk, math, opinions, and questions
- Built-in content safety filters

</td>
</tr>
</table>

---

## 🏗️ Architecture


---

## ☁️ AWS Services Used

| Service | Purpose |
|---|---|
| **AWS Amplify Hosting** | Git-based CI/CD + global CDN hosting for the frontend |
| **Amazon CloudFront** | Edge delivery of static assets (managed by Amplify) |
| **Amazon S3** | Static asset storage (managed by Amplify) |
| **Amazon API Gateway** | HTTP API routing to Lambda functions |
| **AWS Lambda** | Serverless compute — API logic + Bedrock agent |
| **Amazon DynamoDB** | NoSQL storage for all operational data |
| **Amazon Bedrock** | LLM reasoning via Claude 3.5 Sonnet |
| **Strands Agents SDK** | Agent framework for tool-using AI |
| **AWS Certificate Manager** | Free SSL/TLS certificates (via Amplify) |
| **Amazon CloudWatch** | Logs and monitoring for Lambda functions |
| **AWS IAM** | Access control and least-privilege policies |

---

## 🛠️ Tech Stack

<div align="center">

| Layer | Technology |
|:---:|:---:|
| **Frontend** | HTML5 · CSS3 · Vanilla JavaScript (ES2020+) |
| **Design** | Custom Liquid Glass system · Apple-inspired motion |
| **Typography** | Inter · JetBrains Mono |
| **Backend** | AWS Lambda (Node.js 20.x · Python 3.12) |
| **Database** | Amazon DynamoDB |
| **AI** | Amazon Bedrock · Strands Agents SDK · Claude 3.5 Sonnet |
| **Hosting** | AWS Amplify Hosting |
| **CI/CD** | Git-based auto-deploy via Amplify |

</div>

---

## 🚦 Getting Started

### Prerequisites

- A modern browser (Chrome, Safari, Firefox, Edge)
- No build tools required — Sentinel runs as a single HTML file

### Local Development

```bash
# Clone the repository
git clone https://github.com/your-username/sentinel.git
cd sentinel

# Open in your browser — that's it
open index.html          # macOS
xdg-open index.html      # Linux
start index.html         # Windows
