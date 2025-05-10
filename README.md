# 🏠🔌 Energy Consumption in Buildings – Dataset Overview

## 📄 About the Dataset

This dataset contains information on energy consumption patterns in **residential** and **commercial** buildings. It supports classification of energy usage into **Low**, **Medium**, and **High**, based on structural, behavioral, and environmental factors.

The data is ideal for **Excel-based analysis**, with compatibility for pivot tables, charts, and dashboards.

---

## 📊 Dataset Summary

**File Name:** `Energy_Consumption_Prediction.csv`  
**Size:** 71.51 KB  
**Rows:** ~1000  
**Columns:** 11

### 🔑 Features:

| Column Name              | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| `Building_Type`          | Type of building – **Residential** or **Commercial**                       |
| `Floor_Area`             | Total building area in square feet                                          |
| `Number_Of_Occupants`    | Average daily number of occupants                                           |
| `Insulation_Type`        | Insulation rating – **Good**, **Average**, or **Poor**                      |
| `Appliance_Count`        | Number of electrical appliances in use                                      |
| `Average_Temperature`    | Daily average temperature (°C)                                              |
| `HVAC_Efficiency`        | HVAC system efficiency score (0.50 to 1.00)                                 |
| `Energy_Sources`         | Primary energy source – **Electric**, **Gas**, or **Hybrid**                |
| `Peak_Usage_Hours`       | Hours per day when energy use peaks                                         |
| `Annual_Energy_Cost`     | Yearly energy cost in USD                                                   |
| `Energy_Consumption_Class` | Target variable: **Low**, **Medium**, or **High** energy consumption class |

---

## 🔍 Research Questions

These questions guide the analysis and dashboard insights:

### 💡 Energy Usage & Source
1. **What source of energy is used the most between Electric, Gas, and Hybrid?**  
2. **Does the type of energy determine the cost spent on energy?**  

### 💰 Cost Analysis
3. **Between commercial and residential buildings, which spend the most on energy?**  
4. **Does insulation type determine the cost of energy?**  
5. **How does HVAC efficiency correlate with annual energy costs?**

### ⚙️ Consumption Patterns
6. **How does average temperature influence energy consumption levels?**  
7. **Does insulation type significantly affect energy consumption?**  

---

## 📈 Tools & Techniques for Excel Analysis

- **Pivot Tables** for grouped insights (e.g., by building type, energy source)
- **Pivot Charts & Slicers** for interactive dashboards
- **Bar & Column Charts** for comparison across categories
- **Scatter Plots** to assess correlations (e.g., HVAC vs Cost)
- **Conditional Formatting** to highlight trends in cost and efficiency
- **Regression Analysis** using Excel's Data Analysis Toolpak for insights into cause-effect relationships

---

## 📉 Regression Analysis: Does Insulation Type Affect Energy Cost?

A linear regression using Excel was conducted to determine whether a building's insulation type influences **Annual Energy Cost**.

### 📊 Key Regression Results:

| Metric                  | Value         |
|-------------------------|---------------|
| **R Square**            | 0.0010        |
| **Adjusted R Square**   | -0.0020       |
| **F-statistic**         | 0.517         |
| **Significance F**      | 0.671         |
| **Observations**        | 1000          |

### 🔍 Coefficient Summary:

| Insulation Type | Coefficient | P-Value | Interpretation |
|------------------|-------------|---------|----------------|
| **Intercept**    | 5320.75     | <0.001  | Baseline average annual cost |
| **Poor**         | +115.55     | 0.563   | Slight increase (not significant) |
| **Average**      | 0 (baseline)| —       | Reference category |
| **Good**         | -82.80      | #NUM!   | Slight decrease (not significant) |

### 🧠 Interpretation:

- **Very low R² (0.001)** indicates insulation explains almost none of the variance in cost.
- **P-values > 0.05** mean differences between insulation types are not statistically significant.
- Conclusion: **Insulation type does not significantly impact annual energy cost** in this dataset.

---

