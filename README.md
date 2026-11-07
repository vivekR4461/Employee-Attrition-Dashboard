# Employee-Attrition-Dashboard

Project Overview
This project delivers an interactive HR analytics solution that isolates the root causes of voluntary employee churn and forecasts retention risks across departments. By converting raw HR data into predictive risk metrics and automated department benchmarks, the dashboard equips decision-makers to target retention strategies effectively and reduce costly turnover.

The Business Problem
Human resources and executive leadership require real-time visibility into workforce dynamics to minimize expensive recruitment cycles and preserve institutional knowledge. The objective of this analysis was to:

Identify which departments and job roles suffer from the highest voluntary turnover rates.

Track the impact of compensation, overtime, and tenure on employee churn.

Flag high-risk employee cohorts and engagement drop-offs for immediate HR intervention.

Tech Stack & Skills Used
Python (Pandas): Data cleaning, handling missing values, encoding categorical variables, and engineering composite satisfaction and workload scores from raw survey logs.

SQL (SQLite): Advanced data transformation utilizing Common Table Expressions (CTEs) and aggregations to calculate department-level turnover rates and tenure brackets.

Microsoft Power BI: Interactive data visualization, Power Query data validation, and custom DAX measure creation (e.g., Attrition Rate %, Average Employee Lifetime Value, Median Salary).

Methodology & Workflow
1. Data Engineering & Cleaning (Python/Pandas)
Ingested a 15,000+ row employee record dataset, removed duplicate entries, and addressed missing values in performance review logs.

Engineered custom features such as Overtime_Frequency_Ratio and Tenure_Bracket to group employees into clear analytical cohorts.

2. Statistical Aggregation (SQL)
Built an in-memory SQL database to process the cleaned HR data.

Executed relational queries to compute department-wise attrition benchmarks, comparing compensation percentiles against industry averages to isolate underpaid high-performers.

3. Data Visualization (Power BI)
Engineered custom DAX formulas for high-level KPIs (Total Headcount, Overall Attrition Rate %, Average Job Satisfaction).

Designed an executive layout featuring a Donut Chart for department breakdown and a Scatter Plot mapping Monthly Income against Years at Company, color-coded by attrition status.

Implemented cross-filtering so stakeholders can click a specific department and instantly isolate its primary churn drivers.

Key Insights
Departmental Risk: The Sales and Research & Development departments exhibit the highest voluntary attrition rates, driven primarily by recurring mandatory overtime.

Tenure Vulnerability: Employees within their 1st to 2nd year of tenure account for 45% of total resignations, highlighting onboarding or early career-pathing bottlenecks.

Compensation Impact: Employees with low stock options and below-median compensation in high-stress roles show a 3.2x higher likelihood of leaving within 90 days of an annual review cycle.

Files in this Repository
HR_Attrition_Prep.ipynb: The Python script containing the Pandas cleaning and feature engineering logic.

Cleaned_HR_Data.csv: The processed output dataset ready for BI ingestion.

Employee_Attrition_Dashboard.pbix: The final Power BI dashboard file.

Attrition_Dashboard_Preview.png: A high-resolution preview of the final visualizations.

Screenshots
