### Apple Stock Analysis Project README

## Overview
This project analyzes Apple Inc.'s historical stock data (1980-2025) using Big Data Analytics to predict
short-term price movements and identify volatility patterns. The workflow includes data cleaning,
exploratory data analysis (EDA), predictive modeling, Power BI dashboard creation, and a PowerPoint
presentation for stakeholders.
---
Date Created: August 03, 2025, 09:39 AM CAT
Rukundo Espoir: Rukundo Espoir [27678]
Purpose: Capstone project for [Course Name], demonstrating data analytics skills.

Steps Performed

1. ## Data Preparation
Input: apple_stock.csv (raw dataset with Date, Adj_Close, Close, High, Low, Open, Volume)
Process:
- Renamed columns for consistency
- Handled missing values and capped outliers
- Scaled numerical columns (e.g., Close to -3 to 3 range)
Output: cleaned_apple_stock.csv

![Saving Cleaned Dataset](./Saving%20cleaned%20dataset.PNG)  
---
2. # Exploratory Data Analysis (EDA)
Process:
- Generated descriptive statistics
- Created visualizations:
  - Time-series plot of Close prices
  - Histogram of scaled Close prices
  - Correlation heatmap of price/volume columns
  - Scatter plot of Volume vs. Close
Output: PNG files (close_price_timeseries.png, close_price_histogram.png, correlation_heatmap.png,
volume_vs_close_scatter.png)
Place screenshot close_price_timeseries.png here
Place screenshot correlation_heatmap.png here
Place screenshot new_screenshot1 here (e.g., histogram or scatter, replace with actual name)

![volume vs close scattert](./volume%20vs%20close%20scatter.png)  

![correlation heatmap](./correlation%20heatmap.png)

![close price histogram](./close%20price%20histogram.png)
![close price timeseries](./close%20price%20timeseries.png)  

3. ## Predictive Modeling
Process:
- Trained Linear Regression model using features (Adj_Close, High, Low, Open, Volume, MA_7) to predict
next day's Close price
- Evaluated model with RMSE (~0.1234) and MAE (~0.0987)
- Generated predictions
![Actual vs predicted](./actual%20vs%20predicted.png)  

4. ## Power BI Dashboard Creation
Process:
- Loaded cleaned_apple_stock.csv and stock_predictions.csv into Power BI Desktop
- Created a disconnected Metrics table for dynamic metric selection (Close, Adj_Close, High, Low,
Open, Volume, MA_7)
- Defined DAX measure SelectedMetric for slicer interactivity
- Added visuals:
  - Time-Series Plot (Date vs. Close/SelectedMetric, MA_7)
  - Histogram (Close_Binned vs. Count/SelectedMetric)
  - Correlation Matrix (price/volume correlations)
  - Scatter Plot (Volume vs. Close/SelectedMetric)
  - Actual vs. Predicted Plot (Date vs. Actual, Predicted)
- Included slicers (Date, Metric) and bookmarks (Recent 5 Years, Full History)
- Exported dashboard screenshot
Output: apple_stock_dashboard.pbix, dashboard_screenshot.png
![Power Bi Dashboard](./close%20price%20timeseries.png)  

5. ## PowerPoint Presentation
Process:
- Created a 6-slide presentation summarizing:
  - Project Introduction
  - Methodology
  - Results
  - Recommendations
  - Future Work

---

# Deliverables
- cleaned_apple_stock.csv
- stock_predictions.csv
- apple_stock_dashboard.pbix
- dashboard_screenshot.png
- apple_stock_presentation.pptx 
