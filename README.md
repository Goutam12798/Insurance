🏥 Insurance Analytics & Customer Sentiment Dashboard

📌 Problem Statement

This dashboard helps the insurance company understand its policy performance, customer behavior, claim trends, and customer sentiment to improve operational efficiency and customer satisfaction.

The objective of this project is to:

Analyze policy distribution across different customer segments
Track total premium collected and claim amounts
Identify high-claim risk categories
Monitor policy status (Active, Expired, Cancelled)
Understand customer demographics (Age, Gender, Region, Policy Type)
Perform Sentiment Analysis on customer feedback to measure satisfaction levels
Provide actionable insights to reduce churn and improve customer experience
Since insurance companies operate on risk management and customer retention, this dashboard enables stakeholders to:
Detect high-risk segments
Monitor claim-to-premium ratio
Improve customer retention strategies
Identify dissatisfaction through feedback sentiment
Make data-driven business decisions

🛠️ Steps Followed
Step 1: Data Import into MS SQL Server

Imported raw dataset (InsuranceData.csv) into Microsoft SQL Server
Created structured database tables
Defined appropriate data types (INT, VARCHAR, DATE, FLOAT)

Step 2: Loading Data into Power BI

Connected Power BI to MS SQL Server
Imported cleaned tables into Power BI Desktop
Established relationships between fact and dimension tables

Step 3: Table View & Data Profiling

Opened Power Query Editor
Enabled:
Column Distribution
Column Quality
Column Profile

Checked:
Null values
Outliers
Data consistency
Performed transformations:
Removed null/irrelevant values
Renamed columns
Changed data types

Step 4: Adding Slicers & Text Elements

Added slicers for:
Policy Type
Customer Gender
Region
Policy Status

Step 5: Adding Card Visuals (KPIs)

Created key measures using DAX:
Total Customers
Total Premium Amount
Total Claim Amount
Claim Ratio (%)
Active Policies
Displayed using Card visuals.

Step 6: Multi-Row Card & Ribbon Chart

Multi-row card to show:
Premium by Policy Type
Claims by Region
Ribbon chart to show:
Changing rank of policy types over time

Step 7: Bar & Line Charts

Bar chart:
Claims by Policy Type
Premium by Region

Line chart:
Monthly Premium Trend
Claim Trend Over Time

Step 8: Donut Chart & Matrix Visual

Donut chart:
Policy Status Distribution
Customer Gender Distribution

Matrix visual:
Premium & Claim comparison by Policy Type and Region
Drill-down enabled

Step 9: Publishing Report

Published report to Power BI Service

Step 10: Scheduled Refresh

Configured Gateway
Enabled daily refresh
Ensured real-time business reporting

Step 11: Drill-Through Filter

Implemented drill-through from:
Policy Summary → Individual Policy Details
Region → Customer Level Analysis

Step 12: Row Level Security (RLS)

Created roles in Power BI Desktop
Applied region-based filtering
Tested RLS in Power BI Service
Ensured restricted access for different managers

Step 13: Dashboard Creation

Created:
Executive Summary Dashboard
Claims Analysis Dashboard
Customer Segmentation Dashboard

💬 Sentiment Analysis (Customer Feedback)
Step 14: Sentiment Analysis in Power Query

Performed basic sentiment analysis using Power Query:
Created conditional column:
If feedback contains positive words → “Positive”
Negative keywords → “Negative”
Otherwise → “Neutral”
Categorized customer reviews into:
Positive
Neutral
Negative

Step 15: Sentiment Visualizations

Added:

Donut chart for Sentiment Distribution
Bar chart for Sentiment by Policy Type
Line chart for Sentiment Trend
KPI Card for % Positive Feedback

📊 Insights
1️⃣ Customer & Policy Insights

Majority of customers belong to the mid-age working group
Most policies are concentrated in specific regions
High number of policies are Active
Certain policy types generate maximum premium revenue

2️⃣ Claim Analysis Insights

Claim ratio highlights high-risk categories
Some regions show higher claim frequency
Certain policy types have high claim-to-premium ratio
Monthly trend shows seasonal spike in claims

3️⃣ Revenue Insights

Total Premium collected is significantly higher than claim payout
Business sustainability depends on maintaining healthy claim ratio
Returning customers contribute major revenue share

4️⃣ Sentiment Analysis Insights

Majority of feedback is Positive
Negative feedback is concentrated in:
Claim processing time
Customer support delays
Positive feedback highlights:
Easy policy purchase
Smooth renewal process

🎯 Business Recommendations

Improve claim settlement speed
Focus on high-risk policy monitoring
Introduce retention programs for dissatisfied customers
Improve customer service for negative sentiment regions
Monitor sentiment trend monthly
