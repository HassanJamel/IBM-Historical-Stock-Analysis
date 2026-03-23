<p align="center">
  <a href="https://www.kaggle.com/code/hassanjameelahmed/ibm-historical-stock-analysis-2000-2026" target="_blank">
    <img src="2005.png" alt="IBM" alt="IBM" width="500">
  </a>
</p>
<br>

# IBM Stock Market Dataset (2000-2026) - Project Documentation (PRD)

## a. Project Name & Description

**Project Name:** IBM Stock Price Historical Data (2000-2026) | Daily Financial Analysis
**Project Description:** This project provides a comprehensive daily historical dataset of International Business Machines Corp. (IBM) stock prices from January 2000 to January 2026. This dataset is designed for financial analysts, data scientists, and machine learning enthusiasts to perform exploratory data analysis, time-series forecasting, and algorithmic trading strategy development.

---

## b. Kaggle Dataset Information

### Columns & Details

| Column     | Type    | Description                                                           |
| :--------- | :------ | :-------------------------------------------------------------------- |
| **Date**   | Date    | The trading date (MM/DD/YYYY format).                                 |
| **Close**  | Float   | The final price at which the stock traded during the regular session. |
| **High**   | Float   | The highest price at which the stock traded during the day.           |
| **Low**    | Float   | The lowest price at which the stock traded during the day.            |
| **Open**   | Float   | The price at which the stock first traded upon the market opening.    |
| **Volume** | Integer | The total number of shares traded during the day.                     |

---

## c. Top 5 Kaggle Tags

1. `Finance`
2. `Stock Market`
3. `Time Series Analysis`
4. `Data Visualization`
5. `IBM`

---

## d. SEO-Optimized Metadata

- **SEO Project Name:** IBM Stock Market Historical Dataset 2000-2026
- **SEO Description:** Download the complete IBM stock price historical dataset (2000-2026). Features daily Open, High, Low, Close (OHLC) and Volume data for financial modeling, trend analysis, and deep learning.

---

## e. Dataset Coverage

- **Data Coverage:** 100% (Daily trading days excluding weekends and market holidays).
- **Format:** CSV (Comma-Separated Values).
- **Volume:** ~6,560 rows of daily market activity.

---

## f. Temporal & Geospatial Scope

- **Start Date:** 01/03/2000
- **End Date:** 01/30/2026
- **Relevant Country:** USA
- **Relevant City:** Armonk, New York (IBM Headquarters)
- **Primary Market:** New York Stock Exchange (NYSE)

---

## g. Provenance & Transformations

- **Source:** Historical market data points were aggregated from financial data providers such as Yahoo Finance and Alpha Vantage.
- **Transformations:**
  - Data cleaned for missing values.
  - Standardized date formatting to MM/DD/YYYY.
  - Precision of decimal values maintained for Close, High, Low, and Open prices.

---

## h. Collection Methodology

Data was collected using API-based extraction from reputable financial repositories. The methodology involves scraping daily OHLC records and trading volumes, followed by a validation step to ensure consistency between different financial reporting sources.

---

## i. Biggest Problems & Challenges

1. **Market Volatility:** IBM's long history includes significant shifts in the tech landscape, making long-term forecasting difficult without external context (e.g., earnings reports, global events).
2. **Missing Data Points:** Occasional gaps due to exchange-specific closures or technical glitches in historical feeds require interpolation or external validation.
3. **Corporate Actions:** Handling stock splits and dividends correctly in "Close" vs "Adjusted Close" calculations is critical for accuracy.
4. **Outlier Management:** Sudden spikes in volume during earnings calls can skew statistical models if not properly normalized.
5. **Data Decay:** Older records might have lower precision or different reporting standards compared to modern electronic trading records.

---

## j. Correct Source & Link

- **Source:** Yahoo Finance / NYSE Historical Records
- **Source Link:** [https://finance.yahoo.com/quote/IBM/history/](https://finance.yahoo.com/quote/IBM/history/)

---

## k. Step-by-Step Problem Development Walkthrough

1. **Initial Identification:** The need for a long-term, high-quality historical dataset for IBM became apparent when studying the transition from hardware to cloud/AI-centric business models.
2. **Data Acquisition:** Identified the primary trading period (2000-2026) to capture the dot-com bubble burst, the 2008 financial crisis, the cloud transition era, and the recent AI booms.
3. **Preprocessing:** Raw data often contained "Dirty" fields or inconsistent volume reporting across different exchanges.
4. **Alignment:** OHLC data was synced to ensure that `Low <= (Open, Close) <= High` across all 6,000+ entries.
5. **Contextualization:** The final step involves mapping these numbers to real-world events to provide a narrative for why certain price actions occurred.
