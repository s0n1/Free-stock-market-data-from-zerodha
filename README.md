📈 Zerodha Free Historical Data Fetcher

🔥 Introduction

Zerodha’s Kite Connect API allows traders to fetch historical market data. However, accessing this data comes with limitations, and Zerodha does not provide it for free through its web platform. This project offers a Python script that efficiently retrieves minute-by-minute historical data for free using Zerodha’s API, helping traders analyze past price movements without incurring extra costs.

⚠️ Zerodha Data Limitations

Zerodha does not provide historical data for free via its web trading platform. If you need detailed minute-level historical data, you must use their Kite Connect API, which requires a paid subscription. Even with the API, there are strict limitations:

⏳ Only 2 months of minute data can be fetched at a time.

🚀 Max 3 API requests per second (Rate limit enforced by Zerodha).

📉 Only up to 2000 minute-candles per request (~33 hours of data at a time).

⏱️ No tick-by-tick data (Only OHLCV format is provided for historical queries).

How This Project Helps You Fetch Free Data

With this Python script, you can:

Fetch historical minute-level OHLCV data for free using the Kite Connect API.

Store the data in CSV format for future analysis.

Automate the retrieval of multiple instruments without hitting API rate limits.

Use Zerodha WebSockets (optional) for real-time price updates.

🛠️ How to Use

1️⃣ Install Required Libraries

Ensure you have Python installed and install the required packages:

pip install pandas requests

2️⃣ Get Your Zerodha API Credentials

To use this script, you need to sign up for Kite Connect API on Zerodha’s developer portal and get your:

API Key

Access Token

3️⃣ Run the Script

Modify the script with your credentials and run:

python fetch_data.py

This will fetch minute-level historical data and save it as a CSV file.

🚀 Features

📊 Fetches historical data for any stock, index, or commodity.

🕒 Stores data in CSV format with timestamps as index.

🔄 Supports multiple instruments without exceeding API rate limits.

🏎️ Optimized to fetch data as fast as possible within Zerodha’s API constraints.

⚠️ Disclaimer

This tool is for educational purposes only. You must comply with Zerodha’s terms of service and use the API responsibly. Excessive API requests may lead to temporary or permanent bans on your account.

