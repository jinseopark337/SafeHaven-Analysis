# SafeHaven-Analysis

Python-based financial data analysis on safe-haven assets during geopolitical risks.

# Overview

This project analyzes the behavior of traditional safe-haven assets during geopolitical risks using Python and financial market data.

The objective is to examine whether assets such as Gold, the U.S. Dollar Index, and U.S. Treasury Bonds consistently function as safe havens across different geopolitical events.

The analysis compares two geopolitical events:

- Russia–Ukraine War
- U.S.–Iran Conflict

# Motivation

While studying economics and participating in an economic newspaper study group, I encountered an article discussing how Gold had not fully performed its traditional role as a safe-haven asset during a period of geopolitical uncertainty.

This raised a question: does Gold actually function as a safe haven across different geopolitical events?

Rather than relying on the conventional assumption that Gold is always a safe haven, I wanted to examine its behavior directly using financial market data.

The analysis was later expanded to compare Gold with the U.S. Dollar and U.S. Treasury bonds.

# Research Questions

- Does Gold always act as a safe-haven asset?
- Do safe-haven assets behave differently across geopolitical events?
- Can safe-haven characteristics be explained by returns alone?

# Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Statsmodels
- yfinance

# Data

### Safe-Haven Candidates

- Gold Futures: `GC=F`
- U.S. Dollar Index: `DX-Y.NYB`
- U.S. Treasury Bond ETF: `IEF`

### Benchmark & Control Variables

- S&P 500: `^GSPC`
- U.S. 10-Year Treasury Yield: `^TNX`
- VIX: `^VIX`

### Events

- Russia–Ukraine War: February 24, 2022
- U.S.–Iran Conflict: February 28, 2026

Source: Yahoo Finance via `yfinance`

# Methodology

1. Financial data collection and preprocessing
2. Daily log-return calculation
3. Return and volatility analysis
4. Pre/Post-event correlation analysis
5. Correlation with the S&P 500
6. Value at Risk (VaR)
7. Regression analysis

# Analysis Update

The initial version of this project focused mainly on comparing Gold, DXY, U.S. Treasury yields, and VIX before and after geopolitical events.

After reviewing the analysis, several parts of the framework were revised:

- `^TNX`, which represents the U.S. 10-year Treasury yield, was separated from the safe-haven assets and used as an interest-rate control variable.
- `IEF`, a U.S. Treasury bond ETF, was added to measure Treasury bond investment performance.
- The S&P 500 was added as a risk-asset benchmark to evaluate whether safe-haven candidates provided diversification during periods of market stress.
- Asset returns were standardized using daily log returns.
- The event-period specification was adjusted to reduce the potential influence of information already reflected in prices immediately before each event.
- Earlier versions of the analysis were replaced by the revised specification.

# Visualization Examples

### Russia–Ukraine War

<!-- Add Russia–Ukraine visualization here -->

### U.S.–Iran Conflict

<!-- Add U.S.–Iran visualization here -->

### Cross-Event Comparison

<!-- Add comparison visualization here -->

# Results

The analysis showed that safe-haven behavior was not consistent across assets or geopolitical events.

In both events, the U.S. Dollar Index showed a negative post-event correlation with the S&P 500, while Gold and U.S. Treasury bonds displayed less consistent patterns.

The results also differed depending on the evaluation metric. An asset showing diversification benefits did not necessarily exhibit lower volatility or downside risk.

Regression results further indicated that the geopolitical event dummy itself was not statistically significant at the conventional 5% level. Therefore, the observed asset movements cannot be attributed solely to the geopolitical events.

These findings suggest that safe-haven characteristics should not be evaluated using a single indicator or by assuming that a particular asset always functions as a safe haven.

# Limitations

This is an exploratory first-stage analysis.

- Only two geopolitical events are examined.
- Pre/Post comparisons may capture other macroeconomic changes occurring during the same period.
- Correlation does not establish causality.
- Interest rates and market uncertainty may affect safe-haven performance.

These limitations motivated a more structured second-stage research project.

# Future Work

The second-stage project expands the analysis by reviewing academic literature and refining the research framework.

Current hypotheses include:

- **H1:** Safe-haven assets may differ depending on the type of geopolitical risk.
- **H2:** Gold alone may be insufficient to explain recent safe-haven behavior.
- **H3:** Comparing Gold, DXY, and U.S. Treasury bonds may provide a more comprehensive framework for evaluating safe-haven assets.

Future analysis will focus on:

- shorter event windows,
- additional geopolitical events,
- robustness checks across different event windows,
- macroeconomic control variables,
- and classification of geopolitical risk types.
