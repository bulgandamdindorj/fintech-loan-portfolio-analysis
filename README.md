# Moni Fintech App: UX Analysis, Customer Intelligence & Product Contribution

> This internal customer analysis saved approximately CAD $75,000 in external agency costs. During a mandatory end-of-probation review with senior leadership, I raised several product and brand issues I had noticed — which led the CEO to decide on a company-wide rebrand for both Moni and Omnicapital. A marketing agency was brought in and quoted 200M MNT (~CAD $75,000) for the customer research alone. I proposed to do it internally instead, got access to the company data, and delivered the full analysis myself..

---

## Background

**Company:** Moni is a mobile micro-lending app based in Mongolia, operated under Omnicapital NBFI. It targets younger, digital-first borrowers with short-term personal loans.

Three months into my role, during a mandatory end-of-probation review with the President, CEO, HR Head, and Department Heads, I raised three issues that nobody had flagged before:

**1. Brand mismatch between social media and the app**
Moni's Facebook and social media content was minimal, colorful, and youthful — exactly the kind of modern fintech feel the brand was going for. But when customers opened the actual app, the experience was completely different. The interface was dark, heavy, and corporate — closer in feel to Omnicapital, the traditional NBFI parent company. A customer who discovered Moni through social media would open the app and feel like they were in an entirely different product. The brand was promising one experience and delivering another.
<img width="1710" height="962" alt="Screenshot 2026-06-24 at 10 50 48 AM" src="https://github.com/user-attachments/assets/9af622b1-e525-42d6-b9c7-ff8da7c06af3" /> <img width="1710" height="962" alt="Screenshot 2026-06-24 at 10 50 57 AM" src="https://github.com/user-attachments/assets/226482c8-4f7b-4fc4-8408-e74fab59c3ef" />



**2. Broken features pushing customers out of the app**
Several in-app buttons were routing users to an inactive Facebook page instead of keeping them inside the app. Customers who tapped on certain services were being sent outside Moni entirely — to a page that no longer worked.

**3. The loyalty feature was effectively invisible**
Moni had a loyalty rewards program that customers were actively being advertised. But the feature itself was buried inside a rotating banner on the home screen. When the banner rotated away, the button disappeared. I only found it myself after asking my manager to point it out — and even then I hadn't realized it was a clickable button. It looked like a decorative banner, not a feature.

The CEO hadn't noticed any of this. He decided on the spot to move forward with rebranding both Moni and Omnicapital.

A week later, a marketing agency came in to pitch the rebrand. They proposed doing customer research, defining the target audience, and building the brand direction for both companies. Their price: **200M MNT (approximately CAD $75,000 — a significant amount in the Mongolian market, roughly equivalent to the annual salaries of several senior professionals).**

I told the CEO I could do the customer research myself if he gave me access to the company data. He did. This repository covers the Moni side of that work.

---

## Part 1 — UX Issues & App Redesign

### What I flagged
The three issues above were documented in my presentation with direct comparisons between Moni's social media mood (minimal, colorful, youthful) and the app interface mood (dark, heavy, corporate). The gap between the two was the core problem.

### What happened next
The CEO called an urgent meeting with the product development team, designers, and developers. The product team took ownership of the interface redesign. My role in this process was:

- Providing written feedback on layout and information structure
- Writing and refining all in-app copy — how features were named, described, and communicated to users
- Reviewing prototypes and giving feedback to designers and developers from a marketing and user clarity perspective

The result: Moni's app was redesigned to be clean, minimal, and consistent with its social media identity. Features are now clearly visible and accessible. The loyalty program is a permanent, clearly labeled button — not a rotating banner.

### Before vs After
*Screenshots showing old dark interface vs current clean interface are included in the `/screenshots` folder.*

---

## Part 2 — Moni Customer Data Analysis

### The Data
- **380,000 Moni app customer records**
- Variables: age, gender, marital status, monthly income, property ownership, vehicle ownership

### Key Findings

