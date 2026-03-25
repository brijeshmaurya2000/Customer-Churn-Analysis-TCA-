# Customer-Churn-Analysis-TCA-

## Project Overview

This project analyzes a Telecom Customer Churn dataset containing 7,043 customers and 21 features. The goal is to identify key factors driving customer churn and provide actionable business insights to improve retention.

### The dataset includes:

#### Customer demographics
#### Account information
#### Subscribed services
#### Churn status

After data cleaning, no missing values or duplicate records were found.

## Data Cleaning

The following preprocessing steps were performed:

Replaced blank values in TotalCharges with 0 (customers with zero tenure had no charges)
Converted TotalCharges from object to float
Re-encoded SeniorCitizen from 0/1 to Yes/No
Verified:
##### . 0 null values
 ##### .0 duplicate customerID records
##### .Key Performance Indicators (KPIs)
### Metric	Value
##### .Total Customers	7,043
##### .Churn Rate	26.5% (~1,869 customers lost)
##### .Avg Monthly Charges	$64.76
##### .Avg Tenure	32.4 months

## Insight:
Approximately 1 in 4 customers churn, indicating a significant retention challenge.

### Churn Breakdown
Segment	Retained	Churned	Insight

###### .Month-to-Month	2,220	1,655	Highest churn risk

###### .One-Year Contract	1,307	166	Better retention

###### .Two-Year Contract	1,647	48	Strongest retention

###### .Non-Senior	4,508	1,393	Lower churn

###### .Senior Citizens	666	476	~42% churn rate

###### .Electronic Check	1,294	1,071	Highest risk

###### .Other Payments	2,880	798	Lower churn

## Key Insights
### 1. Contract Type — Strongest Predictor
Month-to-month customers churn the most
Long-term contracts significantly improve retention

#### Conclusion: Contract duration is the biggest churn driver

### 2. Tenure — Early Churn Risk
Most churn occurs within the first 1–2 months
Long-term customers are highly loyal

### Conclusion: Poor onboarding leads to early churn

### 3. Senior Citizens — High-Risk Segment
~42% churn rate vs ~24% for others

### Conclusion: Seniors need targeted retention strategies

## 4. Payment Method — Electronic Check Risk
Highest churn observed in electronic check users

### Conclusion: Payment friction may impact retention

## 5. Add-on Services — Retention Booster
Customers without services like:
Online Security
Tech Support
Backup
Device Protection
→ show very high churn (~55–58%)
Customers with services → low churn (~15–22%)

### Conclusion: Bundling increases customer stickiness

## 6. Gender — Not Significant
No major difference in churn between male and female

### Conclusion: Gender is not a useful predictor

# Business Recommendations

Based on the analysis:

## Promote long-term contracts
Offer discounts, rewards, or value-added benefits
## Improve onboarding experience
Focus on first 1–2 months with proactive engagement
## Encourage service bundling
Increase perceived value and reduce churn
## Optimize payment methods
Promote auto-pay options with incentives
## Target senior customers
### Provide:
Simplified plans
Dedicated support
Easy billing systems
## Tools & Technologies Used
Python (Pandas, NumPy)
Data Visualization (Matplotlib / Seaborn / Tableau)
Excel / SQL (optional if used)
 

This analysis highlights that contract type, tenure, payment method, and service usage are the most critical drivers of churn. By focusing on early customer experience and value-added services, businesses can significantly reduce churn and improve customer lifetime value.
