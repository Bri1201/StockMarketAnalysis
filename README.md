# Indian Stock Market Analysis Project

This project focuses on analyzing stocks in the Indian stock market by utilizing the `yfinance` library in Python. It aims to identify and highlight stocks with significant growth in trade volume over the past few hours. The project employs AWS Lambda for executing frequent code runs and automating the process of data analysis and notification.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)


## Introduction

The Indian Stock Market Analysis Project is designed to provide insights into the stock market's trade volume trends and help users identify potential investment opportunities. By gathering data using the `yfinance` library, the project calculates the change in trade volume for various stocks and generates a list of the top 20 stocks that have experienced the most significant trade volume growth over the specified time period. Users are then notified via email about these high-growth stocks.

## Features

- Fetches daily stock data using the `yfinance` library.
- Compares trade volume changes for different stocks.
- Emails a list of the top 20 stocks with the highest trade volume growth.
- Utilizes AWS Lambda for automated and frequent code runs.

## Installation

1. Clone the repository:

```bash
git clone https://github.com/your-username/indian-stock-analysis.git
```

2. Change to the project directory:

```bash
cd StockNewsletter
```

3. Install the required dependencies:

```bash
pip install yfinance
```


## AWS Lambda Integration

This project can be integrated with AWS Lambda to automate the analysis and notification process. To set up AWS Lambda:

1. Package your code: Create a deployment package containing your code and dependencies.

2. Configure AWS Lambda: Create a new Lambda function on AWS and upload the deployment package. Set up a trigger for the Lambda function to run at desired intervals.

3. Environment Variables: Set the required environment variables (e.g., `EMAIL_CONFIG`) in the Lambda function to provide email configuration.

4. Test and Monitor: Test the Lambda function to ensure it works as expected. Monitor logs and notifications to verify successful execution.
