# Flipkart Web Scraper

## Project Overview
This Python script scrapes book details from Flipkart, including the title, author, publication year, price, and rating. It also tracks price changes over time by saving the data in a CSV file. Additionally, it includes an email notification system that alerts the user when the book price drops below a specified amount.

## Features
- **Web Scraping**: Extracts book details using `BeautifulSoup` and `requests`.
- **Data Storage**: Saves the extracted data into a CSV file.
- **Automated Price Tracking**: Runs periodically (every 24 hours) to track price changes.
- **Email Alerts**: Sends an email notification when the book price falls below a set threshold.

## Technologies Used
- Python
- BeautifulSoup
- Requests
- Pandas
- CSV Handling
- SMTP (for email notifications)

## How to Use
1. **Install Required Libraries**:
   ```bash
   pip install beautifulsoup4 requests pandas
   ```
2. **Run the Script**:
   ```bash
   python flipkart_scraper.py
   ```
3. **Modify Email Credentials**:
   - Update the `send_mail()` function with your Gmail credentials.

## Notes
- Ensure your Gmail account allows less secure apps or set up an app password.
- Flipkart's website structure may change, requiring class selectors to be updated.
- Running the script continuously (every 24 hours) will help track price changes effectively.

## Disclaimer
This project is for educational purposes only. Scraping websites without permission may violate their terms of service.

