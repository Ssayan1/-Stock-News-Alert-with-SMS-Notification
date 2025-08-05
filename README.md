# 📈 Stock News Alert with SMS Notification

This project sends SMS alerts with the latest news when a stock price changes significantly. It uses the **Alpha Vantage API** to get stock prices, the **NewsAPI** to fetch relevant news headlines, and **Twilio** to send SMS messages.

---

## 🔧 Features

- Tracks stock price changes (e.g., TSLA – Tesla Inc)
- Detects if the price changes more than a certain threshold (e.g., 5%)
- Fetches the top 3 latest news articles about the company
- Sends SMS alerts using Twilio API

---

## 🚀 Technologies Used

- Python 🐍
- [Alpha Vantage API](https://www.alphavantage.co/)
- [NewsAPI](https://newsapi.org/)
- [Twilio](https://www.twilio.com/)
- `requests`, `twilio`, `python-dotenv`

---

## 📂 Project Structure

```bash

stock-news-alert/
│
├── main.py # Main Python script
├── .env # Stores API keys (excluded from GitHub)
├── .gitignore # Ignores .env and other unnecessary files
├── requirements.txt # Python dependencies
└── README.md # You're reading it!

```
---

## ⚙️ Setup Instructions
### 1. Clone this repo
```bash
git clone https://github.com/YOUR_USERNAME/stock-news-alert.git
cd stock-news-alert
```
### 2. Create and activate virtual environment (optional but recommended)
```bash
python -m venv .venv
source .venv/bin/activate  # macOS/Linux
.venv\Scripts\activate     # Windows
```
### 3. Install dependencies
```bash
pip install -r requirements.txt
```
### 4. Create a .env file and add your API credentials
```bash
STOCK_API_KEY=your_alphavantage_api_key
NEWS_API_KEY=your_newsapi_key
TWILIO_SID=your_twilio_sid
TWILIO_AUTH_TOKEN=your_twilio_auth_token
VIRTUAL_TWILIO_NUMBER=your_twilio_virtual_number
VERIFIED_NUMBER=your_verified_phone_number
```
### 5. Run the script
```bash
python main.py
```
---

## 📱 Sample Output
When a stock moves more than 5%:
```bash
TSLA: 🔺6%
Headline: Tesla announces new self-driving update.
Brief: Tesla's new update includes major improvements to Full Self-Driving technology.
```
----
## ⚠️ Important Notes
- Make sure your Twilio number is verified and able to send SMS to your personal number.
- Alpha Vantage's free tier has request limits
- Never commit your .env or API keys to GitHub.

---

## 📜 License
This project is for educational purposes. You can use or modify it for personal or learning projects.

---

## 🙋‍♂️ Author
Sayan Sanki
 https://github.com/Ssayan1/-Stock-News-Alert-with-SMS-Notification.git

 ---

 ## Let me know if you'd like:
- A **version** where your credentials are read from `.env`
- Help writing a `.env` parser using `dotenv`
- Help pushing this `README.md` to your repo




