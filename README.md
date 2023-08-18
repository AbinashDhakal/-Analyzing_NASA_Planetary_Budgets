# Analyzing NASA Planetary Budgets
Welcome to the GitHub repository for analyzing NASA's planetary exploration budgets using SQL. In this project, we explore the financial aspects of NASA's planetary missions over the years and gain insights into spending patterns, adjustments for inflation, mission costs by destination, and more. This readme provides an overview of the project structure, objectives, and the SQL queries used to perform the analysis.

## Objective
The main objective of this project is to analyze NASA's planetary exploration budgets using SQL queries. We'll be working with a cleaned version of the public dataset provided by The Planetary Society, focusing on aspects such as:

Total cost of all planetary missions over all time.
Adjusting mission costs for inflation.
Identifying the most expensive mission.
Tracking annual spending trends.
Analyzing spending by destination.

## Dataset
The dataset used for this analysis includes two main tables: mission_budgets and inflation. Additionally, we'll utilize the mission_details table to analyze spending by destination. The tables have the following structure:

mission_budgets table:

mission: Name of the mission.
fiscal_year: Year for accounting purposes.
cost_type: Fine-grained aspect of the project (e.g., "Spacecraft").
cost_group: Broader aspect of the project (e.g., "Development/Implementation").
cost_MUSD: Cost in million US dollars.
inflation table:

fiscal_year: Year for accounting purposes (includes inflation-adjusted values for certain years).
inflation_adjustment: Multiplier to adjust currency values for inflation.
mission_details table:

mission: Name of the mission.
mission_full_name: Formal name of the mission.
destination: Place in the solar system that the mission is exploring.
program: NASA program that the mission is part of.
## Project Structure
The analysis is divided into multiple tasks, each focusing on a specific aspect of the data. The SQL queries for each task are provided along with brief explanations. The tasks include:

### Total Cost of All Planetary Missions
Calculating the total cost of all missions over all time.
### Adjusting for Inflation
Adjusting mission costs for inflation using the inflation table.
### Identifying the Most Expensive Mission
Identifying the mission with the highest total cost after adjusting for inflation.
### Annual Spending Trends
Grouping the budgets by year and calculating the adjusted total cost for each year.
Creating a bar plot to visualize annual spending trends.
### Spending by Destination
Joining budgets and mission details to analyze spending by destination.
Calculating the total adjusted cost for each destination.
### Spending by Destination Over Time
Joining budgets, inflation adjustments, and mission details.
Grouping by fiscal year and destination to analyze spending trends.
Creating a bar plot to visualize spending by year, colored by destination.
