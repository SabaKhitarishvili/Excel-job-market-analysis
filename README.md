Excel Job Market Analysis

An Excel-based data analysis project focusing on job market trends, salary insights, and skill demand. This project demonstrates practical data analysis and visualization skills using Excel.

📊 Excel Salary Dashboard

Introduction

This salary dashboard project is my customized analysis of job market trends, designed to help job seekers explore salary variations across different roles, locations, and job types. The dashboard provides key insights into how job titles, regions, and required skills influence salaries, aiding informed career decisions.

Dashboard File

My final dashboard file: Excel_Job_Market_Analysis.xlsx

🛠 Excel Skills Highlighted

In creating this project, I applied several advanced Excel skills, including:

📊 Data Visualization: Charts and graphs for clear and impactful insights.

🧮 Advanced Formulas: Multi-condition filtering, aggregations, and dynamic calculations.

✔️ Data Validation: Ensuring accuracy and consistency in data inputs.

🔍 Power Query & Power Pivot: Data extraction, transformation, and modeling.

📂 About the Dataset

The dataset consists of real-world job market data from 2023 and includes:

💼 Job Titles

💰 Salaries

🌍 Locations

🛠️ Key Skills

The original dataset was modified and refined to enhance analysis and visualization within this dashboard.

📊 Dashboard Components

📈 Job Salaries by Role (Bar Chart)

Objective: Show salary variations across job roles.

Implementation: A horizontal bar chart sorted by descending salaries for easy comparison.

Insights: Senior-level roles such as Data Engineers and Data Scientists command significantly higher salaries compared to Analyst roles.

🗺️ Median Salaries by Country (Map Chart)

Objective: Visualize global salary trends.

Implementation: A map chart with color gradients indicating salary variations across regions.

Insights: Clear disparities exist between regions, with the US and Western Europe offering higher median salaries.

🧮 Advanced Formulas

Median Salary Calculation by Role

Formula Example:

=MEDIAN(
IF(
    (jobs[job_title_short]=A2)*
    (jobs[job_country]=country)*
    (ISNUMBER(SEARCH(type,jobs[job_schedule_type]))) *
    (jobs[salary_year_avg]<>0),
    jobs[salary_year_avg]
)
)

Purpose: Calculate median salary based on multiple criteria (role, location, job type).

Dynamic Filtering: Ensures relevant data is used for accurate results.

Unique Job Types List

Formula Example:

=FILTER(J2#, (NOT(ISNUMBER(SEARCH("and", J2#)) + ISNUMBER(SEARCH(",", J2#)))) * (J2#<>""))

Purpose: Generate a clean list of unique job types for filtering.

Application: Used in dropdowns for user input validation.

✅ Data Validation

To enhance usability, data validation rules were implemented for:

Job Titles

Countries

Job Types

This ensures consistent input and eliminates errors caused by invalid entries.

📢 Acknowledgment

This project was inspired by various Excel learning resources and serves as a practical application of data analysis techniques.

💡 Insights and Takeaways

Senior-level roles and specialized positions tend to command higher salaries.

Geographic location significantly influences salary ranges, with notable disparities between countries.

Data validation and advanced formulas make the dashboard user-friendly and efficient for exploring the dataset.

🔍 Personal Reflection

This project allowed me to refine my Excel skills while exploring real-world job market trends. It showcases my ability to analyze data, extract meaningful insights, and present them effectively through visualization.

Feel free to check out the project and share your feedback. Connect with me on LinkedIn to discuss this project or any collaboration opportunities!
