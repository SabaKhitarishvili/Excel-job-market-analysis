# Excel Job Market Analysis

An Excel-based data analysis project focusing on job market trends, salary insights, and skill demand. This project demonstrates practical data analysis and visualization skills using Excel.

## 📊 Excel Salary Dashboard

![image alt](https://github.com/SabaKhitarishvili/Excel-job-market-analysis/blob/e0f75b8de6195964602acc86f576d894f19ea4ee/Screenshot%202025-03-30%20at%2018.23.59.png)


## 🌟 Overview

This project presents a Salary Dashboard designed to help job seekers and professionals understand salary trends across different roles, locations, and industries. By leveraging Excel's powerful data analysis tools, I transformed raw job market data into an insightful, easy-to-navigate dashboard.

📂 Final Dashboard File: Excel_Job_Market_Analysis.xlsx


## 🔥 Key Excel Skills Used

📊 Data Visualization – Clear, insightful charts and graphs.

🧮 Advanced Formulas – Multi-condition filtering, aggregations, and calculations.

✔️ Data Validation – Ensuring clean and accurate data input.

🔍 Power Query & Power Pivot – Data extraction, transformation, and modeling.


## 📂 Dataset Information

This dataset contains real-world job market data from 2023, including:

💼 Job Titles (e.g., Data Scientist, Business Analyst, Data Engineer)

💰 Salaries (Annual salary data across different roles)

🌍 Locations (Country-wise salary distribution)

🛠️ Key Skills (Top skills required for data jobs)

The original dataset was refined and customized to enhance analysis and visualization.



## 📊 Dashboard Breakdown


1️⃣ Job Salaries by Role (Bar Chart)

Objective: Compare salaries across job roles.

Implementation: Horizontal bar chart sorted by salary (descending) for clarity.

Insights: Higher salaries are observed in senior roles like Data Engineers and Machine Learning Experts, while Analyst roles generally pay less.

2️⃣ Median Salaries by Country (Map Chart)

Objective: Show salary differences across regions.

Implementation: A world map with color-coded salary distributions.

Insights: The US and Western Europe have significantly higher salaries compared to other regions.


## 🏆 Advanced Excel Techniques

📌 Median Salary Calculation by Role

=MEDIAN(
IF(
    (jobs[job_title_short]=A2)*
    (jobs[job_country]=country)*
    (ISNUMBER(SEARCH(type,jobs[job_schedule_type]))) *
    (jobs[salary_year_avg]<>0),
    jobs[salary_year_avg]
)
)

✅ Purpose: Calculates median salary based on role, location, and job type.
✅ Dynamic Filtering: Ensures only relevant data is considered.

📌 Unique Job Types List

=FILTER(J2#, (NOT(ISNUMBER(SEARCH("and", J2#)) + ISNUMBER(SEARCH(",", J2#)))) * (J2#<>""))

✅ Purpose: Creates a clean, unique job type list for filtering.
✅ Application: Used in dropdowns for easy selection and analysis.


## ✅ Data Validation for Accuracy

To maintain data integrity, data validation rules were applied to

Job Titles (Standardized selection to avoid errors)

![image alt](https://github.com/SabaKhitarishvili/Excel-job-market-analysis/blob/0efe07787edbb0d41db6bfb28050eed07d3fbd68/Screenshot%202025-03-30%20at%2018.43.50.png)

Countries (Ensuring correct geographical classification)

![image alt](https://github.com/SabaKhitarishvili/Excel-job-market-analysis/blob/0efe07787edbb0d41db6bfb28050eed07d3fbd68/Screenshot%202025-03-30%20at%2018.44.25.png)

Job Types (Dropdown-based filtering for structured analysis)

![image alt](https://github.com/SabaKhitarishvili/Excel-job-market-analysis/blob/0efe07787edbb0d41db6bfb28050eed07d3fbd68/Screenshot%202025-03-30%20at%2018.44.36.png)

## 💡 Insights & Key Takeaways

📌 Senior roles and specialized positions generally offer higher salaries.
📌 Location plays a major role in salary variations, with notable differences between regions.
📌 Data validation & advanced formulas make the dashboard more interactive and user-friendly.


## 🚀 Personal Reflection

This project enhanced my Excel proficiency and allowed me to apply data analytics techniques to real-world job market trends. It highlights my ability to:
✅ Process and clean large datasets.
✅ Build meaningful visualizations.
✅ Extract insights for better decision-making.

📢 Feel free to explore the project and share your feedback! Connect with me on LinkedIn if you'd like to discuss this project or collaborate on similar work. 😊
