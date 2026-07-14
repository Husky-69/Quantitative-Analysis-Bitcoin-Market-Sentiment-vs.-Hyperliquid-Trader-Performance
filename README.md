# Quantitative Analysis: Bitcoin Market Sentiment vs. Trader Performance

## Project Overview
This project is a complete data science pipeline built in a Python Jupyter Notebook. It investigates the behavioral and financial relationships between market-wide Bitcoin sentiment (the Fear & Greed Index) and individual retail trader metrics derived from Hyperliquid historical data.

The goal of this analysis is to uncover hidden behavioral patterns and formulate actionable quantitative trading strategies based on historical win rates, daily profit and loss (PnL), and trading volume.

---

## Features
This notebook is broken down into a robust, professional data science workflow:
* **Step 1 & 2: Data Cleaning & Time Alignment:** Standardizes column names, handles missing values, and aligns timestamp data to UTC daily intervals for accurate merging.
* **Step 3: Feature Engineering:** Aggregates transactional telemetry into daily performance metrics (Total PnL, Total Volume, Trade Frequency, and Win Rate).
* **Step 4: Data Merging:** Synchronizes the trader performance dataset with the daily Bitcoin market sentiment dataset.
* **Step 5: Exploratory Data Analysis (EDA):** Generates high-fidelity visual distributions (Time Series, Boxplots, Scatter Plots, and Heatmaps) using Matplotlib and Seaborn.
* **Step 6: Advanced Statistical Analysis & Machine Learning:** 
  * Executes a One-Way ANOVA test to determine the statistical significance of PnL variance across different sentiment regimes.
  * Implements a Random Forest Classifier (with balanced class weights and probability thresholding) to predict next-day profitability.
* **Step 7: Actionable Insights:** Translates the quantitative findings into concrete trading rules.

---

## Prerequisites
To run this notebook, you will need Python installed on your machine along with several core data science libraries. 

You can install the required dependencies using `pip`:

```bash
pip install pandas numpy matplotlib seaborn scipy scikit-learn
