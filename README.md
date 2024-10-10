# Manchester-City-2023-2024-Premier-League-Analysis
**Introduction**

The Manchester City Premier League 2023/2024 Analysis project is a comprehensive Power BI dashboard that provides a detailed analysis of the team's performance throughout the season as they emerge champions. I sourced for their Premier League data online at the end of the season. I entered them on Microsoft Excel and then I made use of Power BI to create an interactive and insightful dashboard. Leveraging various data visualizations, this project presents key insights into match outcomes, goals statistics, comparative performance in home versus away games, the team top goal scorer and the team best player of the season. Designed for fans, analysts, and coaching staff, the dashboard offers an intuitive and interactive way to explore Manchester City's journey in the English Premier League, making it easier to identify trends, strengths, and areas for improvement.

**Project Overview**

This Power BI project provides an in-depth analysis of Manchester City's performance during the 2023/2024 English Premier League (EPL) season. The dashboard visualizes key metrics, offering insights into the team's match outcomes, goal statistics, performance at home and away, and more.

**Key Performance Indicators (KPIs)**

The analysis focuses on the following KPIs:

•	Match Outcomes (Win/Draw/Loss) Breakdown: Displays the number of wins, draws, and losses, along with their respective percentages.

•	Total Goals Scored vs. Conceded: Compares the total goals scored by Manchester City to the goals conceded across the season.

•	Average Goals per Game: Shows the average number of goals scored per match.

•	Goal Difference: Tracks the cumulative goal difference over the course of the season.

•	Home vs. Away Performance: Compares the team's performance in home and away matches.

•	Opposition Analysis: Breaks down goals scored and conceded against each opponent.

•	Top goal scorer, top assist, the team best player of the season and the winning head coach


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


**Visualizations**

**•	Match Outcomes Wins/Draws/Losses:** A card visualization showing the total number of wins, draws, and losses. Win/Draw/Loss Breakdown: A donut chart visualizing the percentage breakdown of wins, draws, and losses.

**•	Total Goals Scored vs. Conceded Clustered Column Chart:** Comparing the total goals scored and goals conceded across the season, with match outcome on the x-axis and the number of goals on the y-axis.

**•	Home vs. Away Performance Stacked Bar Chart:** Comparing the results in home versus away games, filtered by the venue.

•	Slicer to filter by venue.

