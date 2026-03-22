# 🚚 Amazon Ghost Delivery Risk Analysis

> *"My order was marked delivered. It never arrived. I'm a data analyst. So I investigated."*

## 📊 Live Dashboard

![Amazon Ghost Delivery Risk Analysis](Amazon_Ghost_Delivery_Risk_Analysis.pdf)

## Overview
This project analyses 43,739 real Amazon delivery records to identify ghost delivery patterns — deliveries marked as completed but potentially never received by customers.

**Tools:** Python · Pandas · SQL · Looker Studio  
**Dataset:** Amazon Delivery Dataset — Kaggle (43,739 deliveries)

## Key Findings

| Metric | Value |
|--------|-------|
| Total Deliveries | 43,739 |
| Suspicious Deliveries | 632 |
| Suspicious Rate | 1.4% |
| Avg Delivery Time — All | 124.9 mins |
| Avg Delivery Time — Suspicious | 44.8 mins |
| Primary Risk Area | Metropolitan (78%) |
| Primary Risk Vehicle | Motorcycle (74%) |
| Primary Risk Weather | Windy / Stormy / Sandstorms |

## The Core Insight
Suspicious deliveries are 65% faster than normal. Agents mark deliveries as complete in bad weather — particularly in metropolitan areas on motorcycles — without completing the actual delivery.

## Recommendations
- Mandatory photo proof at delivery
- OTP verification before marking delivered
- GPS location matching at time of delivery scan
- Agent performance scoring based on delivery patterns
- AI flagging for suspiciously fast deliveries in adverse weather

## Files
- `amazon_ghost_delivery_analysis.ipynb` — Full analysis
- `amazon_delivery.csv` — Raw dataset
- `ghost_risk_deliveries.csv` — Suspicious deliveries
- `ghost_summary.csv` — Summary metrics

## Author
**Navneet Kaur** — Data Analyst  
[Portfolio](https://neet813.github.io/navneet-portfolio) · [LinkedIn](https://linkedin.com/in/navneet-kaur-analyst)
