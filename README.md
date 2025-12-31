# Subqueries & CTEs
**By: Taran Schlichtmann**
**Date: 10/28/2025**

SQL Analysis Using Snowflake

Applying subqueries, Common Table Expressions (CTEs), and SQL best practices to analyze U.S. Census data stored in Snowflake. The assignment required writing SQL, following a style guide, and exporting results into an Excel workbook.

------------------------------------------------------------
Overview
------------------------------------------------------------

The goal of this assignment was to demonstrate proficiency in:

- Writing CASE statements
- Using subqueries for filtering
- Building multi‑step transformations using CTEs
- Performing population and demographic analysis
- Applying SQL style conventions
- Exporting query results for reporting

All work was executed in Snowflake using the CLASSWORK warehouse and the CENSUS database.

------------------------------------------------------------
Repository Contents
------------------------------------------------------------

GB882_Assignment 4_Subqueries and CTEs_Schlichtmann_T.txt  
    All SQL statements written for the assignment.

GB882_Assignment 4_Subqueries and CTEs_Schlichtmann_T.xlsx  
    Excel workbook containing query results in separate tabs.

README.md  
    Documentation and context for the assignment.

------------------------------------------------------------
Assignment Summary
------------------------------------------------------------

Query 1 — Advanced Degree Concentration by Zip Code  
Identified zip codes with a high percentage of residents holding a master’s degree.  
Included:
- Percentage of population with an advanced degree
- Classification (High ≥ 5%, otherwise Low)
- 2018 data only
- Population > 0
- Sorted by highest percentage

Result Insight:  
There were 16 zip codes where at least 60% of residents held an advanced degree.

------------------------------------------------------------

Query 2 — Household Counts in Key Counties  
Used a subquery to filter zip codes located in:
- Clark County, NV
- Los Angeles County, CA
- Maricopa County, AZ

Returned 2018 household counts, sorted from most to fewest.

Result Insight:  
Zip code 90250 (Hawthorne, CA) had 31,978 households in 2018.

------------------------------------------------------------

Query 3 — Population Growth Analysis (CTEs)  
Built a multi‑step CTE pipeline to:
1. Extract 2013 population
2. Extract 2018 population
3. Calculate numeric and percentage growth
4. Filter zip codes with ≥ 5,000 residents in 2013
5. Rank by percentage growth

Result Insight:  
Zip code 92618 had the highest percentage population growth.

------------------------------------------------------------
Tools & Technologies
------------------------------------------------------------

- Snowflake (SQL execution & data exploration)
- Excel (result storage & reporting)
- SQL Style Guide (formatting & readability standards)

------------------------------------------------------------
Skills Demonstrated
------------------------------------------------------------

- Analytical SQL (CASE, CTEs, subqueries)
- Data quality filtering
- Multi‑step transformation logic
- Clean, readable SQL following style conventions
- Reproducible result export workflows
