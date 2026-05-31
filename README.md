# GROUP-14-PROJECT

# Stock Market Analysis and Prediction Using Machine Learning and Transfer Learning
---
## Project Overview

This project is about the analysis and prediction of stock market prices using Machine Learning, Deep Learning and Transfer Learning techniques.

Historical stock market data from selected companies listed on the London Stock Exchange (LSE) is combined with UK macroeconomic indicators to develop predictive models that can forecast future stock prices.

The project evaluates the performance of multiple forecasting methods and provides an interactive Streamlit dashboard where users can visualise stock trends and prediction results.

---
## Research Question

> How effectively can machine learning, hybrid deep learning, and transfer learning models predict stock market prices using historical stock market and macroeconomic datasets?

---

## Project Objectives

- Collect and preprocess historical stock market and macroeconomic datasets.
- Perform data cleaning and feature engineering.
- Generate technical indicators such as:
  - SMA
  - EMA
  - RSI
  - MACD
- Develop and compare:
  - LSTM Neural Network
  - CNN-LSTM Hybrid Model
  - Transfer Learning Model
- Optimise model performance through hyperparameter tuning.
- Evaluate models using industry-standard performance metrics.
- Deploy an interactive Streamlit dashboard.

---
## Datasets

### Historical Stock Market Dataset

**Source:** Yahoo Finance
**Selected LSE Companies**

| **Ticker** | BP.L | SHEL.L | TSCO.L | ULVR.L | BLND.L | LAND.L | SGE.L | CCC.L | AZN.L | GSK.L |
|------------|---------|-----------|-----------|--------------|--------------|-----------------|------------|------------|------------|----------|
| **Company** | BP plc | Shell plc | Tesco plc | Unilever plc | British Land | Land Securities | Sage Group | Computacenter | AstraZeneca | GSK plc |

### Features

- Date
- Open Price
- High Price
- Low Price
- Close Price
- Adjusted Close Price
- Trading Volume
- Stock Ticker

---

### UK Macroeconomic Dataset

**Sources**

- Yahoo Finance
- FRED (Federal Reserve Economic Data)

**Features**

- Inflation Rate
- Interest Rate
- GDP Growth
- Unemployment Rate
- Exchange Rate
- CPI
- FTSE100 Index

---

## Project Pipeline

```text
Historical Stock Data + Macroeconomic Data
                    │
      Data Collection & Integration
                    │
     Data Cleaning & Preprocessing
                    │
          Feature Engineering
                    │
          Data Normalisation
                    │
             Train/Test Split
                    │
     ┌──────────────────────────┐
     │      Model Training      │
     ├──────────────────────────┤
     │ • LSTM                   │
     │ • CNN-LSTM               │
     │ • Transfer Learning      │
     └──────────────────────────┘
                    │
       Hyperparameter Tuning
                    │
          Model Evaluation
                    │
         Prediction Comparison
                    │
        Streamlit Web Dashboard
```

---


