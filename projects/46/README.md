# CRM Sales Dashboard Project Report

## Project Overview
This project involved building an interactive dashboard for Maven Tech's Sales Managers to track their team's quarterly performance using CRM sales data. The dashboard provides insights into sales trends, win-loss analysis, and individual sales agent performance.

## Objectives and Achievements

### Objective 1: Data Preparation
- **Datasets Used:**
  - `sales_pipeline.csv`: Sales opportunities data.
  - `sales_teams.csv`: Sales agents with their managers and regional offices.
  - `accounts.csv`: Client account details.
  - `products.csv`: Product details and pricing.
  - `data_dictionary.csv`: Dataset field descriptions.
- **Key Actions:**
  - Merged sales pipeline data with sales teams to include manager and regional office information.
  - Converted date columns to datetime format for analysis.
  - Created a 'quarter' column based on the close date to facilitate quarterly performance tracking.

### Objective 2: Data Exploration with Pivot Tables
- **Opportunities Won by Quarter:** Identified quarterly sales trends by counting won opportunities.
- **Win vs. Loss Percentage by Quarter:** Analyzed the proportion of won and lost deals across quarters.
- **Sales Agent Performance by Quarter:** Ranked sales agents based on deals won per quarter, sorted by the most recent quarter.

### Objective 3: Dynamic Dashboard
- **Visualizations Created:**
  - **Bar Chart:** Opportunities won by quarter.
  - **Stacked Bar Chart:** Percentage of deals won vs. lost by quarter.
  - **Horizontal Bar Chart:** Sales agent performance in the most recent quarter.
- **Interactive Features:**
  - Data was structured to support filtering by manager and regional office.
  - Visuals were designed to clearly highlight key sales metrics.

## Key Insights
- **Quarterly Performance:** Visuals highlighted growth trends in sales opportunities over the quarters.
- **Win/Loss Ratios:** Showed fluctuating success rates, helping identify periods needing strategic adjustments.
- **Top Performer:** **Kary Hendrixson** from **Summer Sewald's** team won the most deals in **Q4 2017**.

## Recommendations
- **Focus on High Performers:** Leverage successful sales agents' strategies to improve team performance.
- **Address Declining Quarters:** Investigate and address causes of performance dips in specific quarters.
- **Expand Dashboard Functionality:** Introduce more interactivity, such as real-time filters and trend analysis, to further enhance decision-making.

## Conclusion
The CRM Sales Dashboard offers a comprehensive view of the sales pipeline, equipping Sales Managers with the tools to monitor, evaluate, and optimize their teams' performance. This data-driven approach is expected to foster strategic growth and efficiency in sales operations.


