# AQI Prediction Using Multiple Regression

## 📌 Project Description

A data analysis project using a secondary dataset of 154 cities to study air quality and apply multiple linear regression to understand how major pollutants (PM2.5, PM10, O₃, NO₂, SO₂ and CO) influence the Air Quality Index (AQI).

---

## 🎯 Project Objective

The main objective of this project is to:

* analyse air quality levels across different cities, and
* identify which pollutants have the strongest impact on AQI using multiple regression analysis.

---

## 📂 Dataset Information

* Type: Secondary dataset
* Number of cities: 154
* Source: Mendeley Data – *Air Quality Index of Major Indian Cities and Stations*
* Coverage: Indian cities and a few international locations

### Features used

* City
* AQI
* PM2.5
* PM10
* O₃
* NO₂
* SO₂
* CO

---

## 🧹 Data Pre-processing

The following steps were performed before analysis:

* Removal of rows with completely missing values
* Handling partial missing values using N/A
* Removal of duplicate city records
* Standardisation of city names
* Cleaning non-numeric values such as “–” and “N/A”
* Verification of unit consistency

---

## 🗂 Final Variables Used

| Variable | Description                         |
| -------- | ----------------------------------- |
| AQI      | Air Quality Index (target variable) |
| PM2.5    | Fine particulate matter             |
| PM10     | Coarse particulate matter           |
| O₃       | Ozone                               |
| NO₂      | Nitrogen dioxide                    |
| SO₂      | Sulphur dioxide                     |
| CO       | Carbon monoxide                     |

---

## 🏷 Air Quality Categorisation

The pollutants and AQI values were classified into:

* Good
* Moderate
* Poor

based on:

* U.S. EPA guidelines for AQI
* WHO Global Air Quality Guidelines for pollutants.

---

## 📊 Exploratory Data Analysis

The following visual analyses were performed:

* Pareto chart for AQI by city
* Pareto chart for PM2.5 by city
* Pareto chart for PM10 by city
* Pareto chart for O₃ by city
* Pareto chart for SO₂ by city
* Line chart with error bars for NO₂ levels

These charts were used to identify the cities contributing most to overall pollution.

---

## 📐 Methodology – Multiple Linear Regression

### Dependent Variable

* AQI

### Independent Variables

* PM2.5, PM10, O₃, NO₂, SO₂, CO

### Regression model

AQI = β₀ + β₁(PM2.5) + β₂(PM10) + β₃(O₃) + β₄(NO₂) + β₅(SO₂) + β₆(CO) + ε

---

## 📈 Average Pollution Levels (154 Cities)

| Pollutant | Average Value |
| --------- | ------------- |
| AQI       | 107.18        |
| PM2.5     | 112.3 µg/m³   |
| PM10      | 53.2 µg/m³    |
| O₃        | 16.7 µg/m³    |
| NO₂       | 9.5 µg/m³     |
| SO₂       | 9.8 µg/m³     |
| CO        | 7.1 mg/m³     |

---

## 🧮 Conceptual Regression Model (for interpretation)

AQI = 26.88

* 0.50(PM2.5)
* 0.30(PM10)
* 0.20(O₃)
* 0.40(NO₂)
* 0.10(SO₂)
* 0.15(CO)

*(Conceptual coefficients are used to demonstrate relative contribution.)*

---

## 🔍 Key Findings

* PM2.5 is the largest contributor to AQI.
* PM10 and NO₂ show moderate influence.
* SO₂ and CO contribute comparatively less.
* Most cities fall under moderate to poor air quality categories.

---

## 🛠 Tools and Technologies

* Python
* Pandas
* NumPy
* Matplotlib / Seaborn
* Jupyter Notebook

---

## 📁 Project Structure

```
├── dataset/
│   └── air_quality_data.csv
├── notebooks/
│   └── aqi_analysis.ipynb
├── charts/
│   └── generated_plots
├── README.md
```

---

## ▶ How to Run

1. Clone the repository
2. Open the notebook file
3. Install required libraries
4. Run all cells in order

---
