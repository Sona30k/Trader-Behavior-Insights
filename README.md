# Trader-Behavior-Insights

# 📊 Market Sentiment vs. Trader Performance Analysis

This project investigates how **Bitcoin market sentiment**—as measured by the Fear & Greed Index—impacts **trader performance and behavior**. It combines sentiment data with real historical trade data to derive insights that can improve trading strategy design.

---

## 📁 Dataset Overview

### 1. Fear & Greed Index (`fear_greed_index.csv`)
- **Columns**: `timestamp`, `value`, `classification`, `date`
- Describes market sentiment per day (`Fear`, `Greed`, etc.)

### 2. Historical Trader Data (`historical-data-2025-06-28.csv`)
- **Columns**: 
  - Trade-level: `Account`, `Coin`, `Execution Price`, `Size USD`, `Side`, `Timestamp`, etc.
  - Outcome: `Closed PnL`, `Direction`, `Fee`, etc.
- Contains over 96,000 trades

---

## ⚙️ How It Works

1. **Timestamp Alignment**: Converts Unix timestamps in the trade data and maps them to the corresponding market sentiment date.
2. **Data Merging**: Joins trades with the sentiment dataset using daily timestamps.
3. **Analysis Performed**:
   - Mean and total PnL under each sentiment class
   - Average trade size by sentiment
   - Trade direction frequency distribution (e.g., `Buy`, `Sell`, `Close Long`)
4. **Optional Visualization**: (Coming soon)
   - PnL distribution plots
   - Trade volume vs. sentiment
   - Direction heatmaps

---

## 📈 Sample Output

- Highest total PnL observed during **Fear** and **Greed** days.
- **Extreme Greed** and **Neutral** periods show **negative average PnL**.
- Significant changes in trade **directional strategies** (e.g., more `Sell` during `Fear`).

---


