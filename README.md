📊 Trader Performance vs Market Sentiment Analysis

Data Science Intern Assignment – Primetrade.ai

🔎 Project Overview

This project analyzes how Bitcoin market sentiment (Fear/Greed Index) influences trader behavior and performance on Hyperliquid.

The objective is to uncover behavioral patterns and performance differences across sentiment regimes and generate actionable, sentiment-aware trading insights.

🎯 Objectives

Analyze trader profitability during Fear vs Greed market conditions

Identify behavioral shifts in:

Leverage usage

Trade frequency

Position size

Long/Short bias

Segment traders into meaningful groups

Propose actionable trading strategies

(Optional) Build a simple predictive model

📂 Dataset Description
1️⃣ Bitcoin Market Sentiment Dataset

Columns: Date, Classification (Fear / Greed)

Daily sentiment classification

2️⃣ Historical Trader Data (Hyperliquid)

Key fields:

account

symbol

execution price

size

side

time

closedPnL

leverage

event

🛠️ Methodology
1️⃣ Data Cleaning

Removed duplicates

Handled missing values

Converted timestamps to datetime format

Aggregated data at daily level

2️⃣ Data Alignment

Extracted trade dates from timestamps

Merged trader data with sentiment data on daily basis

3️⃣ Feature Engineering

Created key behavioral and performance metrics:

Daily PnL per trader

Win Rate

Average Leverage

Trades per Day

Long/Short Ratio

Trader Segments

High vs Low Leverage

Frequent vs Infrequent Traders

Consistent Winners vs Inconsistent Traders

📊 Exploratory Analysis
✅ Performance vs Sentiment

Compared average PnL on Fear vs Greed days

Compared win rates

Analyzed drawdown proxy

✅ Behavioral Changes

Leverage distribution shifts

Trade frequency variation

Long/Short bias differences

✅ Trader Segmentation

Identified performance differences among:

High vs Low leverage traders

Frequent vs Infrequent traders

Consistent vs Inconsistent traders

📈 Key Insights

Trader profitability differs significantly across sentiment regimes.
Greed days generally show higher average PnL and win rates.

High leverage amplifies losses during Fear periods.
Risk exposure increases vulnerability during negative sentiment.

Frequent traders overtrade during emotional markets.
Trade frequency rises during extreme sentiment phases, impacting stability.

💡 Strategy Recommendations
🔹 Strategy 1 – Dynamic Leverage Adjustment

Reduce leverage during Fear days

Cap leverage during Greed days to prevent overexposure

🔹 Strategy 2 – Sentiment-Aware Trade Filtering

Reduce trade frequency during high-volatility Fear periods

Prioritize high win-rate traders during uncertain sentiment

🤖 (Bonus) Predictive Modeling

Built a simple classification model to predict daily trader profitability using:

Sentiment

Leverage

Win rate

This demonstrates the predictive value of behavioral and sentiment features.

📁 Project Structure
├── data/
│   ├── sentiment.csv
│   └── trader_data.csv
│
├── notebook/
│   └── trader_sentiment_analysis.ipynb
│
├── outputs/
│   ├── charts/
│   └── tables/
│
├── README.md
└── SUMMARY.md

⚙️ How to Run

Clone the repository:

git clone <repo-link>


Install dependencies:

pip install -r requirements.txt


Open and run:

notebook/trader_sentiment_analysis.ipynb

🧠 Skills Demonstrated

Data Cleaning & Preprocessing

Time Series Alignment

Feature Engineering

Behavioral Segmentation

Exploratory Data Analysis

Statistical Comparison

Predictive Modeling

Insight Communication

📌 Conclusion

This analysis demonstrates that market sentiment significantly influences trader behavior and profitability. By incorporating sentiment-aware risk management and behavioral segmentation, trading strategies can be optimized to reduce drawdowns and enhance consistency.
