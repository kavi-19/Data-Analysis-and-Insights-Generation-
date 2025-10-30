Data Analysis & Insights (Task 2)
📋 Overview

This project focuses on performing data analysis and insights generation using Python. The dataset was analyzed to understand its structure, clean inconsistencies, extract meaningful features, and derive actionable insights for stakeholders.

🔍 1. Column-Wise Analysis

Each column was examined for its data type, unique values, distribution, and business significance.

Column Name	Data Type	Description	Key Observations
Order_ID	String	Unique identifier for each transaction	No duplicates; acts as primary key
Customer_Name	Object	Name of the customer	Few inconsistencies in capitalization
Region	Categorical	Represents geographic zone	Uneven distribution — majority from “West” region
Product_Category	Categorical	Product grouping	Balanced distribution across 4 categories
Total_Sales	Numeric	Total sale value per order	Right-skewed; few outliers in high-value sales
🧹 2. Data Cleaning Summary

Missing values: Imputed with mode (categorical) and median (numerical).

Inconsistencies: Fixed typos and standardized text cases in categorical columns.

Outliers: Detected via IQR; high-value outliers retained for business relevance.

Data types: Converted string-formatted numerics to float/int as needed.

✅ Final dataset contains 100% valid rows ready for analysis.

⭐ 3. Top 5 Critical Columns

Based on business impact and interpretability, the following columns were identified as most insightful:

Region – Helps identify location-based performance trends.

Product_Category – Crucial for understanding product-level demand.

Total_Sales – Key financial metric for profitability tracking.

Order_Date – Enables time-series insights and seasonality detection.

Customer_Segment – Differentiates purchase behavior across segments.

📊 Visual Insights

Bar Chart: Sales distribution by product category

Pie Chart: Regional sales contribution

Line Plot: Monthly sales trend over time

(Visualizations generated using Matplotlib and Seaborn.)

🏷️ 4. Feature & Tag Generation

Using NLP-based keyword extraction from the text fields (e.g., Comments, Failure_Reason, Product_Description), custom tags were generated to capture recurring patterns such as:

Example Free Text	Generated Tags
“Motor failure due to overheating”	["motor_failure", "overheating"]
“Delay in shipment from warehouse”	["delay", "shipment_issue"]
“Replaced defective sensor”	["sensor_issue", "replacement"]

These tags helped summarize recurring issues and categorize root causes for better decision-making.

📈 5. Summary & Key Insights

The dataset revealed that sales concentration was regionally uneven, with strong performance in specific areas.

High-value orders contributed significantly to overall revenue — potential focus for premium customer targeting.

Text tag analysis highlighted recurring failure patterns, indicating areas for process improvement.

Addressing identified data gaps and inconsistent entries improved overall dataset reliability.

💡 Actionable Recommendations

Focus marketing on underperforming regions to balance sales.

Investigate frequent tag patterns (e.g., “shipment_delay”) to enhance logistics efficiency.

Leverage high-spending customer segments for loyalty programs.

🧰 Tech Stack

Language: Python

Libraries: pandas, numpy, matplotlib, seaborn, nltk

Deliverables:

Cleaned & tagged dataset (cleaned_data.csv)

Python analysis script (task2_analysis.py)

Visualization outputs (/plots/)

Summary report (task2_report.pdf)
