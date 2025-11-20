B"H

# U.S. Childcare Costs: Economic Patterns and Affordability Challenges

## Research Question
What patterns exist in childcare costs across the United States, and how do geographic and economic disparities create different affordability realities for families across different regions and income levels?

## Project Overview
This project analyzes the National Database of Childcare Prices dataset to reveal important patterns in the U.S. childcare market, focusing on how geographic and economic disparities create vastly different childcare realities for families across the country. The analysis examines costs by age group, care type (center-based vs. family-based), geographic region, and affordability metrics expressed as the share of median household income required for full-time care.

The project encompasses three major components:

1. **Data Preparation & Integration** - Resolving schema drift between years, re-indexing all dollar amounts to 2023 values using CPI-U, building county-to-state aggregates, handling missing county-year observations (<3%) with forward-filling, and exporting tidy JSON to power interactive visualizations

2. **Exploratory Analysis & Findings** - Discovering clear progression of costs by age group (infant care most expensive), center-based vs. family-based care premiums (10-40% depending on geography), strong positive correlation (ρ≈0.62) between median household income and childcare costs, and affordability crisis with national average at 15.9% of income (well above 7% federal benchmark)

3. **Interactive Visualization Development** - Creating an interactive HTML/JavaScript dashboard with geographic choropleth maps showing costs as percentage of median household income by county, filtering capabilities for age groups and care types, state comparison tools, and supporting materials including infographics and presentation decks for policymakers

The project demonstrates advanced data visualization and storytelling techniques including interactive web development with D3.js, accessibility-focused design (color-blind palettes), transparent data transformation documentation, and stakeholder-focused communication. Key findings reveal that while raw costs vary dramatically by region, the proportion of income spent on childcare creates significant financial strain for middle-income families, with counties in the Boston-to-D.C. corridor routinely exceeding 25% of household income.

## Project Files
- [Interactive Dashboard (HTML)](https://dovkoy.github.io/msds-portfolio/projects/child_care_cost/dashboard.html)
- [Dashboard Data (JSON)](https://github.com/dovkoy/msds-portfolio/tree/trunk/docs/projects/child_care_cost/dashboard_data.json)
- [Infographic (PDF)](https://github.com/dovkoy/msds-portfolio/tree/trunk/docs/projects/child_care_cost/infographic.pdf)
- [White Paper (PDF)](https://github.com/dovkoy/msds-portfolio/tree/trunk/docs/projects/child_care_cost/white_paper.pdf)
- [Dashboard Screenshot (PDF)](https://github.com/dovkoy/msds-portfolio/tree/trunk/docs/projects/child_care_cost/dashboard_screenshot.pdf)

