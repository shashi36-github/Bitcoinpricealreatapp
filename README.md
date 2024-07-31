# Bitcoin Price Notification

Get notified of regular updates on the Bitcoin price via Gmail, Telegram, Twitter, Android SMS, and IFTTT app notifications. This script pushes notifications when the Bitcoin price changes at specified intervals. The default interval and threshold are set to 5 minutes and $10,000 respectively. Users can choose which of the 5 applications they want to receive notifications on.

## Description

Bitcoin prices are unpredictable. Instead of constantly checking various sites for the latest updates, use this Python app to automate the process.

- Utilizes the IFTTT automation service.
- Creates 4 IFTTT applets and 1 Gmail service for notifications:
  - Emergency notifications when Bitcoin price falls below a certain threshold, with updates sent to the user's chosen app(s).
  - Triggered by the Python app consuming data from the Coinmarketcap API.
  - An IFTTT applet includes a trigger and an action, triggered by a webhook service provided by IFTTT.
  - The Python app makes an HTTP request to the webhook URL, triggering an action. Actions can include sending an email, updating a Google Spreadsheet, or calling your phone.

## Prerequisites

You must have one of the following apps installed and/or must join or follow one of the following accounts:
  - IFTTT App
  - Telegram App and join this channel: [Telegram Channel](https://t.me/mybitcoinproject)
  - Twitter App and follow this account: [Twitter Account](https://twitter.com/AtanuPa02151991)
  - An email account
  - A contact number to receive SMS

### Links

- [GitHub Repository](https://github.com/shashi36-github/bitcoin_price_alert_app)
- [PyPI Package](https://pypi.org/project/bitcoin-price-alert-app/0.6/)

### Technology

Bitcoin price notifier utilizes the following:
* Python - core development language
* GitHub - version control
* PyPI - distribution
* IFTTT - notification automation services

### Installation

Bitcoin price alert application requires [Python 3](https://python.org/) v3+ to run.

1. Install PIP on Windows by running the following command in your terminal:
```sh
pip install
