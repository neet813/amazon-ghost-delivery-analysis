# 🚚 Amazon Ghost Delivery Risk Analysis
### Identifying Revenue Leakage in Last-Mile Logistics Using Python & SQL

> *"My order was marked delivered. It never arrived. I'm a data analyst. So I investigated."*

## 📊 Live Dashboard
![Amazon Ghost Delivery Risk Analysis](Amazon_Ghost_Delivery_Risk_Analysis.pdf)

---

## 💼 The Business Case
Ghost deliveries — orders marked as delivered but never received — represent a silent revenue leak for every e-commerce company operating in India.

Based on this analysis of 43,739 real delivery records:

| Business Impact | Value |
|----------------|-------|
| Suspicious deliveries identified | 632 (1.4%) |
| Direct loss per incident (avg ₹1,500 order) | ₹9,48,000 |
| Operational leakage (logistics + support) | ₹2,52,800 |
| Customer churn loss (90% stop ordering) | ₹1,70,64,000 |
| **Total Revenue at Risk** | **₹1,82,64,800** |
| Loss multiplier | For every ₹1 lost, Amazon loses ₹18 in ecosystem value |

---

## 🔍 Technical Architecture
Architected an end-to-end data pipeline to detect, score, and visualise ghost delivery risk across 43,739 Amazon delivery records.
```
Raw Dataset (Kaggle)
       ↓
Python + Pandas — Data cleaning, feature engineering
       ↓
SQL (SQLite) — Risk scoring queries, pattern detection
       ↓
Looker Studio — Executive dashboard with KPI scorecards
```

## 🚨 Key Findings

| Metric | Finding |
|--------|---------|
| Total Deliveries Analysed | 43,739 |
| Suspicious Deliveries | 632 (1.4%) |
| Avg Time — All Deliveries | 124.9 minutes |
| Avg Time — Suspicious | 44.8 minutes |
| Speed Anomaly | 65% faster than normal |
| Primary Risk Area | Metropolitan (78%) |
| Primary Risk Vehicle | Motorcycle (74%) |
| Primary Risk Weather | Windy / Stormy / Sandstorms |

## 💡 Core Insight
Suspicious deliveries are **65% faster** than normal. In metropolitan areas during adverse weather, a sub-45 minute delivery is physically improbable — indicating agents are scanning items as delivered without completing the actual drop-off. This pattern is concentrated in cities (78%), on motorcycles (74%), during windy, stormy, or sandstorm conditions.

## 🛠️ Recommendations
- 📸 **Mandatory photo proof** at point of delivery
- 📱 **Hard OTP verification** for orders above ₹5,000
- 🗺️ **GPS timestamp matching** — agent scan location must be within 50 metres of customer address
- ⭐ **Agent accountability scoring** — flag agents with repeated fast deliveries in adverse conditions
- 🤖 **Automated AI flagging** for sub-45 minute metropolitan deliveries during bad weather

## 📁 Repository Structure
```
amazon-ghost-delivery-analysis/
├── amazon_ghost_delivery_analysis.ipynb  — Full Python pipeline
├── amazon_delivery.csv                   — Raw dataset (43,739 records)
├── ghost_risk_deliveries.csv             — Filtered suspicious deliveries
├── ghost_summary.csv                     — Executive summary metrics
├── Amazon_Ghost_Delivery_Risk_Analysis   — Looker Studio dashboard
└── /research                             — Logic notes and methodology
```

## 🔗 Author
**Navneet Kaur** — Data Analyst | Supply Chain & Operations Analytics  
[Portfolio](https://neet813.github.io/navneet-portfolio) · [LinkedIn](https://linkedin.com/in/navneet-kaur-analyst) · [GitHub](https://github.com/neet813)