**The registration drop-off problem**

| Metric | Number |
|---|---|
| App downloads (Play Store + App Store) | 800,000 |
| Registered users | 208,000 |
| Active users | 80,000 |
| Downloaded but never registered | 433,000 |

The biggest opportunity was not acquiring brand new users — it was converting the **433,000 people who had already downloaded the app but never completed registration.** These were warm prospects who had shown interest but dropped off somewhere in the sign-up process.

Additionally, 128,000 registered users were inactive — they signed up but stopped using the app. This was a second recovery opportunity.

**Who the active customers are**

- **37%** of registered users are aged 21–30
- **40%** are aged 31–40
- Women slightly outnumber men in the registered user base

In raw numbers: approximately 78,000 users aged 21–30 and 84,000 aged 31–40 were registered at the time of analysis.

**The market size context**

Mongolia's population aged 20–40: approximately **522,000 men and 519,000 women** — just over 1 million people nationally.

With 208,000 registered users out of a target market of 1,041,000, Moni had reached roughly **20% of its core demographic** — leaving significant room to grow, particularly through reactivating the 433,000 who downloaded but never signed up.

**What drives loan demand — the segmentation framework**

Based on the customer data and supported by academic research on buying behaviour by age and income, I built a segmentation matrix to estimate which customer profiles were most likely to need — and actively use — a consumer loan.

Key insight from the framework:
- Younger customers (20–30) with lower income had high loan demand regardless of marital status
- Middle-income customers aged 31–40 showed the highest overall loan activity
- Single-income households and single parents showed unexpectedly high loan frequency despite tighter budgets
- Higher-income customers (4M+ MNT/month) across all age groups showed lower loan demand — they had less need for short-term micro-lending

**The interest rate sensitivity campaign**

Based on the finding that 433,000 people downloaded Moni but never completed registration, I proposed a targeted SMS campaign to this group offering a temporary interest rate reduction — from the standard 3.6–6% monthly rate down to 1.9–2.5% for one month.

The business question this addressed: does the cost of offering a discounted rate for one month generate enough new long-term customers to justify the short-term revenue loss? The data suggested yes — the prospect pool was large, the interest rate was a known barrier, and a one-time incentive had low downside risk compared to losing those users permanently.

---

## What I Would Do Differently With Current Tools

This analysis was done in Excel. With the tools I have now:

- **SQL** — to query the 380,000 customer records more efficiently and join demographic data with behavioural data
- **Power BI** — to build an interactive dashboard filtering by age, income, location, and activity status
- **Python (pandas)** — to calculate statistical correlation between customer attributes and loan uptake rates

---

## Tools Used

| Tool | Purpose |
|---|---|
| Microsoft Excel | Data cleaning, pivot tables, segmentation analysis, charts |
| PowerPoint | Executive presentation to CEO and senior leadership |

---

## Screenshots

> All customer identifiers have been removed. Screenshots show aggregated data only.

- `/screenshots/moni-old-app.png` — old dark interface
- `/screenshots/moni-new-app.png` — redesigned clean interface
- `/screenshots/brand-mismatch.png` — social media vs app mood comparison slide
- `/screenshots/registration-funnel.png` — 800k downloads → 208k registered → 80k active
- `/screenshots/age-gender-breakdown.png` — registered customer demographics
- `/screenshots/segmentation-matrix.png` — loan demand by age and income
- `/screenshots/sms-campaign.png` — interest rate reduction campaign proposal

---

## Related Project

**Omnicapital Loan Portfolio Analysis** — the traditional lending side of this same engagement, covering 3,900 loan records, non-performing loan analysis by geography and demographics, and the Omnicapital website redesign.

→ [View Omnicapital project](../omnicapital-loan-portfolio-analysis)

---

## About

**Bulgan Damdindorj** | Vancouver, BC
MBA — University Canada West (2026)
[LinkedIn](https://linkedin.com/in/yourprofile) · [GitHub](https://github.com/bulgandamdindorj)
