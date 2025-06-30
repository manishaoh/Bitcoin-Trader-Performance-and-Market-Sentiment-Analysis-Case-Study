# Bitcoin-Trader-Performance-and-Market-Sentiment-Analysis-Case-Study

Explored the relationship between trader performance and market sentiment using two datasets: historical trader data from Hyperliquid and the Bitcoin Fear/Greed Index.

## 📌 Objective

- Investigate how Bitcoin market sentiment (Fear/Greed) impacts trader performance.
- Analyze trading behavior patterns across different sentiment phases.
- Build predictive models to forecast trade profitability based on market sentiment and trader metrics.
- Deliver actionable insights to design smarter trading strategies.

## 🗂️ Datasets

- **Bitcoin Market Sentiment Dataset**  
  Columns: `Date`, `Classification` (Extreme Fear, Fear, Neutral, Greed, Extreme Greed)

- **Historical Trader Data from Hyperliquid**  
  Columns include: `account`, `symbol`, `execution price`, `size`, `side`, `time`, `start position`, `event`, `closedPnL`, `leverage`, and more.

## 📝 Analysis Overview

- **Exploratory Data Analysis (EDA)**  
  - Rolling PnL volatility by sentiment
  - Average net daily PnL, trade volume, and buy/sell ratios across sentiments
  - Trade frequency distributions by sentiment
  - Buy direction biases

- **Predictive Modeling**  
  - Logistic Regression, Random Forest, XGBoost , LightGBM classifiers were trained to predict trade profitability.
  - LightGBM delivered the best performance (89% accuracy).

- **Key Insights**
  - Fear periods correlate with higher trading frequency but poorer overall performance.
  - Extreme Fear drives highly polarized buy/sell behaviors and erratic volatility.
  - Greed phases support more disciplined trading with better average profitability.
  - Sentiment classification is a strong predictor of trade outcomes.

- **Recommendations**
  - Implement dynamic risk management strategies based on real-time sentiment signals.
  - Reduce leverage and trading frequency during Fear/Extreme Fear to avoid unnecessary losses.
  - Integrate sentiment-based entry/exit rules to capitalize on more stable Greed phases.

## 🖼️ Visuals

The notebook generates charts and heatmaps illustrating:
- Rolling 3-day PnL standard deviations by sentiment
- Average trader metrics across sentiments
- Distribution of trades per day by sentiment
- Buy direction biases under different market conditions



