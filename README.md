# Trader Performance vs Market Sentiment Analysis

## Author

**Naman Mankar**

---

# Project Overview

This project analyzes the relationship between **market sentiment (Fear vs Greed)** and **trader behavior and performance** using trading data from Hyperliquid.

The goal is to understand how trader profitability, trade size, and trading activity change based on market sentiment. The findings help propose **data-driven trading strategies** and **risk management rules**.

---

# Objective

The analysis focuses on answering the following questions:

1. Does trader performance (PnL) change between **Fear** and **Greed** market conditions?
2. Do traders modify their behavior depending on sentiment?
3. Can traders be segmented based on behavior patterns?
4. What actionable strategies can be derived from the insights?

---

# Datasets Used

## 1. Bitcoin Market Sentiment Dataset

Contains daily sentiment classification.

Columns include:

* timestamp
* value
* classification (Fear / Greed)
* date

## 2. Historical Trader Data (Hyperliquid)

Contains trader activity data.

Important columns:

* Account
* Coin
* Execution Price
* Size Tokens
* Size USD
* Side
* Timestamp IST
* Closed PnL
* Fee
* Trade ID

---


# Installation

Clone the repository:

```
git clone https://github.com/yourusername/trader-sentiment-analysis.git
cd trader-sentiment-analysis
```

Install required libraries:

```
pip install -r requirements.txt
```

---

# Requirements

The project uses the following Python libraries:

```
pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter
```

Install them using:

```
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

---

# How to Run the Project

Step 1 — Download the datasets and place them inside the **data/** folder.

Step 2 — Open Jupyter Notebook.

```
jupyter notebook
```

Step 3 — Open the notebook file:

```
notebook/trader_sentiment_analysis.ipynb
```

Step 4 — Run all cells sequentially.

The notebook will:

* Clean the datasets
* Merge trader data with sentiment data
* Create new analytical features
* Generate charts and insights

Charts will be saved automatically inside the **output/** folder.

---

# Data Processing Steps

1. **Data Cleaning**

   * Missing value inspection
   * Duplicate removal
   * Timestamp conversion

2. **Dataset Alignment**

   * Converted timestamps to daily dates
   * Merged trader dataset with sentiment dataset

3. **Feature Engineering**

   * Daily PnL
   * Win rate
   * Trade frequency
   * Average trade size

---

# Analysis Performed

## 1. Trader Profitability vs Sentiment

We analyzed how **Closed PnL varies during Fear and Greed periods**.

Visualization:

* Bar chart of PnL by sentiment

---

## 2. Trade Size Behavior

We examined whether traders place larger trades during certain sentiment conditions.

Visualization:

* Boxplot of trade size distribution

---

## 3. Trading Activity

We evaluated changes in trading frequency across sentiment conditions.

Visualization:

* Line chart showing trades per day

---

# Trader Segmentation

Traders were segmented into behavioral groups:

### Frequent vs Infrequent Traders

Based on total number of trades.

### High vs Low Trade Size

Based on median trade size.

These segments help identify behavioral patterns among traders.

---

# Key Insights

1. Traders tend to place **larger trades during Greed periods**, indicating higher risk appetite.

2. Market **Fear periods often show lower profitability and higher volatility**.

3. **Frequent traders generate higher cumulative profits** compared to occasional traders.

---

# Strategy Recommendations

Based on the analysis, the following trading rules can be suggested:

### Strategy 1 — Risk Control During Fear

* Reduce trade size
* Avoid excessive leverage
* Focus on capital preservation

### Strategy 2 — Opportunistic Trading During Greed

* Increase trade frequency moderately
* Allow larger position sizes with controlled risk

---

# Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

---

# Future Improvements

Potential extensions of this project include:

* Building a **predictive model** to forecast trader profitability
* **Clustering traders** into behavioral archetypes
* Developing an **interactive dashboard using Streamlit**

---

# Conclusion

This analysis demonstrates that **market sentiment significantly influences trader behavior and performance**. Understanding these patterns can help traders and platforms design **more effective trading strategies and risk management systems**.

---

