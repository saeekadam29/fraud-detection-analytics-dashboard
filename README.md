# 🔍 Fraud Detection Analytics Dashboard
> Real-time fraud monitoring across 56,892 transactions using Power BI

## 📊 Live Preview
![Dashboard]( Fraud Detection Analytics Dashboard.png)

## Data set used for dashboard fraud_data_clean.csv
This cleaned dataset was prepared for fraud detection analysis and dashboard development. The preprocessing stage involved handling missing values, scaling important numerical features, transforming transaction data, and preparing the dataset for machine learning and visualization purposes.
Checked and handled missing/null values
Standardized transaction-related numerical features
Scaled Amount and Time features using StandardScaler
Prepared data for fraud analysis and predictive modeling

## 🎯 Key Findings
- Fraud Rate: 0.17%** — 97 fraud cases out of 57K transactions
- Critical & High risk bands** show fraud probability > 0.8
- High-value transactions** are disproportionately flagged as fraud
- 99.83% of transactions are legitimate (minimal false positives)
- Fraud is rare but concentrated — 0.17% rate (97 cases from 57K) shows you can identify a needle in a haystack.
- Mention precision/recall tradeoff awareness.
- Risk band segmentation works — Critical and High bands show dramatically higher fraud probability (>0.7 vs near 0 for Low/None). Shows we can stratify risk meaningfully.
- Temporal patterns exist — Transaction volume and fraud probability vary by hour.
- This suggests time-based fraud rules could be deployed operationally.
- High-value transactions are low volume but high risk The HV vs Normal split by risk band shows targeted fraud attempts on larger transactions.

## Based on the insights generated from the dashboard, we can take the following preventive actions:
-Block or flag high-risk transactions automatically
-Apply stricter verification for critical-risk users
-Monitor high transaction velocity activities
-Set transaction limits for suspicious accounts
-Use multi-factor authentication for risky transactions
-Increase monitoring during high fraud probability hours
-Train machine learning models using detected fraud patterns
-Continuously monitor fraud rate trends for early warning signals

## 🛠️ Tools Used
- Power BI Desktop
- DAX for calculated measures
- Python / SQL for data prep

## 📁 Files
fraud_dashboard.pbix` | Power BI source file |
dataset.csv| Cleaned transaction data |
.png file| Dashboard screenshot |

## 💡 Business Impact
This dashboard enables fraud teams to:
- Prioritize investigations by risk band
- Identify high-risk transaction hours
- Reduce manual review time by focusing on Critical/High bands
