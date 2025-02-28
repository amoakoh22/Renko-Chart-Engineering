# XAU/USD Renko Chart Analysis with Wick Tracking

This project analyzes XAU/USD (Gold vs. US Dollar) price data using Renko charts and incorporates wick tracking for enhanced insights into price action.

## Project Overview

Renko charts provide a unique perspective on price movements by filtering out noise and focusing on significant price changes. This project implements a custom Renko generator with wick tracking, enabling the identification of extreme wicks that may indicate potential trend reversals or significant price volatility.

## Features

- **Custom Renko Generator:** Generates Renko bricks from OHLC (Open, High, Low, Close) data with user-defined brick sizes.
- **Wick Tracking:** Calculates and stores wick lengths for each Renko brick, enabling analysis of price extremes within each brick.
- **Extreme Wick Detection:** Identifies and highlights Renko bricks with unusually long wicks, potentially indicating significant price volatility or trend changes.
- **Visualization:** Utilizes the `mplfinance` library to create visually appealing Renko charts with wick information.

## Requirements

- Python 3.x
- Libraries: `pandas`, `numpy`, `matplotlib`, `mplfinance`
- Google Colab environment (recommended)

## Installation
1. Install the required libraries using pip:
2. Mount your Google Drive to access the dataset:

## Usage

1. Update the `file_path` variable in the code to point to your XAU/USD dataset in CSV format.
2. Adjust the `brick_size` parameter to control the sensitivity of the Renko chart.
3. Run the code cells in the provided Colab notebook.

## Data

The project uses XAU/USD price data in OHLC format. The dataset should be in a CSV file with columns named "Date", "Time", "<OPEN>", "<HIGH>", "<LOW>", and "<CLOSE>".

## Results

The project generates a Renko chart with wick information displayed. It also identifies and prints the top 10 extreme wicks, highlighting potential areas of interest for further analysis.

## Limitations

- The accuracy of the Renko chart and wick analysis depends on the quality and frequency of the input data.
- The project currently focuses on XAU/USD data and may require modifications for other instruments.

## Future Enhancements

- Explore different brick size optimization techniques.
- Develop strategies for trading based on Renko chart patterns and wick analysis.
- Integrate with other technical indicators for comprehensive market analysis.
