# pontstrader

pontstrader is a trading script running on python2.7 which adds some extra features to the default Bittrex trading possibilities trough the webinterface.

## What can users do with pontstrader

1. Buy cryptocurrencies (Bittrex)
2. Sell cryptocurrencies (Bittrex)
3. Buy cryptocurrencies and immidiatly add a sell order with a multiplier (Bittrex)
4. Check their balances (Bittrex)
5. Check their orderbook (Bittrex)
6. Watch a cryptocurrencies in real-time 0.5 seconds (Bittrex)
7. Withdraw cryptocurrencies (Bittrex)
8. Check arbitrage oppertunaties between exchanges (Bittrex, HitBTC, Binance, Bitfinex, Poloniex)
9. Use Trailing Stop Loss, which is normally not possible on most exchanges (Bittrex)

Some of the above functions require the script to run on a system which is on 24/7, this is due to the fact the script is actively (every 0.5 seconds) quering the pontstrader redis database for price changes.
Currently the following functions require a 24/7 running system:

- Trailing Stop Loss

## What can users expect from pontstrader in the near future

1. Stop Loss + Take Profit function which allows you to set not just one but multiple tresholds, which means the script will not only sell when it hits your stop loss treshold but will also sell when it hits your profit tresholds. Normally you can only choose one on Bittrex. (this will also require a 24/7 running system)
2. Stop Loss + Take Profit multiple sell tresholds. Same as the above, but then a 50/50 split in selling tresholds. For example you want to sell 50% at 5% profit, and the other 50% at 10%. (this will also require a 24/7 running system)
3. Multiple exchange support on every function, currently only Bittrex is supported on most of them
4. And much more!

## Getting started

### 1. Install python 2.7
  - Windows & Mac: https://www.python.org/downloads/release/python-2714/
  - Linux: apt-get install python2.7 / yum install python2.7

### 2. Install python-pip:
  - Windows: https://pip.pypa.io/en/stable/installing/
  - Linux: apt-get install python-pip / yum install python-pip
  - Mac:
  ```
  easy_install pip
  ```

### 3. Install python-requests
  - Windows (This only works when you've successfully installed python-pip):
  ```
  C:\Python27\python.exe -m pip install requests
  ```
  - Linux:
  ```
  apt-get install python-requests / yum install python-requests
  ```
  - Mac:
  ```
  python -m pip install requests
  or
  easy_install request
  ```

### 4. Install python-colorama for colors:
  - Windows: https://pypi.python.org/pypi/colorama/0.2.7#downloads
  - Linux:
  ```
  apt-get install python-colorama / yum install python-colorama
  ```
  - Mac:
  ```
  python <pathtocolorama>/setup.py install
  or
  easy_install colorama
  ```
  
### 5. Install python-redis
  - Windows:
  ```
  C:\Python27\python.exe -m pip install redis
  ```
  Linux: 
  ```
  pip install redis
  ```
  Mac:
  ```
  pip install redis
  or
  easy_install redis
  ```
