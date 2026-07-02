# Task
# Bitcoin Market Sentiment vs Trader Performance Analysis

## Overview

This project analyzes the relationship between Bitcoin market sentiment and trader performance using two datasets:

1. **Fear & Greed Index Dataset**
2. **Historical Trader Data (Hyperliquid)**

The goal is to determine whether market sentiment (Fear, Greed, Extreme Fear, etc.) has any impact on trading performance by analyzing profit/loss, trading activity, and coin-wise performance.

---

## Datasets Used

### 1. fear_greed_index.csv

This dataset contains daily Bitcoin market sentiment.

**Columns**

* timestamp
* value
* classification
* date

### 2. historical_data.csv

This dataset contains historical trading records from Hyperliquid.

Important columns used:

* Account
* Coin
* Execution Price
* Size Tokens
* Size USD
* Side
* Timestamp IST
* Closed PnL
* Fee

---

## Libraries Used

* pandas
* matplotlib
* seaborn

---

# Notebook Structure

The notebook contains **three sections (cells)**.

---

## Part 1 – Data Loading and Preprocessing

### Purpose

The first section prepares the data for analysis.

### Tasks Performed

* Import required libraries.
* Load both CSV datasets.
* Display sample records.
* Convert date columns into datetime format.
* Rename columns for easier processing.
* Merge trader data with market sentiment using the Date column.
* Convert important numerical columns.
* Handle missing values.
* Display dataset statistics.
* Count total trades, profitable trades, and loss-making trades.
* Show top traded coins and buy/sell distribution.

**Output**

* Clean merged dataset ready for analysis.
* Basic statistics and summary of the data.

---

## Part 2 – Exploratory Data Analysis (EDA)

### Purpose

This section visualizes trader behaviour under different market sentiments.

### Analysis Performed

* Average profit/loss by sentiment.
* Market sentiment distribution.
* Profit/Loss boxplot.
* Average trade size by sentiment.
* Buy vs Sell comparison.
* Top traded coins.
* Profit/Loss distribution.
* Execution Price vs Closed PnL scatter plot.

**Output**

* Multiple charts showing trader behaviour.
* Visual comparison between different market sentiments.

---

## Part 3 – Performance Analysis and Insights

### Purpose

This section extracts useful insights from the merged dataset.

### Analysis Performed

* Win rate by sentiment.
* Total profit/loss by sentiment.
* Top profitable coins.
* Top loss-making coins.
* Average profit during Fear and Greed.
* Overall net profit/loss.
* Average trade size.
* Average execution price.
* Export merged dataset as `merged_analysis.csv`.

**Output**

* Final business insights.
* Coin-wise profitability.
* Overall trader performance summary.

---

# Key Findings

* Compared trader performance across different market sentiments.
* Identified the most profitable trading coins.
* Calculated win rates for each market sentiment.
* Compared Buy and Sell trading performance.
* Generated visual insights using charts.
* Produced a merged dataset for further analysis.

---

# Files Included

* analysis.ipynb
* fear_greed_index.csv
* historical_data.csv
* merged_analysis.csv
* README.md

---

# How to Run

1. Install required libraries.

```
pip install pandas matplotlib seaborn
```

2. Place both CSV files in the same folder as the notebook.

3. Open the Jupyter Notebook.

4. Run all three cells in order:

   * Part 1
   * Part 2
   * Part 3

---

# Conclusion

This project successfully combines Bitcoin market sentiment data with historical trading records to analyze trader performance. Using data preprocessing, exploratory data analysis, and performance metrics, the project provides insights into trading behaviour, profitability, and market trends that can support better trading decisions.
