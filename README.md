# Vault of Satoshi API
[![NPM](https://nodei.co/npm/request.png)](https://nodei.co/npm/vos-api/)

# Endpoint Support
```
/public/ticker  Get trading statistics
/public/orderbook   Get the list of open orders/price levels
/info/currency  Get information about supported currencies
/info/account   Get information about an Api-Key and account
/info/balance   Get wallet balances
/info/wallet_address    Get addresses of wallets
/info/wallet_history    Get list of transfer into/out of wallet
/info/ticker    Get trading statistics
/info/quote Get quote for a trade
/info/orderbook Get the list of open orders/price levels
/info/orders    Get information about your orders
/info/order_detail  Get list of transactions resulting from an order
/trade/place    Place an order
/trade/cancel   Cancel an order
```

# How it works
```javascript
var vos = require('vos-api')('key','secret');

var currency_pair = {
    order_currency: 'btc',
    payment_currency: 'usd'
};

function callback(ticker_data) {

}
vos.Public.ticker(currency_pair, callback);
```
