# Global Wage Dashboard

## Overview
This project is a **Power BI dashboard** that visualizes and analyzes global average wages across countries over time.  
It allows users to explore trends, compare countries, and identify anomalies in wage growth.  

The dashboard includes **interactive elements**, KPIs, and key measures that highlight important insights in a clear and professional format.

---

## Data Description
The dataset has been taken from kaggle (https://www.kaggle.com/datasets/meeratif/list-of-countries-by-average-wage-monthly-yearly)
The project uses **two main datasets**:

1. **`wage_development.csv`**  
   - Columns: `Country`, `Average Wage`  
   - Shows average wages for multiple countries (snapshot of latest year).  

2. **`Wage_History.csv`**  
   - Columns: `Country`, `Year`, `Avg_Monthly_Wage`  
   - Tracks wage development over time for each country.  

> Both datasets are included in the `data/` folder for reproducibility.
---

## Key Measures
The dashboard uses three main **DAX measures**:

1. **Global Average Wage**  
   - **What it does:** Calculates the overall average wage across all countries.  
   - **Purpose:** This card provides a quick snapshot of global wage levels, giving an overall benchmark for compar
2. **Latest Year Wage**  
   - **What it does:** Calculates the average wage for the most recent year in the dataset.  
   - **Purpose:** This measure shows the current wage level across all countries. It automatically updates if new data for future years is added, ensuring the dashboard always reflects the latest information.

3. **Wage Growth %**  
   - **What it does:** Calculates the percentage increase or decrease in wages for each country from the earliest available year to the latest year.  
   - **Purpose:** This measure highlights how much wages have changed over time per country.  
   - **Additional insight:** It helps identify anomalies, such as countries with negative growth or unusually high growth, which can then be emphasized using conditional formatting or KPI visuals.
