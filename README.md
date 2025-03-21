# GPT vs Analysts: Financial Forecasting using GPT-4o

## Project Overview

Can AI outperform Wall Street analysts in forecasting corporate earnings?

This project explores that question by evaluating **GPT-4o**, OpenAI’s publicly available model, as a financial forecasting tool. We benchmarked its performance against traditional analysts using **earnings data from Yahoo Finance**, focusing on the **direction of EPS changes** (up/down). 

Our work builds on the framework presented in the UChicago Booth 2024 working paper:  
*“Financial Statement Analysis with Large Language Models”*

## Key Insights

- **GPT-4o demonstrated lower mean errors** and **greater consistency** than analysts in predicting earnings direction.
- It is especially effective in **stable industries** with historical consistency.
- **Limitations** include lack of access to real-time qualitative signals (e.g., CEO calls, market guidance, Fed decisions).
- GPT-4o is best used as a **complementary tool**, not a replacement for analysts.

## Methodology

Our approach included the following steps:

1. **Data Collection**
   - Extracted earnings and financial data from **Yahoo Finance** for a sample of companies.
   - Selected key performance indicators relevant to forecasting EPS direction.

2. **GPT-4o Testing Setup**
   - Used **OpenAI’s free web interface** to query GPT-4o.
   - Designed standardized prompts mimicking analyst-like behavior: trend observation, ratio analysis, and directional prediction.

3. **Evaluation**
   - Compared GPT’s directional EPS predictions against:
     - Historical earnings data (actuals)
     - Analyst forecasts from Yahoo Finance
   - Focused on **accuracy**, **error variance**, and **consistency**.

4. **Interpretation**
   - Analyzed cases where GPT performed better or worse than analysts.
   - Considered market conditions, sector-specific patterns, and prediction volatility.

## Technologies Used

- **Python** (Pandas, Matplotlib) for data prep & analysis  
- **Yahoo Finance** API for data collection  
- **GPT-4o** (via web interface) for model predictions  
- **Jupyter Notebook** for experiment documentation

## Future Improvements

- Integrate **macroeconomic indicators** and **real-time news feeds**
- Explore performance across **volatility-adjusted sectors**
- Benchmark GPT-4o vs **finetuned finance-specific LLMs**

## Reference

Kim, Muhn, Nikolaev (2024)  
📘 *Financial Statement Analysis with Large Language Models* — [BFI WP 2024-65](https://bfi.uchicago.edu/working-paper/2024-65/)

---
This project is intended for academic and educational use only. Not for commercial deployment.

