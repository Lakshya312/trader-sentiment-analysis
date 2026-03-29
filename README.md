# Trader Performance vs Market Sentiment Analysis

## Objective
This project analyzes how market sentiment (Fear/Greed) influences trader behavior and performance using Bitcoin sentiment data and historical trading data.

---

## Methodology

1. **Data Preparation**
   - Cleaned and validated both datasets (no missing values or duplicates).
   - Converted timestamps to datetime format.
   - Aggregated trade-level data to daily account-level metrics.

2. **Feature Engineering**
   - Daily PnL
   - Win Rate
   - Trade Frequency
   - Average Trade Size (leverage proxy)
   - Long/Short Ratio
   - Loss Rate (drawdown proxy)
   - Consistency (win rate variability)

3. **Data Alignment**
   - Merged trader metrics with sentiment data using date-level alignment.

---

## Key Insights

1. **Non-linear performance across sentiment:**  
   Traders achieve high profitability during both **Fear** and **Extreme Greed**, indicating that both volatility and strong trends create opportunities.

2. **Behavior adapts to sentiment:**  
   Traders increase long positions and risk exposure during **Greed**, while adopting more defensive positioning during **Fear**.

3. **Risk-return tradeoff across segments:**  
   High-activity and large-position traders generate higher returns but with greater variability, while consistent traders show more stable outcomes.

---

## Strategy Recommendations

- **Fear Markets:**  
  Use short-term, volatility-driven strategies with controlled risk.

- **Extreme Greed Markets:**  
  Apply trend-following strategies with a long bias.

- **Neutral Markets:**  
  Reduce exposure and trading activity.

---

## How to Run

# 1. Clone the repository
git clone <[Lakshya312](https://github.com/Lakshya312/trader-sentiment-analysis)>

cd <trader_sentiment_analysis>

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn jupyter

# 3. Open and run the notebook
jupyter notebook notebook.ipynb
