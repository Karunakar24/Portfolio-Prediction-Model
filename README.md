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

## 📂 Project Structure
Portfolio-Prediction-Model/
│
├── notebooks/ # Jupyter notebooks (EDA, modeling)
├── data/ # Stock price datasets (if included)
├── src/ # Custom Python classes & scripts
├── visuals/ # Plots and result visualizations
├── README.md
└── .gitignore

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
*Location:* `visuals/feature_correlation_heatmap.png`

---

## 📈 Prediction Models

### 🔹 Random Forest Regressor
An ensemble learning model used to handle non-linear relationships and noise in financial data.

- Strengths: Robust to outliers, stable predictions  
- Limitation: Limited ability to capture sequential dependencies  

**Visualization:**  
*Location:* `visuals/random_forest_prediction.png`

---

### 🔹 Long Short-Term Memory (LSTM)
LSTM is a specialized recurrent neural network designed to model sequential and time-dependent data, making it ideal for stock price forecasting.

**Model Architecture**
- Two LSTM layers  
- Dense output layers  
- Sliding window input sequence  

**Visualizations:**
*Location:* `visuals/lstm_architecture.png`

*Location:* `visuals/lstm_prediction.png`

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
*Location:* `visuals/model_comparison.png`

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
*Location:* `visuals/portfolio_comparison.png`

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


