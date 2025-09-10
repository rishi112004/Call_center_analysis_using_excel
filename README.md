

# Call Center Performance Analysis

## Project Overview

This project provides a comprehensive analysis of call center data. The primary objective is to evaluate key performance indicators (KPIs) related to call volume, representative performance, customer satisfaction, and sales.

An interactive dashboard was created to visualize these metrics, allowing stakeholders to easily identify trends, uncover insights, and make data-driven decisions to improve call center operations and customer service.

## Dashboard Preview

## Data Source

The analysis is based on a dataset containing detailed information about call logs and customer demographics. The data is structured into two main tables:

1.  **Call Data**: Contains transactional records for each call.

      * **Key Columns**: `Call number`, `Customer ID`, `Duration` (in seconds), `Representative`, `Date of Call`, `Purchase Amount`, `Satisfaction Rating`.

2.  **Customer Data**: Contains demographic information about the customers.

      * **Key Columns**: `Customer ID`, `Gender`, `Age`, `City`.

These tables are linked via the `Customer ID` column.

## Tools Used

  * **Data Cleaning & Transformation**: Microsoft Excel / Power Query
  * **Data Analysis & Calculations**: Microsoft Excel (Formulas, Pivot Tables) / Power BI (DAX)
  * **Data Visualization**: Microsoft Excel / Power BI

## Project Methodology

1.  **Data Loading**: The raw data was imported from the provided CSV files (`Data.csv` and `Assets.csv`).
2.  **Data Cleaning and Transformation**:
      * Checked for and corrected inconsistencies and typos in the dataset.
      * Created calculated columns to aid analysis, such as `Duration Bucket` to categorize calls based on their length and `Day of week` extracted from the call date.
3.  **Data Modeling**: Established a relationship between the 'Call Data' and 'Customer Data' tables using the `Customer ID` as the primary key. This allows for segmenting call performance by customer demographics.
4.  **KPI Development**: Defined and calculated the core metrics for the dashboard:
      * **Total Calls**: The total number of calls received.
      * **Total Purchase Amount**: The sum of all purchases made over the calls.
      * **Average Satisfaction Rating**: The mean customer satisfaction score, rated on a scale of 1-5.
      * **Average Call Duration**: The average length of a call in seconds.
5.  **Dashboard Creation**: Designed an interactive and user-friendly dashboard to visualize the data and KPIs. The dashboard includes:
      * **KPI Cards**: For a quick overview of the main metrics.
      * **Bar Charts**: To compare `Purchase Amount` by representative and by day.
      * **Line Chart**: To track `Satisfaction Rating` trends across the days of the week.
      * **Donut Charts**: To show the proportion of `Calls by Duration` and `Calls by City`.
      * **Slicers**: Interactive filters for `Day of week` and `Representative` to allow for dynamic data exploration.

## Key Insights & Findings

The dashboard provides answers to critical business questions, including:

  * **Representative Performance**: Which representatives are driving the most revenue?
  * **Customer Satisfaction**: What is the overall satisfaction level, and are there specific days when it is higher or lower?
  * **Peak Performance Days**: Which days of the week have the highest purchase amounts and satisfaction ratings?
  * **Geographical Trends**: Which cities generate the highest call volumes?
  * **Call Efficiency**: What is the typical duration of a call, and how does it correlate with other metrics?

## How to Use the Dashboard

The dashboard is fully interactive:

  * **Filter by Representative**: Select one or more representatives from the 'Representative' slicer to view their individual performance.
  * **Filter by Day**: Use the 'Day of week' slicer to isolate data for specific days and analyze weekly trends.
  * All charts and KPIs on the dashboard will dynamically update based on your selections.
