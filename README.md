# ruchi-m
Data Models for Marketing

# 🛒 E‑Commerce Customer Churn Prediction



# Customer Churn Prediction (Classification)

## Overview
This project predicts the probability that a customer will churn in the next 30 days.
The output is a churn risk score used to prioritize retention campaigns and reduce marketing waste.

## Business Problem
Retention is cheaper than acquisition. Identifying high-risk customers early enables targeted interventions
(discounts, reminders, personalized offers) with measurable uplift.

## Churn Definition
- `churn_flag = 1`: no purchase in the next 30 days
- `churn_flag = 0`: at least one purchase in the next 30 days

Population: prior buyers with sufficient history (excludes new customers and suppressed/opt-out records).

## Data & Features
### Example feature groups
- **Purchase behavior:** recency, frequency, monetary value
- **Engagement:** open/click rates, days since last open
- **Customer value/profile:** tenure, loyalty tier
- **Promo sensitivity:** discount usage

## Modeling Approach
- Baseline: Logistic Regression (interpretable, probability scores)
- Output: churn probability (0–1)

## Evaluation
- AUC (ranking quality)
- Lift/Deciles (marketing utility)
- Confusion matrix & precision/recall at selected thresholds

## How to Run
1. Install dependencies:
   ```bash
   pip install -r requirements.txt
