# 📈 Portfolio Prediction Model
### Leveraging Machine Learning for Financial Forecasting

---

## 📌 Project Overview
This project presents a machine learning–based portfolio prediction system designed to forecast stock prices and evaluate portfolio performance using historical financial data. The system applies Long Short-Term Memory (LSTM) networks for time-series forecasting and compares results with a Random Forest Regressor to identify the most effective predictive approach.

The model focuses on a sample portfolio consisting of Apple (AAPL), Tesla (TSLA), and Google (GOOGL), and provides actionable insights through profit and loss analysis to support data-driven investment decisions.

---

## 🎯 Objectives
- Forecast next-day stock prices using historical market data  
- Compare LSTM and Random Forest models for financial time-series prediction  
- Analyze portfolio-level profit and loss based on predicted prices  
- Demonstrate practical application of machine learning in portfolio management  

---

## 🧠 Key Concepts & Techniques
- Time-Series Analysis  
- Feature Engineering & Data Normalization  
- Sliding Window Approach  
- Long Short-Term Memory (LSTM) Networks  
- Random Forest Regression  
- Portfolio-Level Profit/Loss Evaluation  
- Model Performance Metrics (MAE, MSE, RMSE)  

---

## 🛠️ Tech Stack
- **Programming Language:** Python  
- **Libraries & Tools:**  
  - NumPy, Pandas  
  - Scikit-learn  
  - TensorFlow / Keras  
  - Matplotlib, Seaborn  
  - yFinance  
- **Environment:** Jupyter Notebook  

---

## 📊 Data Collection & Preprocessing
Historical stock data is collected using the yfinance library, which provides reliable financial market data.

### Dataset Features
- Open Price  
- High Price  
- Low Price  
- Close Price  
- Volume  

### Preprocessing Steps
- Handling missing values using forward-fill  
- Removing invalid or zero-valued entries  
- Dropping irrelevant columns (Dividends, Stock Splits, Volume)  
- Normalizing data for model training  

### 📌 Visualization
**Feature Correlation Heatmap**  
<img width="1142" height="652" alt="image" src="https://github.com/user-attachments/assets/3572e9ff-ac7c-49ae-a7a5-2196e88aef52" />


**Closing Price History of ‘AAPL’ stock over the past 10 years.**
<img width="1144" height="610" alt="image" src="https://github.com/user-attachments/assets/69d82021-9c8d-4264-b05b-da943bdba02e" />

---

## 📈 Prediction Models

### 🔹 Random Forest Regressor
An ensemble learning model used to handle non-linear relationships and noise in financial data.

- Strengths: Robust to outliers, stable predictions  
- Limitation: Limited ability to capture sequential dependencies  

**Visualization:**  
<img width="846" height="457" alt="image" src="https://github.com/user-attachments/assets/81860460-547c-4610-9c33-842f010fe6a1" />


---

### 🔹 Long Short-Term Memory (LSTM)
LSTM is a specialized recurrent neural network designed to model sequential and time-dependent data, making it ideal for stock price forecasting.

**Model Architecture**
- Two LSTM layers  
- Dense output layers  
- Sliding window input sequence  

**Visualizations:**
<img width="847" height="458" alt="image" src="https://github.com/user-attachments/assets/a5161efc-ea25-4fb0-b99e-a9730637bfcd" />


---

## 📉 Model Evaluation
The dataset is split into:
- **80% Training**
- **20% Testing**

### Evaluation Metrics
- Mean Absolute Error (MAE)  
- Mean Squared Error (MSE)  
- Root Mean Squared Error (RMSE)  

**Model Comparison Visualization:**  
<img width="1529" height="815" alt="image" src="https://github.com/user-attachments/assets/5b4dec85-06b9-40e9-92f7-44c57af18c36" />


**Key Insight:**  
LSTM outperformed Random Forest in capturing sequential dependencies and volatile price movements, making it the preferred model for this project.

---

## 💼 Portfolio Prediction System
The system is implemented using custom Python classes to modularize functionality:

### Custom Classes
- **StockPredictionModel:** Builds, trains, and evaluates LSTM models  
- **Stock:** Handles data fetching, preprocessing, and feature engineering  
- **PortfolioPredictor:** Manages multiple stocks, predictions, and profit/loss calculations  

### Portfolio Allocation
- Apple (AAPL): 50%  
- Tesla (TSLA): 30%  
- Google (GOOGL): 20%  

**Portfolio Visualization:**  
<img width="1256" height="683" alt="image" src="https://github.com/user-attachments/assets/e21a87b2-2e19-4f2b-a1da-2ab545cef2e5" />
<img width="1300" height="708" alt="image" src="https://github.com/user-attachments/assets/be7fd1ee-40d2-4f83-b712-d0fad51e8e48" />
<img width="1278" height="696" alt="image" src="https://github.com/user-attachments/assets/7905d0de-2c57-4dd4-a7f0-63d89cf53358" />

**Stock Comparison:** 
<img width="1255" height="683" alt="image" src="https://github.com/user-attachments/assets/100a3c14-beb0-44e1-96aa-11fe8d406c8b" />

---

## 📊 Results & Insights
- LSTM demonstrated superior performance for time-series stock prediction  
- Portfolio-level profit/loss analysis provided actionable investment insights  
- The project highlights the importance of sequential modeling in financial forecasting  

---

## 🚀 Future Enhancements
- Integrate Transformer-based models  
- Add attention mechanisms for improved prediction accuracy  
- Build an interactive real-time portfolio dashboard  
- Enable dynamic stock inclusion and rebalancing  

---

## 🎓 Academic & Professional Relevance
- Demonstrates real-world application of machine learning in finance  
- Strong portfolio project for Data Analyst and Data Scientist roles  
- Showcases time-series modeling, evaluation, and business insight generation  


