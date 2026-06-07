# 🚗 EV Market Comparison — Tesla vs Rivian vs Ford (2021–2024)

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)

## 📌 Project Overview

An end-to-end Data Analytics project comparing **3 major EV companies** — Tesla, Rivian, and Ford — across **144 monthly records** spanning **4 years (2021–2024)**. This project analyzes EV deliveries, revenue, net income, market share, and operating margins to tell the complete story of the electric vehicle industry's most critical growth period.

**Business Problem:** Who is winning the EV race? Compare Tesla's dominance, Ford's transition from legacy auto to EV, and Rivian's struggle to achieve profitability — and identify what drives success in the EV market.

---

## 🔗 Live Dashboard

👉 [View Interactive Dashboard on Power BI](https://app.powerbi.com/groups/me/reports/33e56cf5-61c8-4844-93ed-0dec806c5cb0/1534786030e03295c261?experience=power-bi)

---

## 📊 Dashboard Preview — 4 Pages

### Page 1 — Overall Comparison
- KPI Cards: Total Deliveries, Total Revenue, Max Market Share, Max Models Available
- Deliveries by Company and Year
- Revenue by Company and Year
- Total Market Share by Year
- Average Revenue Per Vehicle
- EV Models Available by Year
- Net Income by Company and Year

### Page 2 — Tesla Analysis
- Tesla-themed dashboard with vehicle background
- KPI Cards: Total Deliveries, Revenue, Net Income, Operating Margin, Market Share
- Deliveries trend, Revenue by Quarter, Operating Margin, Net Income Waterfall
- Avg Revenue Per Vehicle Gauge, EV Models Growth

### Page 3 — Rivian Analysis
- Rivian-themed dashboard with truck background
- Same metrics as Tesla page — highlights Rivian's growth story
- Operating Margin showing real negative values
- Net Income showing consistent losses reducing over time

### Page 4 — Ford Analysis
- Ford-themed dashboard with vehicle background
- Same metrics — highlights Ford's EV transition journey
- Comparison of EV vs overall revenue contribution

---

## 🗂️ Project Structure

```
EV-Market-Comparison/
│
├── data/
│   ├── EV_Companies_Monthly_2021_2024.csv    # Master dataset (144 rows)
│   └── queries/
│       ├── query_yearly_deliveries.csv
│       ├── query_yearly_revenue.csv
│       ├── query_market_share.csv
│       ├── query_net_income.csv
│       └── query_rev_per_vehicle.csv
│
├── dashboard/
│   └── EV_Comparison_Dashboard.pbix          # Power BI dashboard file
│
└── README.md
```

---

## 🔄 Project Workflow

```
Synthetic Dataset (based on real earnings reports)
      ↓
SQL Analysis (SQLite)
      ↓
Power BI Dashboard (4 Pages)
      ↓
Company-wise & Comparative Insights
```

---

## 📦 About the Dataset

This dataset was **synthetically generated** based on **real publicly reported numbers** from official earnings reports and investor relations pages of Tesla, Ford, and Rivian.

| Property | Detail |
|---|---|
| Total Rows | 144 monthly records |
| Companies | Tesla (TSLA), Ford (F), Rivian (RIVN) |
| Time Period | January 2021 – December 2024 |
| Granularity | Monthly |
| Source | Based on official earnings reports |

### Columns

| Column | Description |
|---|---|
| `Company` | Tesla / Ford / Rivian |
| `Year` | 2021–2024 |
| `Month` | 1–12 |
| `Quarter` | Q1–Q4 |
| `Deliveries` | Monthly EV deliveries |
| `Revenue_USD_M` | Monthly revenue in USD millions |
| `Net_Income_USD_M` | Monthly net income in USD millions |
| `Operating_Margin_%` | Operating margin percentage |
| `EV_Models_Available` | Number of EV models offered |
| `Revenue_Per_Vehicle` | Revenue generated per vehicle delivered |
| `Market_Share_%` | Company's share of total 3-company deliveries |

---

## 🗃️ SQL Analysis

**Tool:** SQLite (via Python)

### Queries Written

| Query | Business Question |
|---|---|
| Yearly Deliveries | How many EVs did each company deliver per year? |
| Yearly Revenue | How much revenue did each company generate per year? |
| Market Share | What % of the market does each company own? |
| Net Income | Which companies are profitable vs losing money? |
| Revenue Per Vehicle | How much does each company earn per car sold? |

---

## 📈 Key Insights

### 1. Tesla Dominates the EV Market
- Tesla holds **~85-90% market share** consistently
- Delivered **6M+ vehicles** from 2021–2024
- Only company with **consistent profitability**

### 2. Rivian — High Potential, High Losses
- Started with **zero deliveries** in early 2021
- Grew to **~14K monthly deliveries** by 2024
- Still **losing money every quarter** — total losses ~$21B
- But losses are **slowly decreasing** — positive sign

### 3. Ford — Legacy Giant Transitioning Slowly
- EV deliveries growing from **27K (2021)** to **91K (2024)**
- Revenue includes **all vehicles** not just EVs
- Operating margin **much lower** than Tesla
- Struggling with EV profitability

### 4. Revenue Per Vehicle
- **Tesla:** ~$50K per vehicle — premium positioning
- **Rivian:** ~$65K per vehicle — ultra-premium trucks
- **Ford:** ~$500K+ (misleading — includes all vehicle revenue)

### 5. EV Models Race
- Tesla: 3 models (2021) → 5 models (2024)
- Ford: 1 model (2021) → 4 models (2024)
- Rivian: 0 models (2021) → 3 models (2024)

---

## 💡 Business Recommendations

| Company | Finding | Recommendation |
|---|---|---|
| **Tesla** | Operating margin declining from 19% to 6% | Focus on cost reduction & new revenue streams |
| **Rivian** | Losses decreasing but still burning cash | Achieve production scale of 100K/year to break even |
| **Ford** | EV division losing money | Separate EV reporting for clearer investor visibility |

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Python (Pandas, NumPy) | Dataset generation & SQL analysis |
| SQLite | SQL querying & aggregation |
| Power BI Desktop | 4-page interactive dashboard |
| Power BI Service | Publishing & sharing |
| Google Colab | Development environment |

---

## 📊 Dashboard Design

Each company page has a **unique theme:**

| Page | Background | Color Theme |
|---|---|---|
| Overall Comparison | Abstract tech | Purple/Dark |
| Tesla Analysis | Tesla vehicle | Red |
| Rivian Analysis | Rivian truck | Gold/Yellow |
| Ford Analysis | Ford vehicle | Blue |

---

## 🌐 Data Sources & References

- Tesla Investor Relations: [ir.tesla.com](https://ir.tesla.com)
- Rivian Investor Relations: [rivian.com/investors](https://rivian.com/investors)
- Ford Investor Relations: [shareholder.ford.com](https://shareholder.ford.com)

---

## 👤 Author

**Adarsh Anay Salukhe**
- GitHub: [@AdarshSalukhe](https://github.com/AdarshSalukhe)
- LinkedIn: [Connect with me](www.linkedin.com/in/adarsh-salukhe-a0a44221a)

---

## ⭐ If you found this project useful, please give it a star!
