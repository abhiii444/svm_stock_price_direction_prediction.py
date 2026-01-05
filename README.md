# svm_stock_price_direction_prediction.py
This Python program implements a Support Vector Machine (SVM) model to predict the direction of stock prices using historical market data. It uses technical indicators derived from Open, High, Low, and Close prices to classify whether the next day’s stock price will rise or fall. 

# Stock Price Direction Prediction Using SVM

This project uses **Support Vector Machine (SVM)** to predict the **next-day stock price direction** based on historical stock data.  
It also evaluates a simple **trading strategy** by comparing cumulative market returns with strategy returns.

---

##  Project Overview

The model predicts whether the **closing price of a stock will increase or decrease the next day** using two technical indicators:
- Open–Close
- High–Low

Multiple SVM kernels are tested to compare accuracy:
- Linear
- Polynomial
- RBF
- Sigmoid

---

##  Dataset

- Stock price data (CSV format)
- Example used: **RELIANCE.csv**
- Required columns:
  - Date
  - Open
  - High
  - Low
  - Close

---

##  Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

---

##  Model Details

- **Algorithm:** Support Vector Classifier (SVC)
- **Train-Test Split:** 80% training, 20% testing
- **Target Variable:**  
  - `1` → Next day closing price increases  
  - `0` → Next day closing price decreases

---

##  Features Created

- `Open-Close` = Open price − Close price  
- `High-Low` = High price − Low price  

---

##  Strategy Evaluation

- Predicts daily trading signals
- Calculates:
  - Daily returns
  - Strategy returns
  - Cumulative returns
- Visual comparison between:
  - Market returns
  - Strategy returns

---

##  Output Visualization

- Line plot comparing:
  - Cumulative market returns
  - Cumulative strategy returns

---

##  How to Run

1. Clone the repository
2. Install required libraries:
   ```bash
   pip install pandas numpy scikit-learn matplotlib
3. Update the dataset path in the code
4. Run the script:
   ```bash
   python stock_price_direction_prediction_svm.py

---

## Future Improvements

- Add more technical indicators
- Hyperparameter tuning
- Cross-validation
- Backtesting on multiple stocks


