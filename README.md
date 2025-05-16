# Manchester-City-2023-2024-Premier-League-Analysis
**Introduction**

The Manchester City Premier League 2023/2024 Analysis project is a comprehensive Power BI dashboard that provides a detailed analysis of the team's performance throughout the season as they emerge champions. I sourced for their Premier League data online at the end of the season. I entered them on Microsoft Excel and then I made use of Power BI to create an interactive and insightful dashboard. Leveraging various data visualizations, this project presents key insights into match outcomes, goals statistics, comparative performance in home versus away games, the team top goal scorer and the team best player of the season. Designed for fans, analysts, and coaching staff, the dashboard offers an intuitive and interactive way to explore Manchester City's journey in the English Premier League, making it easier to identify trends, strengths, and areas for improvement.

**Project Overview**

This project presents an interactive HR Analytics Dashboard built with Power BI, designed to provide key insights into workforce data such as employee demographics, job satisfaction, department composition, service years, and job levels. It allows HR professionals to make data-driven decisions by exploring employee-related metrics at a glance.


**Features**

**•  Employee Demographics**
Breakdown of employees by gender, marital status, and education field.

**•  Service Years Overview**
Visual distribution of employees based on years of service (1 to 10+ years).

**•  Job Level Distribution**
Count of employees across various job levels from Level 1 to Level 5.

**•  On-Service vs. Lay-Off Status**
Department-wise comparison of active vs. laid-off employees.

**•  Employee Distance Status**
Categorization based on proximity to the workplace (Very Close, Close, Very Far).

**•  Job Satisfaction by Role**
Insight into satisfaction levels across roles like Research Scientist, Sales Executive, Managers, etc.

**•  Education Field Analysis**
View of employee distribution by educational background.



**DAX Analysis**

Below are some key DAX measures used in the dashboard:

**•	Total matches played**

MATCHES PLAYED = COUNTROWS('EPL')

**•	Match Outcome Calculation:**

Wins = CALCULATE('EPL'[MATCHES PLAYED], 'EPL'[OUTCOME] = "Win")

Draws = CALCULATE('EPL'[MATCHES PLAYED], 'EPL'[OUTCOME] = "DRAW")

Losses = CALCULATE('EPL'[MATCHES PLAYED], 'EPL'[OUTCOME] = "Lost")


**•	Goals Scored:**

GOALS SCORED = SUM('EPL'[GOAL_FORWARD])

**•	Total Goals Conceded:**

GOALS CONCEDED = SUM('EPL'[GOAL_AGAINST])

**•	Average Goals per Game:**

AVG GOAL/MATCH = DIVIDE([GOALS SCORED], [MATCHES PLAYED], 0)


**Getting Started**
To explore or modify the dashboard:
1.  Open Power BI Desktop.
2.  Load the .pbix file (if available).
3.  If working with raw data:
    •  Import the dataset via Excel.
    •  Recreate visualizations using Power BI.

**Use Cases**
•  HR Decision Making
•  Workforce Planning
•  Employee Satisfaction Monitoring
•  Recruitment and Retention Analysis
•  Internal Reporting

**Preview**
See attached HR ANALYSIS DASHBOARD.pdf for a snapshot of the dashboard visuals.

**Feedback & Contributions**
Feel free to fork the repo, raise issues, or contribute improvements. Feedback and suggestions are welcome!
