# Customer-Value-Account-Health-Analytics
> An end-to-end customer analytics initiative featuring RFM segmentation, Customer Lifetime Value (CLV) estimation, churn prediction modeling, and an interactive Power BI dashboard.

###  How It Was Done

#### **A. Segmentation & Lifetime Value Modeling**
* **RFM Score Allocation:** Processed transactional logs to compute **Recency, Frequency, and Monetary (RFM)** scores for every unique customer account.
* **Cohort Clustering:** Segmented customer bases into actionable business tiers (*Champions*, *Loyal Accounts*, *At-Risk*, *Hibernating*).

#### **B. Composite Account Health Index**
* **Weighted Metric Score:** Engineered an **Account Health Scorecard** $(0 - 100)$ by weighting continuous activity metrics:
  * Product usage frequency and active login days
  * Support ticket volume and escalation frequency
  * Payment history and subscription renewal frequency

#### **C. Predictive Churn Modeling & BI**
* **Classification Pipeline:** Trained supervised models (**Logistic Regression**, **Random Forest**) in Python using historical behavioral features to predict binary churn risk.
* **Interactive Dashboard:** Built a dynamic **Power BI Dashboard** to monitor account health distributions, churn risk tiers, and customer lifetime value across active cohorts.

###  Key Results & Insights
* **Baseline Churn Rate:** Analysis and Power BI evaluation revealed an overall dataset **churn rate of 39.8%**, flagging **12.1% of active accounts in the high-risk category**.
* **Early Warning Indicators:** Support ticket escalations and steep drops in usage intensity served as leading indicators, surfacing **30–60 days prior to customer cancellation**.
* **Targeted Interventions:** Allowed customer success teams to focus retention campaigns specifically on high-monetary, low-health accounts.
