# Sales Analysis ETL Project

## Overview

This project involves an ETL (Extract, Transform, Load) process for analyzing factors affecting sales in a large retail dataset. The primary goal is to understand how various factors, such as temperature and holidays, impact weekly sales across different stores.

## Dataset

The dataset used for this project includes the following columns:

- **Store**: The store identifier.
- **Date**: The date of the sales record.
- **Weekly_Sales**: The total sales for the week.
- **Holiday_Flag**: Indicates whether the week includes a holiday (1 for yes, 0 for no).
- **Temperature**: The average temperature for the week (in Fahrenheit).
- **Fuel_Price**: The average fuel price for the week.
- **CPI**: Consumer Price Index for the week.
- **Unemployment**: The unemployment rate for the week.

## Objectives

1. **Data Cleaning**: Identify and handle missing or incorrect values in the dataset.
2. **Date Transformation**: Convert date strings into proper date formats and extract relevant date components (like month and season).
3. **Data Aggregation**: Aggregate sales data by store, month, season, and holidays.
4. **Data Analysis**: Analyze the impact of temperature, seasons, and holidays on weekly sales.

## Methodology

1. **Extract**: Load the dataset using PySpark.
2. **Transform**:
    - Clean the data by dropping null values and correcting data types.
    - Create additional columns for month and season.
    - Identify holiday weeks based on the date.
3. **Load**: Store the transformed data back into a DataFrame for analysis.
4. **Analysis**: Perform aggregations to evaluate total weekly sales by store, month, season, and holiday impact.

## Key Findings

- Seasonal trends in sales were identified, with peaks occurring during specific months.
- The analysis revealed significant differences in sales during holidays compared to non-holidays.
- Temperature was explored as a potential factor affecting sales performance.

## Visualizations

- Bar charts illustrating total weekly sales by season.
- Comparison of sales on holidays versus non-holidays.

## Future Work

- Implement more complex analyses, such as regression modeling to predict sales based on various factors.
- Explore additional external datasets that may provide further insights (e.g., economic indicators).

## Technologies Used

- **Apache Spark**: For data processing and analysis.
- **Python**: Programming language for writing the ETL scripts.
- **Pandas**: For data manipulation and visualization.
- **Matplotlib/Seaborn**: For creating visualizations.

## How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/sales-analysis-etl.git

## Credits

The dataset used for this project was obtained from Kaggle. Special thanks to the Kaggle community for providing valuable datasets that support data science and machine learning projects.

[Link to Dataset on Kaggle]([https://www.kaggle.com/](https://www.kaggle.com/datasets/mikhail1681/walmart-sales/)) 
