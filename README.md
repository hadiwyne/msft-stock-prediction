## Stock Prediction Notebook

This repository contains a Jupyter notebook (`Stock_Prediction.ipynb`) that explores a simple machine learning approach for predicting stock price movement, with a focus on risk-free investment only when the price goes up, using historical market data of Microsoft's stock.

---

### Overview

* **Goal**: Build and evaluate a baseline model to predict whether a stock’s price will go up or down on the next day.
* **Approach**:

  1. Load and preprocess historical price and volume data.
  2. Engineer basic predictors.
  3. Split data into train/test sets.
  4. Train a Random Forest classifier.
  5. Evaluate performance using precision.

---

### Dependencies

* Python 3.7+
* yfinance
* pandas
* numpy
* scikit-learn
* matplotlib
* jupyter

*(See `requirements.txt`)*

---


### Results

After training on the default split, the Random Forest model achieves a precision of approximately **52%** on the test set. You can find detailed metric outputs an the tweaking that I performed to push the precision to **58%** in the notebook.

---

### Customization

* **Data**: Replace the CSV file paths in the data-loading section to use your own historical price data.
* **Features**: Feel free to add more technical indicators or external signals.
* **Model Parameters**: Tweak hyperparameters of `RandomForestClassifier` in the notebook to see how performance changes.

---
