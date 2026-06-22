# 📈 Apple Stock Price Forecasting with PySpark

##  Project Overview

This project implements a distributed time-series forecasting system using PySpark to predict future Apple stock prices from historical market data.

The project demonstrates how machine learning and distributed computing can be applied to financial forecasting problems by transforming stock market data into a supervised learning format and training predictive regression models.

The workflow includes feature engineering, time-series preprocessing, model training, evaluation, and visualization of forecasting results.

---

##  Project Objectives

The objectives of this project are to:

- Perform financial time-series forecasting using PySpark
- Create lag-based and rolling statistical features
- Convert time-series data into a supervised learning dataset
- Train machine learning regression models
- Compare forecasting performance using evaluation metrics
- Visualize actual versus predicted stock prices

---

## 🛠 Technologies Used

- Python
- PySpark
- Spark MLlib
- Pandas
- NumPy
- Matplotlib
- Google Colab

---

##  Dataset

### Apple Stock Dataset

The dataset contains historical Apple stock market information, including:

- Date
- Open Price
- High Price
- Low Price
- Close Price
- Trading Volume

### Target Variable

- Close Price

The goal is to predict future stock closing prices based on historical market behaviour.

Dataset Source:

https://www.kaggle.com/datasets/ayeshaaqib/apple-stock-data-1999-2024

---

##  Project Workflow

### 1. Data Loading

- Load historical stock market data
- Convert data into a Spark DataFrame
- Sort observations chronologically

### 2. Feature Engineering

Time-series features were created using Spark window functions:

#### Lag Features

- Previous day closing prices
- Historical stock behaviour

#### Rolling Statistics

- Rolling averages
- Moving trends
- Market momentum indicators

### 3. Data Preparation

- Remove missing values created by lag calculations
- Assemble features into a machine learning pipeline
- Split data into training and testing sets

### 4. Model Training

The following regression models were implemented:

#### Linear Regression

Used as a baseline forecasting model.

#### Gradient Boosted Trees (GBT)

Used to capture more complex and nonlinear relationships in stock price movements.

---

##  Model Evaluation

Model performance was evaluated using:

- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)

These metrics measure forecasting accuracy by comparing predicted stock prices with actual values.

---

##  Forecast Visualization

The forecasting results were visualized by comparing:

- Actual Closing Prices
- Predicted Closing Prices

This allows visual assessment of model performance over time.

---

##  FinTech Applications

This project demonstrates how distributed machine learning can be applied in:

- Financial Forecasting
- Stock Market Prediction
- Risk Analysis
- Investment Decision Support
- Quantitative Finance

---

##  Skills Demonstrated

- Time-Series Forecasting
- Financial Data Analysis
- Feature Engineering
- Lag Feature Creation
- Rolling Statistics
- Regression Modelling
- PySpark Machine Learning
- Distributed Computing
- FinTech Analytics

---

##  Running the Project

### Install Dependencies

```bash
pip install pyspark
```

### Run the Notebook

1. Open the notebook in Google Colab
2. Install required dependencies
3. Load the Apple Stock dataset
4. Run all notebook cells sequentially
5. Review model evaluation metrics and forecasting results

---

##  Repository Structure

```text
Apple-Stock-Forecasting-PySpark/
│
├── Week9_Group10_Oteri_Oritsejolomisan.ipynb
├── README.md
└── Dataset/
```

---

##  Future Improvements

- Hyperparameter tuning
- Cross-validation for time-series data
- Advanced forecasting models
- LSTM neural networks
- Prophet forecasting
- Real-time stock prediction pipelines

---



This project demonstrates the application of distributed machine learning techniques using PySpark for financial time-series forecasting and stock market prediction.
