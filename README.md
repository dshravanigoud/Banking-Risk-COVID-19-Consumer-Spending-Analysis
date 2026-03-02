# 🏦 Banking Risk & COVID-19 Consumer Spending Analysis

![Domain](https://img.shields.io/badge/Domain-Banking%20Risk%20%7C%20Macro%20Analysis-blue)
![Tool](https://img.shields.io/badge/Tool-Microsoft%20Excel-217346?logo=microsoft-excel&logoColor=white)
![Data](https://img.shields.io/badge/Data-Time%20Series%20%7C%20Daily-orange)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

A three-part financial analysis project spanning **bank liquidity risk modeling**, **COVID-19 consumer spending behavior**, and **Citigroup FY2022 institutional financial analysis**. Built to demonstrate applied skills in risk management, macroeconomic data analysis, and corporate financial modeling.

---

## 📌 Table of Contents
- [Project Overview](#project-overview)
- [Task 3 — COVID-19 & Credit Card Spending](#task-3--covid-19--credit-card-spending)
- [Task 4 — Bank Liquidity & Stress Testing](#task-4--bank-liquidity--stress-testing)
- [YE 2022 — Citigroup Financial Model](#ye-2022--citigroup-financial-model)
- [Key Insights](#key-insights)
- [Skills Demonstrated](#skills-demonstrated)
- [About the Author](#about-the-author)

---

## 📋 Project Overview

| Task | Focus | Period |
|---|---|---|
| **Task 3** | COVID-19 impact on consumer credit card spending | Jan 2020 – Dec 2021 |
| **Task 4** | Bank liquidity stress testing — deposits, loans, surplus | Dec 2022 – Feb 2023 |
| **YE 2022** | Citigroup full-year financial model (11 segments) | FY2021 A vs FY2022 E |

---

## Task 3 — COVID-19 & Credit Card Spending

Analyzes the relationship between daily new COVID-19 case counts and indexed consumer credit card spending across four categories: Total, Delayable, Social, Staples, and Work-related (indexed to February 2020 = 100).

![Credit Sales vs COVID Cases](output2_credit_sales_vs_covid.png)

**Key Findings:**
- Spending collapsed to ~**50–55** (index) during the first lockdown in March–April 2020, then gradually recovered through mid-2020
- **Social and Delayable** spending were the most sensitive to case surges — dropping sharply during the Jan 2021 and Dec 2021 waves
- **Staples** remained relatively stable throughout, reflecting non-discretionary demand
- By late 2021, total spending surpassed 120 (index) — **20%+ above pre-COVID baseline** — despite the Omicron case surge, suggesting consumer desensitization to case counts over time
- The Dec 2021 Omicron wave (nearly **300,000 daily cases**) caused only a minor spending dip, versus the far greater behavioral impact of the first wave at ~5,000 daily cases

---

## Task 4 — Bank Liquidity & Stress Testing

A daily liquidity risk model tracking three deposit products, three loan products, their resulting surplus positions, and stress-tested surplus after applying haircuts — with embedded early warning triggers and management action thresholds.

![Surplus & Stressed Surplus](output1_surplus_stressed_surplus.png)

**Model Structure:**

| Category | Products | Starting Value |
|---|---|---|
| Deposits | Deposit 1, 2, 3 | $100M, $115M, $250M |
| Loans | Loan 1, 2, 3 | $70M, $50M, $10M |
| Surplus | Surplus 1, 2, 3 | Deposits minus Loans |
| Stressed Surplus | Stressed 1, 2, 3 | Haircut-adjusted surplus |

**Early Warning Triggers:**
- Deposit balance drops by more than **3%**
- Loan balance increases by more than **5%**
- Loan increases by **50%** of last year's level
- Surplus drops by more than **half** of last year

**Management Action Threshold:**
- Surplus falls below **$0**

**Key Findings:**
- **Surplus 1** approached zero and turned negative by late February 2023 — breaching the management action threshold
- **Stressed Surplus 1** deteriorated steadily from ~$6M to **–$45M**, signaling a meaningful liquidity risk for that product
- **Surplus 3** remained healthy and trending upward ($240M → $290M), providing a buffer at the portfolio level
- The divergence between Surplus 1 and Surplus 3 highlights concentration risk — overall liquidity looks healthy, but individual product exposure is critical to monitor

---

## YE 2022 — Citigroup Financial Model

A full institutional financial model of Citigroup's FY2022 estimated results vs FY2021 actuals, built across 11 Excel sheets covering the full income statement, balance sheet, and all four business segments.

**Segments Analyzed:**

| Segment | 2022E Revenue | YoY Change |
|---|---|---|
| Institutional Clients Group (ICG) | $9,159M | +2.8% |
| Personal Banking & Wealth Mgmt (PBWM) | $6,096M | +5.4% |
| Legacy Franchises | $2,052M | –6.4% |
| Corporate / Other | $699M | NM |
| **Total** | **$18,006M** | **+5.8%** |

**Headline Metrics:**
- Net Interest Income surged **+23%** ($10.8B → $13.3B) driven by the Fed rate hiking cycle
- Total operating expenses declined **–4%** as restructuring benefits took hold
- Investment banking fees fell **–56%** ($1.67B → $728M) reflecting the 2022 dealmaking drought
- Legacy Franchises revenue declined **–6%** as wind-down progressed

---

## 💡 Key Insights

1. **COVID desensitization is real** — By wave 3 (Omicron, Dec 2021), consumers barely changed spending behavior despite record case counts, unlike the severe contraction in wave 1
2. **Liquidity risk is product-specific** — Portfolio-level surplus can mask individual product vulnerabilities; Surplus 1 breached management action thresholds while Surplus 3 remained strong
3. **Rising rates are a double-edged sword** — Citi's NII jumped 23% in 2022 due to Fed hikes, but investment banking fees collapsed 56% as deal activity froze
4. **Stress testing reveals hidden risk** — The gap between the base surplus and stressed surplus widened significantly for Products 1 and 2 by February 2023, validating the importance of haircut analysis

---

## 🧠 Skills Demonstrated

- **Liquidity Risk Modeling** — Daily surplus tracking, stress testing, early warning triggers, ILAAP-style framework
- **Macroeconomic Data Analysis** — Time-series correlation between COVID cases and consumer spending
- **Institutional Financial Analysis** — Full P&L, balance sheet, and segment analysis for a global bank (Citigroup)
- **Data Visualization** — Dual-axis charts, multi-series line charts, indexed comparisons
- **Excel Best Practices** — Structured data, formula-driven models, print-ready outputs

