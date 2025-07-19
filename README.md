# Capstone-syamsu
Superstore Analysis - Data Classification and Summarization Using IBM Granite

# RAW Dataset Link
Dataset Title: Sample - Superstore
Source: Kaggle.com
Link: https://www.kaggle.com/datasets/vivek468/superstore-dataset-final/data

# Project Overview
Goals:
- Identify key profit drivers
- Detect low-performing segments
- Summarize insights using AI tools (IBM Granite)

# Analysis Project
1. Data cleaning and preparation
2. Grouping by Category, Region, Segment
3. Aggregating metrics: Sales, Profit, Quantity
4. Detecting anomalies and discount-profit correlation

# Insights and Findings
From the available data, Office Supplies appears to be the category with the highest key profit driver, with a mean profit of roughly $20.33 per unit. Furniture follows with a mean profit of about $8.70 per unit. There is no 'Technology' category present in the dataframe to comment on.
Based on the given data, the low-performing segments are ['Consumer']. These are the segments where the average profit is less than zero.\n\nExplanation:\n- We used the pandas `groupby` function to group the data by 'Segment' and then calculated the mean profit for each group using `df.groupby('Segment')['Profit'].mean()`.\n- We filtered the segments with mean profit less than zero using the `lt(0).index.tolist()` function, which returned the segment names as a list.\n- In this case, the list contained only one segment: 'Consumer'. This indicates that, on average, this segment is not profitable

# AI Support: IBM Granite
IBM Granite Instruct used to:
- Summarize tabular data
- Classify patterns in discount & profit
- Generate natural language insights









