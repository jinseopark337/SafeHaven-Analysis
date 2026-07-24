# SafeHaven-Analysis
Python-based financial data analysis on safe-haven assets during geopolitical risks.

# Overview

This project analyzes the behavior of traditional safe-haven assets during geopolitical risks using Python and financial market data.

The objective is to examine whether assets such as Gold, the U.S. Dollar Index, and U.S. Treasury Bonds consistently function as safe havens under different geopolitical events.

# Motivation

While studying economics and participating in an economic news discussion group, I became interested in how geopolitical risks influence financial markets.

Rather than relying on common assumptions, I wanted to verify the behavior of safe-haven assets using real financial data.

# Research Question

- Does Gold always act as a safe-haven asset?
- How do different geopolitical risks affect asset behavior?
- Are descriptive statistics sufficient to explain safe-haven characteristics?

 
# Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Statsmodels
- yfinance


# Methodology

1. Financial data collection
2. Data preprocessing
3. Return analysis
4. Volatility analysis
5. Correlation analysis
6. Value at Risk (VaR)
7. Regression analysis

# Data

- Gold Futures: GC=F
- U.S. Dollar Index: DX-Y.NYB
- U.S. Treasury indicator: ^TNX
- Market uncertainty indicator: ^VIX
- Events: Russia–Ukraine War, U.S.–Middle East geopolitical conflict
- Source: Yahoo Finance via yfinance

# Visualization example
<img width="4800" height="3600" alt="A_comprehensive_analysis" src="https://github.com/user-attachments/assets/da6bac37-1585-48d8-942a-f16f262c00a6" />


# Results

The first-stage analysis compared Gold, the U.S. Dollar Index,
U.S. Treasury-related indicators, and market volatility across
geopolitical risk periods.

The results showed that safe-haven performance was not consistent
across assets or events. Return, volatility, correlation, VaR, and
regression results produced different evaluations depending on the
asset and event period.

This suggests that safe-haven characteristics cannot be determined
using a single descriptive statistic alone.

This finding motivated the design of a second-stage research project.

# Future Work

The second-stage project expands the analysis by reviewing academic literature and refining the research framework to better explain safe-haven behavior under different geopolitical conditions.
