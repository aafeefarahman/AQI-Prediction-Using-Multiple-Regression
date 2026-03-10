# AQI Prediction Using Multiple Regression

## Project Description

This project analyses air quality data from multiple cities to understand how different pollutants influence the **Air Quality Index (AQI)**.

Using **multiple linear regression**, the project models the relationship between AQI and major pollutants including **PM2.5, PM10, O₃, NO₂, SO₂, and CO**.

The analysis combines **statistical modelling in R** with **interactive dashboard visualisations in Excel** to better interpret pollution patterns.

---

# Project Objective

The objectives of this project are to:

• Analyse air quality levels across cities
• Understand which pollutants influence AQI the most
• Build a **multiple regression model to predict AQI**
• Create **visual dashboards to explore pollution trends**

---

# Dataset Information

**Type:** Secondary dataset
**Source:** Mendeley Data – *Air Quality Index of Major Indian Cities and Stations*
**Observations:** 154 cities/stations

### Features

| Feature   | Description               |
| --------- | ------------------------- |
| City      | Monitoring location       |
| AQI       | Air Quality Index         |
| PM2.5     | Fine particulate matter   |
| PM10      | Coarse particulate matter |
| O3        | Ozone                     |
| NO2       | Nitrogen dioxide          |
| SO2       | Sulphur dioxide           |
| CO        | Carbon monoxide           |
| Latitude  | Geographic coordinate     |
| Longitude | Geographic coordinate     |
| Date      | Observation date          |
| Time      | Observation time          |

---

# Data Pre-processing

Before performing analysis, the following cleaning steps were applied:

• Removed units such as **µg/m³ and mg/m³**
• Converted pollutant values to numeric format
• Removed rows with missing AQI values
• Cleaned non-numeric entries such as "–" or "N/A"
• Checked consistency of pollutant units
• Standardised column formatting

---

# Exploratory Data Analysis & Visualisation

An **Excel dashboard** was created to explore pollution patterns across cities.

### AQI Dashboard

<img src="images/dashboard.png" width="900">

---

### Top 10 Most Polluted Locations

Shows cities contributing most to high AQI values.

<img src="images/top10_locations.png" width="600">

---

### AQI Trend Over Time

Visualises how AQI levels change across observation dates.

<img src="images/aqi_trend.png" width="600">

---

### Average Pollutant Levels

Compares the average concentration of major pollutants affecting AQI.

<img src="images/average_pollutants.png" width="600">

---

### PM2.5 vs AQI Relationship

Scatter plot showing correlation between **PM2.5 concentration and AQI**.

<img src="images/pm25_vs_aqi.png" width="600">

---

# Methodology – Multiple Linear Regression

A **multiple linear regression model** was fitted using R.

### Dependent Variable

AQI

### Independent Variables

PM2.5
PM10
O3
NO2
SO2
CO

### Regression Model

AQI = β₀ + β₁(PM2.5) + β₂(PM10) + β₃(O3) + β₄(NO2) + β₅(SO2) + β₆(CO) + ε

---

# Example Prediction

The model can estimate AQI given pollutant concentrations.

Example:

PM2.5 = 112.3
PM10 = 53.2
O3 = 16.7
NO2 = 9.5
SO2 = 9.8
CO = 7.1

Predicted AQI is calculated using the regression model.

---

# Key Findings

• **PM2.5 has the strongest influence on AQI**
• PM10 and NO2 show moderate impact
• SO2 and CO contribute relatively less
• Most cities fall within **moderate to poor AQI categories**

---

# Tools and Technologies

**Programming & Analysis**

• R
• ggplot2
• Multiple Linear Regression (lm)

**Data Processing**

• Base R
• CSV dataset handling

**Visualization**

• Excel Dashboard
• Pivot Charts
• Scatter Plots
• Trend Analysis

---

# How to Run

### Run Regression Analysis

1. Open the R script
2. Install required library

```r
install.packages("ggplot2")
```

3. Run the script

```r
source("regression_model.R")
```
