# telegram-news-automation
Zapier, RSS & Telegram API based news delivery bot.
# Automated News Delivery Bot (Zapier + RSS + Telegram)

A no-code automation workflow designed to fetch real-time news from RSS feeds and deliver them directly to a Telegram bot. 

## 📌 Project Overview
The objective of this project was to build a hands-free, automated news delivery system. It aggregates news from multiple RSS feeds and pushes the latest headlines directly to a Telegram chat.

## 🛠️ Tech Stack & Tools
- **Automation Platform:** Zapier
- **Data Source:** RSS Feeds (BBC, etc.)
- **Delivery Channel:** Telegram Bot API

## ⚙️ How It Works
1. **Trigger:** Zapier checks the specified RSS feed URLs every 15 minutes for new items.
2. **Action:** When a new article is detected, Zapier extracts the title, description, and link.
3. **Delivery:** Zapier formats the extracted data and sends it to the configured Telegram Bot using the Telegram API.

## 🚧 Challenges & Debugging
- **Issue:** Encountered `403 Forbidden` errors when fetching data from specific news outlets (e.g., Daily Star, Kalerkantho) due to server security filters blocking automated requests.
- **Solution:** Switched to alternative RSS feeds that allow webhook/automated pings, and utilized Google News RSS links as a workaround.

## 🚀 Future Enhancements
- Implement a database (SQL) to store multiple user Chat IDs.
- Convert this from a personal POC (Proof of Concept) to a public multi-user bot.
- Add an AI layer to summarize the news before sending.
