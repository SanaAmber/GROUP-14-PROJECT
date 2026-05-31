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
              Web Dashboard
```

---

## Feature Engineering

| Feature | Purpose |
|----------|----------|
| SMA | Trend Identification |
| EMA | Trend Smoothing |
| RSI | Momentum Measurement |
| MACD | Trend and Momentum Analysis |
| Daily Returns | Price Movement Analysis |
| Volatility | Risk Measurement |

---

## Models Implemented

### 1. LSTM Neural Network

Long Short-Term Memory networks designed for time-series forecasting and sequential learning.

### 2. CNN-LSTM Hybrid Model

Combines CNN layers for feature extraction with LSTM layers for temporal learning.

### 3. Transfer Learning Model

Leverages pre-trained forecasting architectures to improve generalisation and reduce training complexity.

### 4. Benchmark Model

- XGBoost Regressor

Used as a benchmark against deep learning approaches.

---

## Evaluation Metrics

| Metric | Description |
|----------|----------|
| RMSE | Root Mean Squared Error |
| MAE | Mean Absolute Error |
| R² Score | Coefficient of Determination |
| Accuracy | Forecasting Accuracy |

### KPI Targets

| KPI | Target |
|------|--------|
| RMSE | Minimise |
| MAE | < 5% |
| R² Score | > 0.85 |
| Prediction Accuracy | > 80% |
| Response Time | < 3 Seconds |

---

## Technology Stack

### Languages

- Python

### Data Processing

- Pandas
- NumPy

### Visualisation

- Matplotlib
- Seaborn
- Plotly

### Machine Learning

- Scikit-Learn
- TensorFlow
- Keras
- XGBoost

### Deployment

- Streamlit

### Version Control

- Git
- GitHub

---

## Repository Structure

```text
stock-market-prediction/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│
├── src/
│   ├── preprocessing/
│   ├── feature_engineering/
│   ├── models/
│   ├── evaluation/
│   └── utils/
│
├── streamlit_app/
│
├── tests/
│
├── docs/
│
├── requirements.txt
├── README.md
└── .gitignore
```

---

## Installation

```bash
git clone https://github.com/your-team/stock-market-prediction.git

cd stock-market-prediction
```

Create a virtual environment:

```bash
python -m venv venv
```

Activate environment:

### Windows

```bash
venv\Scripts\activate
```

### Mac/Linux

```bash
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Running the Project

### Train Model

```bash
python src/models/train_lstm.py
```

### Evaluate Models

```bash
python src/evaluation/evaluate_models.py
```

### Launch Dashboard

```bash
streamlit run streamlit_app/app.py
```

---

## Testing

Run all tests:

```bash
pytest
```

Testing includes:

- Data Validation Testing
- Unit Testing
- Model Evaluation Testing
- User Acceptance Testing (UAT)

---

## Team Members

| Name | Role |
|--------|--------|
| Akash Govardhane | Team Leader |
| Sana Amber | GitHub Document Manager |
| Laxmi Gurrala | Scrum Master |
| Abimbola Olasupo | Communications Leader |
| Muhammad Azeem | Test Plan Manager |
| Zafar Iftikhar | Code Review Manager |

---

## Project Timeline

| Phase | Week |
|---------|---------|
| Planning & Dataset Collection | Week 1 |
| Data Cleaning & EDA | Week 2 |
| Feature Engineering | Week 3 |
| LSTM Development | Week 4 |
| CNN-LSTM Development | Week 5 |
| Transfer Learning Model | Week 6 |
| Hyperparameter Tuning | Week 7 |
| Model Evaluation | Week 8 |
| Streamlit Dashboard | Week 9 |
| Testing & UAT | Week 10 |
| Documentation | Week 11 |
| Final Submission | Week 12 |

---

## Ethical Considerations

- No personal data is collected.
- No GDPR-sensitive data is used.
- All datasets are publicly available.
- The project complies with academic research standards.

---

## Disclaimer

This project is intended for academic and educational purposes only.

The predictions generated by this system should **not** be considered financial or investment advice.
