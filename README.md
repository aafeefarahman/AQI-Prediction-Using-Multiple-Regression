# 🌍AQI Prediction Using Multiple Regression

## 📌Project Description

This project analyses air quality data from multiple cities to understand how different pollutants influence the **Air Quality Index (AQI)**.

Using **Multiple Linear Regression**, the project models the relationship between AQI and major pollutants including **PM2.5, PM10, O₃, NO₂, SO₂, and CO**.

The analysis combines **statistical modelling in R** with **visual dashboard analysis in Excel** to better interpret pollution patterns.

---

# 🎯Project Objectives

The main goals of this project are:

1. 📊 Analyse air quality levels across cities
2. 🔍 Identify pollutants that most strongly influence AQI
3. 📈 Build a **Multiple Linear Regression model** to predict AQI
4. 📉 Create visual dashboards to explore pollution trends

---

# 📂Dataset Information

• **Type:** Secondary dataset
• **Source:** Mendeley Data – *Air Quality Index of Major Indian Cities and Stations*
• **Observations:** 154 cities/stations

### 📑Features Used

* City
* AQI
* PM2.5
* PM10
* O3
* NO2
* SO2
* CO
* Latitude
* Longitude
* Date
* Time

---

# Data Pre-processing

Before performing analysis, the following cleaning steps were applied:

* 🧽 Removed pollutant **units (µg/m³ and mg/m³)**
* 🔢 Converted pollutant values to **numeric format**
* ❌ Removed rows with **missing AQI values**
* 🧾 Cleaned non-numeric entries such as `"–"` or `"N/A"`
* ✔ Verified **unit consistency**
* 🔤 Standardised column formatting

---

# 📊Exploratory Data Analysis & Visualisation

### 📍 Top 10 Most Polluted Locations

Shows cities contributing most to **high AQI values**.
<img width="737" height="376" alt="image" src="https://github.com/user-attachments/assets/49786c81-bd08-45c1-b40a-96f5ab83be1d" />

---

### 📅AQI Trend Over Time

Visualises how **AQI changes across observation dates**.
<img width="721" height="426" alt="image" src="https://github.com/user-attachments/assets/48950275-106f-4635-9059-9b4c79681a26" />

---

### 🧪 Average Pollutant Levels

Compares the **average concentration of major pollutants** affecting AQI.
<img width="806" height="420" alt="image" src="https://github.com/user-attachments/assets/b166fd5a-ce37-47dd-b93e-cdf90cb7b072" />

---

### 🔬 PM2.5 vs AQI Relationship

Scatter plot showing the correlation between **PM2.5 concentration and AQI**.
<img width="869" height="452" alt="image" src="https://github.com/user-attachments/assets/8ca62b1c-8819-4588-ad66-f61fa344968e" />

---

# 📉Methodology – Multiple Linear Regression

A **Multiple Linear Regression model** was built using **R**.

### 🎯Dependent Variable

* AQI

### 🔬Independent Variables

* PM2.5
* PM10
* O3
* NO2
* SO2
* CO

### 📌Regression Model

```
AQI = β₀ + β₁(PM2.5) + β₂(PM10) + β₃(O3) + β₄(NO2) + β₅(SO2) + β₆(CO) + ε
```

---

# 🔎Example Prediction

The regression model can estimate AQI from pollutant values.

Example input:

* PM2.5 = 112.3
* PM10 = 53.2
* O3 = 16.7
* NO2 = 9.5
* SO2 = 9.8
* CO = 7.1

The model predicts the **corresponding AQI value**.

---

# 📌Key Findings

* 🔥 **PM2.5 has the strongest influence on AQI**
* ⚠ PM10 and NO₂ show moderate impact
* 🌫 SO₂ and CO contribute relatively less
* 📊 Most cities fall within **Moderate to Poor AQI categories**
* 📈 Higher PM2.5 concentrations strongly correlate with higher AQI

---

# 🛠Tools & Technologies

### 📊 Programming & Analysis

* R
* ggplot2
* Multiple Linear Regression (`lm()`)

### 📁 Data Handling

* CSV Dataset Processing
* Data Cleaning in R

### 📉 Visualisation

* Excel Dashboard
* Pivot Charts
* Scatter Plots
* Trend Analysis

---

---

# ▶ How to Run

## 1️⃣ Run Regression Analysis

Install required library:

```r
install.packages("ggplot2")
```

Run the script:

```r
source("regression_model.R")
```

---
# 🚀Future Improvements

Possible extensions to this project include:

📊 Building a machine learning model for AQI prediction

🌍 Expanding the dataset with more cities and longer time series

📈 Creating an interactive dashboard using Power BI or Tableau

🧠 Applying feature importance analysis to better interpret pollutant impact

🔮 Implementing time-series forecasting for AQI trends

---
