# Penlink_project
The Shefa Be-Paa Initiative: orchestrating retail efficiency through advanced data modeling

 --> Retail Analytics: Operational Optimization at Shefa Issachar Supermarket
-- Project Overview
This project delivers an end-to-end analysis of the Yavne branch operations for the "Shefa Issachar" supermarket chain. By leveraging geolocation and transactional data from June to November 2025, the study transforms raw operational data into strategic insights regarding workforce scaling, self-checkout investment, and customer monetization.

-- Tools & Technologies
* Google BigQuery (SQL): Data cleaning, Exploratory Data Analysis (EDA), and complex KPI development.
* Looker: Development of interactive dashboards and data visualization to communicate insights to stakeholders.
* Google Sheets: Statistical modeling and implementation of Linear Regression analysis for trend forecasting.
* Advanced Statistics: Percentile-based normalization (P25/P75) for demand peak detection and customer segmentation.

-- Technical Challenges & Solutions
* Data Quality & Cleaning: Identified that 31.76% of GPS signals were imprecise (>30m). I implemented spatial precision filters to ensure the dwell time analysis reflected actual in-store behavior, excluding parking lot noise.
* Anomaly Detection: Validated actual operational hours by cross-referencing sales logs with customer presence, identifying unexpected closures and extreme demand days.
* Dynamic Segmentation: Developed a 3x3 matrix based on Average Ticket and Visit Frequency (P25/P75), allowing for the identification of a "VIP" segment that drives the majority of total revenue.

-- Key Business Insights
* Demand Concentration: Customer flow and operational pressure are non-uniform, peaking drastically on Thursdays and Fridays.
* Loyalty & App Engagement: The supermarket app shows exceptionally high penetration, linked to 89.6% of total sales, making it the primary channel for marketing and loyalty strategies.
* Checkout Efficiency: Analysis proved that self-checkouts should serve as an operational buffer during peaks and a cost-reduction lever during "dead hours," rather than a one-size-fits-all solution.

-- Repository Structure
* `sql/`: Full script covering data cleaning, business logic, and regression models.
* `visualizations/`: Dashboard exports and charts created in **Looker**.
* `models/`: Spreadsheet containing the **Linear Regression** and statistical calculations performed in Google Sheets.
* `docs/`: Final Technical & Executive Report containing strategic recommendations.
