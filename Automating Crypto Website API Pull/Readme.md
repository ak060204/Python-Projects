# Automating Crypto Website API Pull

## Project Overview
This project automates the process of pulling cryptocurrency data from the CoinMarketCap API. The script fetches live market data, processes it into a Pandas DataFrame, saves it to a CSV file, and visualizes the price changes over time using Seaborn and Matplotlib.

## Features
- Fetches live cryptocurrency data from CoinMarketCap API.
- Processes data into a Pandas DataFrame.
- Saves data to a CSV file for further analysis.
- Runs the API request automatically every minute for 333 iterations.
- Analyzes percentage changes in cryptocurrency prices.
- Generates visualizations using Seaborn and Matplotlib.

## Technologies Used
- Python
- Requests (for API calls)
- Pandas (for data processing)
- Matplotlib & Seaborn (for data visualization)
- OS & Time (for scheduling requests)

## Installation & Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo-name.git
   ```
2. Install dependencies:
   ```bash
   pip install requests pandas matplotlib seaborn
   ```
3. Replace `'X-CMC_PRO_API_KEY'` with your actual API key in the script.
4. Run the script:
   ```bash
   python script.py
   ```

## How It Works
1. The script fetches live data from CoinMarketCap API every minute.
2. It processes the response and normalizes it into a Pandas DataFrame.
3. The data is saved to `API.csv` for tracking historical changes.
4. It groups and analyzes the percentage change of different cryptocurrencies.
5. Data is visualized using Seaborn, plotting price trends and percentage changes.

## Data Visualization
- A point plot is generated to compare percentage changes over various time frames.
- A line plot visualizes the price trend of Bitcoin over time.

## Future Improvements
- Implement error handling for missing API responses.
- Store data in a database instead of CSV.
- Expand analysis to include more advanced metrics.



