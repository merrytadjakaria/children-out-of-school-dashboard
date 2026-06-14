# Children Out of School in Primary Age Dashboard
Interactive dashboard and exploratory analysis of primary school-age children out of school using R and Shiny.


## Project Overview
This project analyzes the global distribution of primary school-age children who are out of school using Unicef data.
The objective is to identify trends, geographic patterns, and socioeconomic factors associated with educational exclusion.
The analysis was conducted using R and visualized through an interactive dashboard.


## Business Problem
Despite significant global efforts to improve access to education, millions of primary school-age children remain out of school.
Understanding how this issue varies across countries, genders, and income groups is essential for policymakers, educational institutions, and international organizations seeking to design effective interventions.

This project aims to answer the following questions:
1. How has the number of out-of-school children changed over time?
2. Are there differences between boys and girls?
3. Which countries contribute the largest share of out-of-school children globally?
4. Is there a relationship between a country's income level and educational access?


## Data Collection and Initial Assessment
Source: data.unicef.org

The dataset contains information on primary school-age children who are out of school across multiple countries from 2011 to 2020.

Key variables include:
- Country Name
- Country Code
- Income Group
- Latitude
- Longitude
- Indicator Name
- Indicator Code
- Year
- Number of Children Out of School


## Data Cleaning and Preparation
### Data Quality Assessment
The dataset was imported from Excel and reviewed to assess completeness and structure.

Activities performed:
- Imported data using the readxl package.
- Inspected records and variable structure.
- Conducted missing value analysis.

Purpose:
To identify incomplete records and ensure the reliability of subsequent analyses.


### Data Cleaning
To improve data quality, records with missing values in critical fields were removed.

Variables checked:
- Latitude
- Longitude
- Income Group

Purpose:
These variables are required for geographic visualization and country-level analysis.


## Data Transformation
The original dataset stored yearly observations in separate columns.
The dataset was transformed from a wide format into a long format by converting yearly columns (2011–2020) into a single Year variable.

Additional transformations included:
- Standardizing variable data types.
- Converting categorical variables into factors.
- Creating a Gender variable derived from the indicator description.

Purpose:
To support time-series analysis, dashboard interactivity, and efficient visualization.


## Analysis and Visualization
### Analyze Trends by Gender
Research Question: How has the number of out-of-school children changed over time for boys and girls?

Methodology:
- Aggregated data by country, year, and gender.
- Calculated the total number of out-of-school children for each category.
- Developed an interactive line chart using ggplot2 and Plotly.

Purpose:
- Compare trends between boys and girls.
- Monitor changes over time.
- Identify periods of improvement or deterioration.


### Identify Geographic Hotspots
Research Question: Which countries contribute the largest share of out-of-school children globally?

Methodology:
- Calculated each country's contribution relative to the global total.
- Computed average contribution rates across the study period.
- Combined analytical results with geographic coordinates.

Purpose:
- Identify geographic concentrations of educational exclusion.
- Compare countries spatially.
- Detect regional patterns.


### Analyze the Impact of Income Level
Research Question: Is there a relationship between income level and the number of out-of-school children?

Methodology:
- Grouped countries according to income classifications data.
- Calculated average annual counts of out-of-school children.
- Compared distributions across income groups.
  
Purpose:
- Compare educational outcomes across income groups.
- Identify variation within each category.
- Detect potential outliers.


## Dashboard Features
The interactive dashboard allows users to:
- Select a country of interest.
- Explore historical trends from 2011 to 2020.
- Compare outcomes between boys and girls.
- Visualize country-level patterns on a world map.
- Analyze educational inequality across income groups


## Tools Used
- R
- RStudio
- Shiny
- ggplot2
- Plotly
- Leaflet
- dplyr
- tidyr
- readxl
- glue


## Skills Demonstrated
- Data Cleaning
- Data Wrangling
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Data Visualization
- Interactive Dashboard Development
- Geospatial Analysis
- Statistical Interpretation
- Data Storytelling
- Data Visualization

## Dashboard
https://merrytadjakaria.shinyapps.io/Education_Dashboard/

- Geospatial Analysis
- Dashboard Development
