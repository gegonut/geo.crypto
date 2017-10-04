This is a cryptocurrency ticker designed to be very easy to customize and blend in well with the default Rainmeter widgets.
Provided by Geo.Ego on DeviantArt.
https://gegonut.deviantart.com/

To remove a crypto, just delete the entire block reading from "; COIN X START" to "; COIN X END" in both "MEASURES" and "METERS". Also, delete the cryptoXUrl variable line from [Variables].

To add a coin, first add the "cryptoUrlX" URL for the coin in the [Variables] section. An example for ZCash would be:
crypto6URL=https://api.coinmarketcap.com/v1/ticker/zcash/
The correct URLs can be figured out by visiting https://coinmarketcap.com/api/.

Next, copy the blocks and change the heading names in both "MEASURES" and "METERS".
You'll also need to change the following variable values:

measureCoinXName String - Change to what the coin is called, such as "BTC" or "Bitcoin".

measureCoinXUsd URL - Should be "#cryptoXUrl#".

measureCoinXValue URL - Should be "measureCoinXUsd".

measureCoinXPercentChange URL - Should be "#cryptoXUrl#".

measureCoinXChangeValue - Should be "measureCoinXPercentChange".

measureCoinXPrice Formula - Should be "measureCoinXValue".

measureCoinXChange - All instances of "measureCoinX" and "meterCoinX" should be changed to this coin's number.

meterCoinXName MeasureName - Should be "measureCoinXName".

meterCoinXValue MeasureName - Should be "measureCoinXPrice".

meterCoinXValue NumOfDecimals - The number of decimals for this value. Smaller-value cryptos need more decimals to be able to display their value.

meterCoinXChange MeasureName - Should be "measureCoinXChange".



If you find this useful, please donate!

BTC = 184J6U6h8gVUsdKAkexJ67Zqp3qbbYz2gt

ETH = 0xe9593011eA2b8f224896ce032913D7D38beF2875

XRP = rBjWBHKyvhJR5wDsSgvwbAuMWzFh3xqmXE

SC  = dda34ab07247a2cafe280e1e18e7c70491628fc2bef824f9a746f0ed4062b614516089d3bf68
