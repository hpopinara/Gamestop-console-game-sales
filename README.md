# Gamestop-console-game-sales

## Overview
This repository contains a **synthetic dataset** estimating the annual sales of gaming consoles and physical video games for GameStop, broken down by U.S. state. As this specific sales data is not publicly released by GameStop, this dataset was programmatically generated using real-world demographic and interest-based proxies to ensure realism and logical consistency.

## 🎯 Motivation
The goal is to create a plausible dataset to analyze:
- Which states are the largest markets for GameStop?
- What is the relationship between console sales and game sales?
- Which states are the most profitable based on typical retail margins?

## 📊 Data Sources & Synthesis Methodology
The synthetic data is built upon a foundation of real, publicly available data:
1.  **U.S. Census Data:** State population and median household income.
2.  **GameStop Location Data:** Estimated number of retail stores per state.
3.  **Google Trends Data:** Relative search interest for "PS5" by state (a proxy for consumer demand).
4.  **Industry Reports:** Common industry metrics like average console and game prices, and typical profit margins.

A Python script was used to combine these factors and generate the final sales figures. The code for this generation is included in the `generate_data.py` file.

## 📁 Dataset: `synthetic_gamestop_sales.csv`

| Column | Description |
| :--- | :--- |
| `State` | The U.S. state or district. |
| `Total_Consoles_Sold` | Estimated annual units of all consoles sold (PS5, Xbox Series X/S, Switch). |
| `Total_Physical_Games_Sold` | Estimated annual units of physical game software sold. |
| `Total_Revenue` | Estimated total revenue (in USD) from consoles and games. |
| `Avg_Games_Per_Console` | The average number of games sold per console in that state. |
| `Profit_Margin` | The estimated weighted average profit margin for revenue in that state. |

## 🔍 Example Insights
- **Top 5 States by Console Sales:** California, Texas, Florida, New York, Illinois.
- **Highest Games-Per-Console Ratio:** States with higher median income tend to have a slightly higher attach rate.
- **Most Profitable States:** While California generates the most revenue, states with a higher proportion of game sales (which have better margins) can be more profitable per dollar.

## ⚠️ Important Disclaimer
**This is not official GameStop data.** This is a synthetic dataset created for educational purposes, portfolio projects, and data analysis practice. The numbers are estimates based on public proxies and should not be used for financial or business decisions.

## 🛠 How to Use
1.  Clone the repo.
2.  Run `generate_data.py` to recreate the dataset with optional random seeds.
3.  Analyze the `synthetic_gamestop_sales.csv` file using Pandas, Tableau, Excel, etc.

## Conclusion and key findings
Based on the analysis of this synthetic dataset, we can draw several compelling conclusions about the hypothetical state-level performance of GameStop's console and physical game sales:

1. Market Dominance is Concentrated in Populous States:
The top 5 states by revenue—California, Texas, Florida, New York, and Pennsylvania—account for a disproportionately large share of total national sales. This aligns perfectly with their high populations and number of retail locations, confirming that market size is the primary driver of sales volume.

2. The "Attachment Rate" is Key to Profitability:
While console sales drive total revenue, the number of physical games sold per console (Avg_Games_Per_Console) is the strongest indicator of profitability. States like Rhode Island, Massachusetts, and Utah (with attachment rates of 7.8+) consistently show a profit margin of 0.22, compared to the national average of ~0.21. This highlights the critical importance of selling high-margin software and accessories with each console.

3. Revenue Does Not Always Equal Efficiency:
A state like Florida is a top contributor by total revenue but has a lower-than-average attachment rate (7.04) and profit margin (0.20). This suggests that while Florida generates massive sales volume, its customers may be purchasing fewer games per console on average, making it a slightly less efficient market compared to smaller states with higher attachment rates.

4. Regional Strategies Could Be Applied:
This data suggests a one-size-fits-all national strategy is not optimal. Commercial initiatives could be tailored by state:

High-Volume, Lower-Attachment States (e.g., Florida, Ohio): Focus marketing on game pre-orders, season passes, and special editions at the point of console sale to boost the attachment rate.

High-Attachment States (e.g., Northeast, Utah): These are already healthy markets. Strategies could focus on customer loyalty and selling collector's items or higher-margin peripherals.

Lower-Volume States: Focus on lean operations and targeted local marketing to capture a larger share of a smaller market.

Final Summary: This analysis underscores that for a retailer like GameStop, maximizing software sales is even more important than selling hardware. The most successful markets are not just those that sell the most consoles, but those that most effectively capitalize on each console sale with high-margin physical game sales.

