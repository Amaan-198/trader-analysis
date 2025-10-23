# Trader Behavior & Market Sentiment Analysis

This is my submission for the Junior Data Scientist assignment. The objective is to "explore the relationship between trader performance and market sentiment, uncover hidden patterns, and deliver insights that can drive smarter trading strategies".

The final, cleaned notebook is `Analysis1.ipynb`.

## Key Findings

After cleaning and merging the two datasets, my analysis uncovered several key patterns:

### 1. "Smart Money" vs. "Dumb Money"
The most significant "hidden pattern" emerged when separating the top 10% of traders ("Smart Money") from the bottom 10% ("Dumb Money"):
* **During "Extreme Fear,"** the Bottom 10% of traders panic-sell at a loss (a **0.63 Profit Factor**).
* The "Smart Money" traders are on the other side of this trade, buying the dip and achieving a massive **12.60 Profit Factor**.

### 2. "Panic Trading" is Real
Trader behavior changes wildly with sentiment. During periods of "Extreme Fear," traders are frantic:
* **Extreme Fear:** 1,521 trades per day
* **Greed (Calm):** 247 trades per day

This "panic trading" directly correlates with the worst performance, proving that emotional, high-frequency trading is a losing strategy for the average trader.

## The Final "Smarter Trading Strategy"

The ultimate insight from the data is that **there is no single "one-size-fits-all" strategy.** The best strategy is coin-specific.

The final heatmap visualization proves this:
1.  **ETH Strategy:** The best strategy is to "buy the dip." It is most profitable during **Extreme Fear** (241x Profit Factor) but is a *losing* strategy during **Extreme Greed** (0.66x Profit Factor).
2.  **HYPE Strategy:** This is a "take profits" coin. It's wildly profitable during **Extreme Greed** (120x Profit Factor).
3.  **BTC Strategy:** This coin is the most stable. Its *worst* performing time is during **Extreme Fear** (1.24x Profit Factor).

The "smartest strategy" is to identify these unique "Coin + Sentiment" profiles and trade them accordingly.

## Visualizations
The notebook `Analysis1.ipynb` contains all supporting visualizations, including:
* Average Trade Size vs. Sentiment
* Overall Profit Factor vs. Sentiment
* "Panic Trading" Frequency
* "Smart Money" vs. "Dumb Money" Performance
* The final **Coin vs. Sentiment Profit Factor Heatmap**
