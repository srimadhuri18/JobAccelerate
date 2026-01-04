# 🚀 JobAccelerateAi — Autonomous AI Job Search Engine

**Get 3x More Interviews With Automated Job Matching, Auto-Apply, Recruiter Outreach & Analytics**

<p align="center">
  <img src="assets/banner.png" alt="JobAccelerateAi Banner" width="800"/>
</p>

<p align="center">
  <b>The world’s first fully agentic AI system that finds and applies to jobs for you, emails recruiters, and optimizes your CV using real-time analytics.</b>
</p>

<p align="center">
  <a href="#"><img src="https://img.shields.io/badge/Status-Active_Development-blue?style=flat-square" alt="status"></a>
  <a href="#"><img src="https://img.shields.io/badge/License-MIT-green?style=flat-square" alt="license"></a>
  <a href="#"><img src="https://img.shields.io/badge/PRs-Welcome-brightgreen?style=flat-square" alt="prs-welcome"></a>
  <a href="#"><img src="https://img.shields.io/github/issues/yourname/jobaccelerateai?style=flat-square" alt="issues"></a>
</p>

---

## 🚀 Overview

**JobAccelerateAi** is a modern SaaS platform that automates every part of the job search:

- AI agents search and filter jobs daily  
- Automatically apply on your behalf where permitted  
- Find recruiter emails and send personalized outreach  
- Measure what’s working using analytics, A/B testing, and optimization insights  

**Goal:** Make job searching effortless while materially increasing interview conversions.

---

## 🌟 Key Features

### 🔍 Intelligent Job Matching
- Multi-source job aggregation (via partner APIs & permitted feeds)  
- AI semantic matching and relevance scoring  
- Skill & keyword extraction and ranking  
- Daily new job summaries and alerts

### 🤖 Autonomous Auto-Apply Engine
- Auto-apply to relevant jobs daily (where officially supported)  
- Custom rules: title, location, remote, salary ranges, companies  
- Multiple CV variants and A/B testing across applications  
- Detailed application activity logs & retry handling

### ✉️ Recruiter Outreach Automation
- Integrated recruiter email discovery (via paid API integrations)  
- AI-generated personalized outreach using templates & tokens  
- Throttled bulk outreach with deliverability best practices  
- Open, reply, bounce, and reply-quality analytics

### 📄 Resume Intelligence
- Structured resume parsing (skills, experience, education, dates)  
- ATS-compatibility scoring and keyword suggestions  
- Auto-tailor CVs to roles with optional manual review  
- Multi-CV A/B testing with conversion reporting

### 📊 Analytics Dashboard
- End-to-end funnel: Applications → Emails → Opens → Replies → Interviews  
- CV comparison cards showing conversion improvements  
- Email A/B testing results and template recommendations  
- Application heatmaps and trend charts

### 🤖 Bot Integrations
- Telegram / WhatsApp bot for uploads, alerts, and quick actions  
- Bot-driven recruiter message generation and confirmation flows

### 🔐 Security & Compliance
- Encrypted resume storage (at rest & in transit)  
- GDPR-aware consent & data processing flows  
- Verified email sending (DKIM / SPF / DMARC)  
- Audit logs & user data export / deletion

---

## 🏗️ Architecture Overview

                              ┌──────────────────────────────┐
                              │          Frontend            │
                              │     (Next.js + Tailwind)     │
                              └──────────────┬───────────────┘
                                             │
                                             ▼
                 ┌────────────────────────────────────────────────────┐
                 │           Backend API (FastAPI / Node)             │
                 │ Authentication, Matching, Resume Parsing, Billing  │
                 └─────────────────────┬──────────────────────────────┘
                                       │
                                       ▼
             ┌────────────────────────────────────────────────────────┐
             │      Agent Orchestration Layer (Celery/Temporal)       │
             │   Auto-Apply Engine • Email Outreach • Schedulers      │
             └───────────────────────┬────────────────────────────────┘
                                     │
                                     ▼
    ┌────────────────────────────────────────────────────────────────────────┐
    │         Integrations: Job APIs • Email Finder • ATS Connectors         │
    │ Indeed, partner feeds, Email Providers, Hunter/Snov, other providers   │
    └──────────────────────────────┬─────────────────────────────────────────┘
                                   │
                                   ▼
                    ┌──────────────────────────────┐
                    │      Databases & Storage     │
                    │ Postgres                     │
                    └──────────────────────────────┘
