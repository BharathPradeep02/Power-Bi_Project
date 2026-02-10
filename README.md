# Power-Bi_Project
An interactive Stock Market Analytics dashboard built using Python for data collection and Power BI for visualization.
This project fetches real-time & historical stock data using the yFinance API and transforms it into meaningful business insights.

Project Overview :
    The goal of this project is to analyze stock performance of major tech companies and present insights through an interactive dashboard.
The workflow:
    Python ➜ Fetch stock data ➜ Clean & transform ➜ Export dataset ➜ Power BI Dashboard
This project demonstrates skills in:
  Data Collection (API)
  Data Cleaning & Analysis (Python)
  Business Intelligence & Visualization (Power BI)

Tech Stack
Tool	Purpose
Python	Data fetching & preprocessing
yFinance	Stock market data API
Pandas	Data cleaning & transformation
Power BI	Dashboard & visualization

Dashboard Features

The dashboard provides key stock market insights such as:
🔹 KPIs
  Average Closing Price
  Average Opening Price
🔹 Visual Analytics
  Minimum Closing Price by Year (Donut Chart)
  Average Trading Volume by Company (Bar Chart)
Minimum Opening Price Drilldown by:
  Company
  Year
  Month
Power BI Q&A Insights panel
Company filter buttons (AAPL, MSFT, TSLA)
Data Collection (Python)
Stock data is fetched using the yFinance library.

Sample Python Code: 
  import yfinance as yf
  import pandas as pd
  stocks = ['AAPL','MSFT','TSLA']
  start_date = "2018-01-01"
  end_date = "2025-01-01"
  data = yf.download(stocks, start=start_date, end=end_date)
  data.to_csv("stock_data.csv")
  This dataset is then imported into Power BI for visualization.

📂 Project Structure
Stock-Market-Analysis/
│
├── data/
│   └── stock_data.csv
│
├── python/
│   └── fetch_stock_data.py
│
├── dashboard/
│   └── StockDashboard.pbix
│
└── README.md

