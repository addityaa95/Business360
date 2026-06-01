# 📊 Business 360 — AtliQ Hardware | Power BI Dashboard

<p align="center">
  <img src="https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black"/>
  <img src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white"/>
  <img src="https://img.shields.io/badge/DAX-512BD4?style=for-the-badge&logo=microsoftpowerbi&logoColor=white"/>
  <img src="https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white"/>
  <img src="https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge"/>
</p>

<p align="center">
  <b>An end-to-end Power BI dashboard covering Finance, Sales, Marketing, Supply Chain & Executive views for AtliQ Hardware — built as part of the Codebasics Power BI Course.</b>
</p>

---

## 📌 Table of Contents
- [About the Project](#-about-the-project)
- [Company Background](#-company-background)
- [Problem Statement](#-problem-statement)
- [Dashboard Views](#-dashboard-views)
- [Key Metrics & Insights](#-key-metrics--insights)
- [Data Model](#-data-model)
- [DAX Measures Used](#-dax-measures-used)
- [Tools & Technologies](#-tools--technologies)
- [Project Learnings](#-project-learnings)
- [Live Dashboard](#-live-dashboard)
- [Connect with Me](#-connect-with-me)

---

## 📖 About the Project

**Business 360** is a comprehensive, multi-view Power BI dashboard built for **AtliQ Hardware Ltd** — designed to replace siloed Excel reports with a single, interactive analytics platform accessible to all business departments.

The dashboard enables stakeholders across Finance, Sales, Marketing, Supply Chain, and Executive teams to monitor KPIs, compare performance against benchmarks, and make faster, data-driven decisions.

> 📅 Data Last Updated: 14 Dec 2025
> 🗄️ Data Source Start: 01 Dec 2021
> 💰 All values in Million USD ($M)

---

## 🏢 Company Background

**AtliQ Hardware** is a leading computer hardware manufacturer in India with a strong domestic presence and a rapidly expanding global footprint. They sell products across:

- **Segments:** Notebook, Accessories, Peripherals, Desktop, Storage, Networking
- **Channels:** Retailer (68.76%), Direct (20.42%), Distributor (10.82%)
- **Regions:** APAC, NA, EU, LATAM
- **Fiscal Year:** September – August

---

## ❗ Problem Statement

AtliQ Hardware's management was relying on scattered Excel reports across departments — making it impossible to get a **unified, real-time view** of business performance.

Key challenges:
- No single source of truth for Finance, Sales & Supply Chain data
- Inability to compare performance against benchmarks (BM) and last year (LY)
- No visibility into forecast accuracy or supply chain risk by customer/segment
- Executive team lacked a consolidated top-level view for strategic decisions

**Business 360 was built to solve all of this — in one dashboard.**

---

## 📊 Dashboard Views

### 🏠 Home Page
A clean navigation landing page with quick access to all 5 views:

| View | Purpose |
|---|---|
| Finance View | P&L Statement — any customer, product, region, time period |
| Sales View | Customer & Product profitability in a growth/margin matrix |
| Marketing View | Regional performance across GM% and NP% metrics |
| Supply Chain View | Forecast accuracy, net error and supply risk profiling |
| Executive View | Top-level KPI consolidation for C-suite decision making |

---

### 💰 Finance View
> *"Get the complete P&L statement for any customer / product / country — over any time period."*

**Key Metrics Displayed:**
| Metric | FY2020 Value | vs Benchmark | Chg % |
|---|---|---|---|
| Gross Sales | $535.95M | $209.06M BM | +156.36% |
| Net Sales (NS) | $267.98M | $111.37M BM | +140.61% |
| Gross Margin (GM%) | 37.10% | 41.20% BM | -9.95% ▼ |
| Net Profit (NP%) | -0.85% | 2.21% BM | -138.68% ▼ |
| Total COGS | $168.56M | $65.49M BM | +157.39% |

**Regional Breakdown:**
| Region | P&L Value ($M) | P&L Chg % |
|---|---|---|
| APAC | 147.98 | +107.48% |
| NA | 62.21 | +182.70% |
| EU | 55.79 | +224.03% |
| LATAM | 2.00 | +141.89% |

📌 *Insight: While Net Sales grew 140% above benchmark, Net Profit is negative (-0.85%) — driven by Operational Expenses of -$101.71M, significantly outpacing the -$43.43M benchmark.*

---

### 🛒 Sales View
> *"Analyse customer and product performance across Net Sales and Gross Margin in a profitability/growth matrix."*

**Top Products by Net Sales:**
| Product | NS ($M) | GM ($M) | GM % |
|---|---|---|---|
| AQ Wi Power Dx2 | 14.37 | 5.46 | 37.96% |
| AQ BZ Gen Y | 12.09 | 4.47 | 36.99% |
| AQ Wi Power Dx1 | 11.84 | 4.38 | 36.97% |
| AQ Lite | 11.55 | 4.21 | 36.47% |
| AQ BZ Compact | 11.40 | 4.16 | 36.47% |

**Total:** NS $267.98M | GM $99.42M | GM% 37.10% | ΔGM% -0.10%

📌 *Insight: Gross Margin % is consistent across products (~37%) but the Δ GM% is uniformly negative — indicating margin compression across the entire product portfolio.*

---

### 📣 Marketing View
> *"Analyse product performance by region across key metrics — Net Sales, Gross Margin and Net Profit — in a profitability/growth matrix."*

**Regional Performance:**
| Region | NS ($M) | GM % | NP ($M) | NP % | ΔNP % |
|---|---|---|---|---|---|
| EU | 55.79 | 37.82% | 0.35 | 0.62% | +1.65 |
| LATAM | 2.00 | 30.96% | 0.00 | -0.08% | -1.01 |
| NA | 62.21 | 39.35% | -1.11 | -1.79% | -0.80 |
| APAC | 147.98 | 35.97% | -1.52 | -1.03% | -1.17 |

📌 *Insight: APAC generates the highest Net Sales ($147.98M) but runs at a -1.03% Net Profit — the largest absolute net loss of all regions. EU is the only region with positive Net Profit (+0.62%).*

---

### 🚚 Supply Chain View
> *"Monitor Forecast Accuracy, Net Error and supply risk profile by product, segment, category and customer."*

**Top-Level KPIs:**
| Metric | FY2020 | vs LY | Change |
|---|---|---|---|
| Forecast Accuracy % | 72.99% | 86.45% | -15.57% ▼ |
| Net Error | 492K | 0.64M | -22.88% ▲ |
| ABS Error % | 6M | 1.55M | +271.06% ▼ |

**Key Metrics by Customer:**
| Customer | FA % | FA % LY | Net Error | Risk |
|---|---|---|---|---|
| AtliQ Exclusive | 56.65% | 76.67% | 330,680 | EI |
| Atliq e Store | 55.24% | 76.51% | -544,329 | OOS |
| Amazon | 48.43% | 78.07% | -917,373 | OOS |

**Key Metrics by Segment:**
| Segment | FA % | Risk |
|---|---|---|
| Storage | 81.01% | EI |
| Notebook | 76.65% | EI |
| Accessories | 71.42% | OOS |
| Networking | 52.50% | OOS |

📌 *Insight: Forecast Accuracy dropped sharply from 86.45% to 72.99% (-15.57%). Amazon and Atliq e Store are flagged OOS (Out of Stock) risk — critical for inventory planning.*

---

### 👔 Executive View
> *"A top-level dashboard consolidating the most important insights from all business dimensions for C-suite executives."*

**Top-Level KPIs:**
| KPI | Value | vs BM/LY |
|---|---|---|
| Net Sales | $267.98M | +140.61% vs BM ▲ |
| Gross Margin % | 37.10% | -9.95% vs BM ▼ |
| Net Profit % | -0.85% | -138.68% vs BM ▼ |
| Forecast Accuracy % | 72.99% | -15.57% vs LY ▼ |

**Top 5 Customers by Revenue Contribution:**
| Customer | RC % | GM % |
|---|---|---|
| Amazon | 18.6% | 37.96% ▼ |
| Atliq e Store | 11.8% | 37.47% ▼ |
| AtliQ Exclusive | 8.6% | 45.79% ▼ |
| Flipkart | 4.1% | 33.54% ▼ |
| Sage | 3.1% | 31.22% ▼ |

**Top 5 Products by Revenue Contribution:**
| Product | RC % | GM % |
|---|---|---|
| AQ Wi Power Dx2 | 5.4% | 37.96% ▼ |
| AQ BZ Gen Y | 4.5% | 36.99% ▼ |
| AQ Lite | 4.3% | 36.47% ▼ |
| AQ BZ Compact | 4.3% | 36.47% ▼ |
| AQ Wi Power Dx1 | 4.4% | 36.97% ▼ |

📌 *Insight: AtliQ Exclusive has the highest GM% among top customers (45.79%) despite lower revenue contribution (8.6%) — suggesting it's the most profitable customer to grow.*

---

## 🗄️ Data Model

The project uses a **Snowflake/Star Schema** connecting dimension and fact tables:

```
Dimension Tables:
├── dim_customer        → customer_code, customer, market, region, channel
├── dim_product         → product_code, product, segment, category, division
├── dim_market          → market, sub_zone, region
└── dim_date            → date, fiscal_year, fiscal_month

Fact Tables:
├── fact_sales_monthly        → customer_code, product_code, sold_qty, fiscal_year
├── fact_forecast_monthly     → customer_code, product_code, forecast_qty
├── fact_gross_price          → product_code, fiscal_year, gross_price
├── fact_manufacturing_cost   → product_code, cost_year, manufacturing_cost
├── fact_pre_invoice_deductions → customer_code, fiscal_year, pre_invoice_discount_pct
└── fact_post_invoice_deductions → customer_code, product_code, discount_pct
```

---

## 📐 DAX Measures Used

```dax
-- Net Sales
Net Sales = SUM(fact_sales_monthly[net_sales_amount])

-- Gross Margin %
GM % = DIVIDE([Gross Margin], [Net Sales], 0)

-- Net Profit %
NP % = DIVIDE([Net Profit], [Net Sales], 0)

-- Forecast Accuracy %
Forecast Accuracy % = 
1 - DIVIDE(
    SUM(fact_forecast_monthly[abs_error]),
    SUM(fact_forecast_monthly[forecast_qty]),
    0
)

-- % Change vs Benchmark
Chg % vs BM = DIVIDE([Net Sales] - [BM Net Sales], [BM Net Sales], 0)
```

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| **Power BI Desktop** | Dashboard design, visuals, interactivity |
| **SQL (MySQL)** | Data extraction and transformation |
| **DAX** | Custom measures, KPIs, calculated columns |
| **Power Query (M)** | Data cleaning and transformation |
| **Excel** | Data validation and source prep |

---

## 🧠 Project Learnings

✔️ Building a **multi-page interactive Power BI dashboard** with consistent theme and navigation

✔️ Writing complex **DAX measures** — DIVIDE, CALCULATE, SUMX, FILTER, VAR

✔️ Designing a proper **data model** with fact and dimension tables in a star/snowflake schema

✔️ Creating **dynamic benchmark comparisons** (vs LY, vs Target, vs BM) using parameter slicers

✔️ Building **supply chain risk profiling** using forecast accuracy and net error logic

✔️ Designing an **Executive View** that consolidates multi-dimensional KPIs for C-suite audiences

✔️ **Stakeholder thinking** — designing each view for a specific business user, not just for aesthetics

---

## 🔗 Live Dashboard

📊 **Power BI Live Report** → [https://tinyurl.com/BuI360]
💼 **Portfolio** → [https://codebasics.io/portfolio/S-K-Adityanarayan]

---

## 🤝 Connect with Me

**S K Adityanarayan**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](your-linkedin-url)

---

<p align="center">
  ⭐ If you found this project helpful, please give it a star — it helps others find it too!
</p>
