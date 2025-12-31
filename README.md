# Trader Behavior vs Market Sentiment

## Objective
This project analyzes how Bitcoin market sentiment (Fear vs Greed) influences trader behavior and performance using historical trading data and the Bitcoin Fear & Greed Index.

The goal is to understand whether market sentiment affects profitability, consistency of outcomes, and risk exposure, and to extract behavioral insights that can inform trading strategy design.

---

## Datasets Used
- Historical trader execution data (Hyperliquid trades)
- Bitcoin Fear & Greed Index (daily sentiment classification)

---

## Methodology
1. Cleaned and aligned trade and sentiment datasets at daily granularity.
2. Merged market sentiment with individual trades based on execution date.
3. Evaluated trader performance using:
   - Average and median closed PnL
   - Win rate (profitability consistency)
4. Analyzed risk exposure using trade size (USD) as a proxy due to lack of leverage data.
5. Visualized profitability distribution and win rates across sentiment regimes.

---

## Key Findings
- Greed periods exhibit higher average profitability, but median trade returns remain zero across both Fear and Greed regimes.
- Win rates remain below 50% in both regimes, indicating low consistency of individual trade outcomes.
- Fear periods are associated with higher average and median trade sizes, suggesting greater capital deployment per trade.
- Greed-driven profitability is achieved despite smaller trade sizes, implying reliance on favorable market movements and occasional outsized wins rather than consistent decision-making.

---

## Business Implications
- Trading strategies should be sentiment-aware but avoid scaling position sizes purely during Greed phases.
- Risk management is especially important during Fear periods due to higher capital exposure per trade.

---

## Limitations
- Market sentiment data is available only at daily granularity.
- Leverage information is not available; trade size is used as a proxy for risk exposure.
- Results indicate association, not causation.

---

## Reproducibility
The analysis is fully reproducible.  
Open the notebook and run **Kernel → Restart & Run All** to regenerate all results.

---

## Author
Parth Kharad
