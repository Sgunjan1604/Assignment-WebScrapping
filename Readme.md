## This project extracts news headlines and summaries from RSS feeds of multiple countries and news agencies.
Installation

## Clone this repository
Install dependencies:

pip install -r requirements.txt
The following libraries are required:

feedparser (for RSS parsing)
BeautifulSoup4 (for HTML parsing)
pandas (for data storage)
requests (for handling network requests)
sqlite3 (for database storage)

## How to Run

Run the main script:

python news_scraper.py

View the results in the output folder:


CSV format: output/news_data.csv
JSON format: output/news_data.json
Database file: output/news_database.db

## Features Implemented

Scrapes news from RSS feeds of 20+ countries
Extracts historical data from the past year
Stores data in multiple formats (CSV, JSON, SQLite)
Implements error handling for network failures and missing fields
Detects and categorizes news by language
Removes duplicates and irrelevant entries
Implements automatic scheduling via cron jobs

## Issues Encountered

Some RSS feeds had rate limiting, resolved by implementing delays between requests
Encoding issues with non-English characters, resolved by using UTF-8 encoding
Some RSS feeds did not provide full historical data, supplemented with web archives
Inconsistent date formats across different news sources, standardized using datetime parsing