## 🧰 Technology Stack

### Frontend
- React
- Next.js 14+ (App Router, Server Actions)
- Tailwind CSS

### Backend
- FastAPI / Node.js

### Database
- PostgreSQL

### AI & Orchestration
- Prompt engineering
- Structured data extraction (JSON mode)
- Agent-based orchestration

## 🤝 Contributing to ECWOC'26

### 🏁 Step-by-Step Setup

1. Fork this repository to your account.

2. Clone your fork:
   ```bash
   git clone https://github.com/DhruvTambekar24/JobAccelerate.git
3. Make your changes to the project.
4. Commit your changes:
   ```bash
    git commit -m "Message"
5.  Push your branch:
      ```bash
      git push origin branch-name
6. Open a Pull Request
👉 Mention ECWOC'26 in the PR description

## 📁 Project Structure
```md

JobAccelerateAi/
├── .next/
│   └── dev/
│       ├── build/
│       ├── cache/
│       ├── logs/
│       ├── server/
│       ├── static/
│       ├── types/
│       ├── build-manifest.json
│       ├── fallback-build-manifest.json
│       ├── package.json
│       ├── prerender-manifest.json
│       ├── routes-manifest.json
│       └── trace
├── app/
│   ├── dashboard/
│   ├── features/
│   ├── login/
│   ├── signup/
│   ├── onboarding/
│   ├── privacy/
│   ├── terms/
│   ├── globals.css
│   ├── layout.tsx
│   └── page.tsx
├── components/
│   ├── MagicBento/
│   ├── magicui/
│   ├── ui/
│   ├── AnimatedBeamDemo.tsx
│   ├── AnimatedBeamMultipleOutputDemo.tsx
│   ├── AnimatedListDemo.tsx
│   ├── FeatureCard1.tsx
│   ├── FluidGlass.tsx
│   ├── GridScan.tsx
│   ├── analytics-chart.tsx
│   ├── auth-card.tsx
│   ├── cards-demo-3.tsx
│   ├── dashboard-activity.tsx
│   ├── dashboard-header.tsx
│   ├── dashboard-sidebar.tsx
│   ├── dashboard-stats.tsx
│   ├── faq-section.tsx
│   ├── feature-card.tsx
│   ├── feature-section.tsx
│   ├── features-deep-dive.tsx
│   ├── features-showcase.tsx
│   ├── footer.tsx
│   ├── hero-section.tsx
│   ├── how-it-works.tsx
│   ├── job-card.tsx
│   ├── nav-header.tsx
│   ├── onboarding-step.tsx
│   ├── pricing-section.tsx
│   ├── testimonials.tsx
│   └── theme-provider.tsx
├── hooks/
├── lib/
├── public/
│   ├── apple-icon.png
│   ├── icon-dark-32x32.png
│   ├── icon-light-32x32.png
│   ├── icon.svg
│   ├── placeholder-logo.png
│   ├── placeholder-logo.svg
│   ├── placeholder-user.jpg
│   ├── placeholder.jpg
│   └── placeholder.svg
├── styles/
├── .gitignore
├── LICENSE.md
├── README.md
├── components.json
├── next-env.d.ts
├── next.config.mjs
├── package.json
├── package-lock.json
├── pnpm-lock.yaml
├── postcss.config.mjs
├── tailwind.config.ts
└── tsconfig.json

```

## 📬 Contact & Support

- **Website:** https://jobaccelerate.ai *(coming soon)*  
- **Support:** support@jobaccelerate.ai  *(coming soon)* 
- **Security:** security@jobaccelerate.ai  *(coming soon)* 

---

## 🙌 Acknowledgements

Thanks to the open-source community, job API providers, email providers, and contributors who inspire and enable this project.

---

**Enjoy building JobAccelerateAi — ship fast, iterate safely, and prioritize user privacy.**
