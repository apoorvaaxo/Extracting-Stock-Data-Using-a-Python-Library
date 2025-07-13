# 📊 Extracting Stock Data Using a Python Library

Welcome to my project repository for the IBM course **"Python Project for Data Science"**. This repository contains my Jupyter Notebook for the lab titled **"Extracting Stock Data Using a Python Library"**.

## 🧠 What I Learned

This lab is a practical demonstration of how Python, when combined with libraries like `yfinance` and `pandas`, can be a powerful tool for financial data analysis. Here’s a summary of what I learned:

- 📌 What stocks and shares represent in the real world.
- 💹 How to use the `yfinance` library to extract **real-time and historical stock data**.
- 🧮 How to work with **Pandas DataFrames** to analyze financial datasets.
- 📈 How to visualize stock data using basic plotting.
- 🧪 Completed hands-on **exercises and quizzes** to reinforce learning.
- 🔍 Understood how data scientists can detect **suspicious stock activity** or trends using Python tools.

## 🗂️ About the Lab

In this lab, I took on the role of a **data scientist at a hedge fund**. My task was to investigate stock activity by extracting and analyzing real-world stock data.

**Key objectives:**
- Understand how to work with Python libraries like `yfinance` to fetch stock market data.
- Use Pandas to manipulate and explore the stock data returned.
- Learn how financial time-series data works.
- Prepare for further data science applications in the financial domain.

## 📦 Tools & Libraries Used

- Python 🐍
- [yfinance](https://pypi.org/project/yfinance/)
- pandas
- datetime
- matplotlib

## 🔎 Lab Topics Covered

- Introduction to stocks and the stock market
- Retrieving data for a specific ticker (like AAPL, TSLA, etc.)
- Getting the **historical prices** of a stock
- Filtering stock data by date
- Extracting **open**, **high**, **low**, and **close** prices
- Performing **basic visualizations** with `matplotlib`

## 🎓 Certificate of Completion

✅ I have successfully completed this lab as part of the IBM course **"Python Project for Data Science"**.  
📎 The certificate is included in this repository as:  
**`IBM_Certificate_Extracting_Stock_Data.pdf`**

## 🧪 Why This Lab Is Important

This lab is designed to help beginners understand how **Python can be used in real-world data science scenarios**, especially in the financial industry. By working through it, I gained insight into how hedge funds or analysts might:
- Track stock performance
- Spot anomalies
- Analyze market trends using code rather than spreadsheets

## 📁 Files Included

- `ExtractingStockDataUsingaPythonLibrary.ipynb`: Jupyter Notebook with all code, output, and explanations.
- `README.md`: This file explaining the lab and its outcomes.

## 📈 Sample Code Snippet

```python
import yfinance as yf

# Define the ticker symbol
tickerSymbol = 'TSLA'

# Get data on this ticker
tickerData = yf.Ticker(tickerSymbol)

# Get the historical prices for this ticker
tickerDf = tickerData.history(period='1d', start='2020-1-1', end='2023-1-1')

# See the closing prices
tickerDf['Close'].plot(title="Tesla Closing Prices")
