# geo.crypto
An easy-to-customize cryptocurrency ticker for Rainmeter.

TODO:
- Add variants for different currencies.
- Add red/green/white-colored text to show currency trends.

Instructions:

To remove a crypto, just delete the entire block reading from "; COIN X START" to "; COIN X END".

To add a crypto, copy one of those blocks and change the coin number in each heading (i.e., measureCoinXName, etc.).
Make sure you copy the blocks and change the heading names in both "MEASURES" and "METERS".
You'll also need to change the following variable values:

measureCoinXName String - Change to what the coin is called, such as "BTC" or "Bitcoin".

measureCoinXUrl URL - The coinmarketcap API address for this coin (https://coinmarketcap.com/api/).

measureCoinXValue URL - Should be "measureCoinXUrl".

measureCoinXPrice Formula - Should be "measureCoinXValue".

meterCoinXName MeasureName - Should be "measureCoinXName".

meterCoinXValue MeasureName - Should be "measureCoinXPrice".

meterCoinXValue NumOfDecimals - The number of decimals for this value. Smaller-value cryptos need more decimals to be able to display their value.


If you find this useful, please donate!

BTC = 184J6U6h8gVUsdKAkexJ67Zqp3qbbYz2gt

ETH = 0xe9593011eA2b8f224896ce032913D7D38beF2875

XRP = rBjWBHKyvhJR5wDsSgvwbAuMWzFh3xqmXE

SC  = dda34ab07247a2cafe280e1e18e7c70491628fc2bef824f9a746f0ed4062b614516089d3bf68
