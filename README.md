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

1 Installation for PIP on windows run the following command in your terminal
sh
pip install

2 Then install the app dependency, this app only requires 1 dependency, to install it run the following commond in you terminal

sh
pip install requests

3 Install bitcoin_price_alert_app package/module from PIP, to do that run the following command on terminal

sh
pip install bitcoin-price-alert-app==0.6

__IF THE APP DOES NOT INSTALL OR RUN PROPERLY AFTER STEP 3 THEN GO TO [THIS LINK](https://github.com/Atanu-Paul-au6/bitcoin_price_alert_app/archive/v0.6.2.tar.gz) TO DOWNLOAD THE ZIP FILE.__

### ALTERNATE STEP TO RUN THE APP AFTER DOWNLOADING THE ZIP FILE

* UNZIP THE FILE 
* OPEN YOUR CMD OR TERMINAL 
* GO TO THE FOLDER PATH OF THE UNZIPPED FOLDER EXAMPLE 'C:\Users\Desktop\bitcoin_price_alert_app-0.5\bitcoin_price_alert_app'


TYPE THE FOLLOWING COMMAND TO SEE HELP MENU
python bitcoin_price_notifier.py --help

you will see a menu like this
Welcome To Bitcoin Price Alert App
usage: bitcoin_alert_prototype4.py [-h] [-a alert_amount] [-t time_interval] [-l log_lenght] -d destination_app

Bitcoin Price Alert App.

optional arguments:
  -h, --help            show this help message and exit
  -a alert_amount, --alert_amount alert_amount
                        The price of 1 bitcoin when an emergency alert will be sent. Default is 7,18,715 INR
  -t time_interval, --time_interval time_interval
                        The time interval in minutes after which the lastest value of bitcoin will be fetched. Defalut is 5 minutes
  -l log_lenght, --log_lenght log_lenght
                        The number of records/entries you want example 5 entries at 5 minutes interval. Default length is 2
  -d destination_app, --destination_app destination_app
                        The mobile application on which you want to recive alert. Destination app options are (1) IFTTT app, (2) Telegram
                        App, (3) Email, (4) Twitter, (5) SMS

This app gives the value of 1 BTC in INR. Destination (-d) must be provided. To recive notification on IFTTT install IFTTT mobile app. To
recive notification on Telegram install Telegram mobile app and join this channel https://t.me/mybitcoinproject . Prerequisite : MUST HAVE A
IFTTT APP AND TELEGRAM APP INSTALLED TO RECIVE NOTIFICATION ALSO MUST JOIN THE TELEGRAM Bit_Coin CHANNEL TO RECIVE MESSAGES. PRESS Ctrl+C to
terminate the app

to run the app type the following command
python bitcoin_price_notifier.py -a 5000 -t 3 -l 5 -d email

* -a : alert limt amount in INR
* -t : time interval in minutes
* -l : the number of records needed
* -d : the destination app like email or telegram etc __THIS MUST BE PROVIDED__


Author: Sudana Shashi Kiran
