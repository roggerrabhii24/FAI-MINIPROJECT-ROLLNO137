# FAI-MINIPROJECT-ROLLNO137

# 🌞 Solar Power Generation Prediction using Linear Regression

## 📘 Overview
This mini project uses **Machine Learning (Linear Regression)** to predict **solar AC power output** from a real solar power plant dataset in **Tamil Nadu, India**.  
The model analyzes factors such as **DC power**, **daily yield**, and **total yield** to accurately estimate the **AC power** generated.

---

## 🎯 Objective
To develop a regression-based ML model that predicts the solar energy output (AC Power) using available solar plant generation data.

---

## 🧩 Features in Dataset
| Column Name | Description |
|--------------|-------------|
| DATE_TIME | Timestamp of generation record |
| PLANT_ID | Unique ID of the solar plant |
| SOURCE_KEY | Unique ID for each inverter |
| DC_POWER | Power generated from solar panels (kW) |
| AC_POWER | Power delivered to the grid (kW) |
| DAILY_YIELD | Energy produced during the day (kWh) |
| TOTAL_YIELD | Cumulative energy produced (kWh) |

---

## ⚙️ Methodology
1. **Data Loading & Exploration**  
   - Imported dataset using Pandas  
   - Checked for missing values and data types  

2. **Feature Engineering**  
   - Extracted `HOUR`, `DAY`, and `MONTH` from `DATE_TIME`  
   - Selected relevant columns for training  

3. **Model Building**  
   - Used **Linear Regression** (from `sklearn`)  
   - Split dataset into training (80%) and testing (20%) sets  

4. **Model Evaluation**  
   - Evaluated using **MAE**, **MSE**, and **R² Score**  
   - Visualized Actual vs Predicted AC Power  

---

## 🧠 Algorithm Used
**Linear Regression**  
A supervised learning algorithm that models the linear relationship between input variables (DC Power, Yield) and the continuous target (AC Power).

---

## 📊 Results
| Metric | Value |
|---------|--------|
| Mean Absolute Error (MAE) | 0.7146 |
| Mean Squared Error (MSE) | 2.1365 |
| R² Score | 0.999986 ✅ |

**Result Interpretation:**  
The model performs exceptionally well with near-perfect prediction accuracy.

---

## 💡 Conclusion
The Linear Regression model successfully predicts solar power generation based on real-world data from an Indian solar power plant.  
Such models can be integrated into energy monitoring systems for **forecasting**, **efficiency analysis**, and **power optimization**.

---

## 📂 Dataset Information
- **Dataset Name:** Plant_1_Generation_Data.csv  
- **Location:** Tamil Nadu, India  
- **Source:** [Kaggle – Solar Power Generation Data](https://www.kaggle.com/datasets/anikannal/solar-power-generation-data)  
- **Plant Capacity:** 5 MW  

---

## 🖥️ Technologies Used
- Python 🐍  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- Google Colab  

---

## 📈 Visualization
A scatter plot was used to visualize the relationship between actual and predicted solar power outputs:

Actual vs Predicted Solar Power Output

---

## 🧾 Sample Prediction

| DC_POWER | DAILY_YIELD | TOTAL_YIELD | Predicted AC_POWER |
|-----------|--------------|--------------|--------------------|
| 500 | 1500 | 200000 | 49.24 |
| 2000 | 5000 | 210000 | 195.78 |
| 3500 | 9000 | 220000 | 342.32 |

---

## 👨‍💻 Author
** Abhishek Newaskar**  
Computer Engineering (AIML)  
DYPCET, Kolhapur  

---

## 🏁 Project Type
Mini Project – **Machine Learning (Linear Regression)**  
Academic Year: 2025  

---

## 🔗 Future Scope
- Add **weather and sunlight intensity data** for better prediction.  
- Integrate with IoT sensors for real-time solar energy monitoring.  
- Deploy model on web dashboard using **Flask or Streamlit**.  

---

*© 2025 – Machine Learning Mini Project | Solar Energy Forecasting*
