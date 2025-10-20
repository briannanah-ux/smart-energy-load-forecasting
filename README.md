# ⚡ Smart Energy Load Forecasting (24-Hour Ahead Prediction)

This repository showcases my MSc coursework project for **Data Analytics for Smart Energy Systems (2023/2024)**.  
It focuses on developing and evaluating **24-hour ahead load forecasting** models for the aggregate electricity consumption of 100 households in London, using real load and weather data from 2013.

---

## 🎯 Project Objective

The goal of this project was to:
- Forecast the **aggregate day-ahead electricity load** using historical hourly data.
- Compare the performance of **Multiple Linear Regression (MLR)** and **Neural Network (NN)** models.
- Explore how weather and temporal features (day, hour, season, etc.) affect electricity demand.

Accurate short-term load forecasting helps utilities:
- Maintain **grid stability** and reliability,  
- Plan **generation and market operations**, and  
- Enable **demand-side management** in smart grids.

---

## 🧩 Methodology

### 📊 Data
- **Period:** January – October 2013  
- **Training:** January – August  
- **Testing:** September – October  
- **Inputs:** 
  - Hourly electricity load (100 London households)
  - Temperature, humidity, and windspeed data  
  - Temporal indicators: day of week, time of day, holidays, and seasons

### ⚙️ Feature Engineering
- Lag features: load 24h and 168h prior  
- Qualitative indicators: day-of-week, time-of-day, and seasonal flags  
- Weather-based predictors: temperature, humidity, and windspeed  

### 🧠 Models Implemented
| Model | Description | Features Used |
|--------|--------------|----------------|
| MLR 1 | Baseline model (lag-24h + temperature) | Simple linear |
| MLR 2–3 | Added lag-168h and day-of-week | Weekly seasonality |
| NN 4–6 | Nonlinear models with ToD, holidays, weather | Deep learning approach |

Each model was trained on the same dataset to ensure a fair comparison.

---

## 🧰 Tools & Libraries
- **Language:** Python  
- **Core Libraries:** NumPy, Pandas, Matplotlib, Seaborn  
- **ML Libraries:** scikit-learn, TensorFlow, Keras  
- **Environment:** Jupyter Notebook  




# Launch notebook
jupyter notebook Coursework.ipynb
