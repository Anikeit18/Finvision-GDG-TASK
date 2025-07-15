Here's a **clean, concise, and professional** version of your README without emojis or symbols:

---

# FINVISION

## Overview

FINVISION is a financial analysis toolkit for collecting, analyzing, and modeling stock market data. It includes tasks such as web scraping, statistical analysis, time series testing, and trading strategy implementation using Python and C++.

---

## Part 1: Data Collection and Analysis

### Stock Data Scraping

Scrape Nifty50 stock data from:

* [NSE India](https://www.nseindia.com/)
* [Screener.in](https://www.screener.in/company/)

Extract the following data: PE, EPS, 52-week high/low, circuit limits, LTP, market cap, volume, and percentage change. Convert the results into a DataFrame.

### Historical Returns

Add 6-month, 1-year, and 5-year returns using the Yahoo Finance API. Use Close or Adjusted Close prices for calculation.

---

## Part 2: Statistical Analysis

Calculate and visualize:

* T-Score
* Z-Score
* Confidence Intervals

Apply these to daily volume, close price, and returns using data from Yahoo Finance. Plot relevant probability distributions.

**Bonus:**
Identify two stocks (from 2023–2024 data) that are stationary or non-stationary using the ADF and KPSS tests.

---

## Final Assignment: BTC-USD Strategy Using Stock Span

### Context

Apply the Stock Span concept to BTC-USD to develop a momentum-based strategy. Span represents the number of consecutive days before today with a price less than or equal to today’s.

### Strategy Use-Cases

1. **Momentum Detection:**

   * High span indicates bullish momentum
   * Low span suggests weak price action

2. **Trend Confirmation:**

   * Increasing span with price suggests a strong trend
   * Combine with moving averages

3. **Support/Resistance Detection:**

   * Rising span before resistance indicates strength
   * Falling span after support suggests reversal

4. **Exhaustion Signals:**

   * Constant high span may indicate overbought
   * Prolonged low span may indicate oversold

### Implementation

Use a stack-based O(n) approach to compute stock span for BTC-USD. Implement in Python or C++ using daily data from Yahoo Finance. Plot and analyze the results.

---

## Task 2: Real-Time Support/Resistance System

### Problem Statement

Build a system that:

* Dynamically appends new stock prices
* Efficiently finds local minima (support) and local maxima (resistance)

### Operations

* `"U X"`: Append price X
* `"Q L R"`: Return min price in range \[L, R]
* `"M L R"` (optional): Return max price in range \[L, R]

### Constraints

* 1 ≤ N, Q ≤ 10^5
* 0 ≤ Price ≤ 10^9
* 0 ≤ L ≤ R < current list length

### Approach

Use a segment tree to support:

* O(log N) update and query operations
* Efficient handling of dynamic data

### Assignment

Implement a Range Minimum Query system on BTC-USD data. Use it to identify support/resistance levels and combine with indicators for trading decisions.

---

Let me know if you need it formatted for GitHub or LaTeX, or want code templates included.
