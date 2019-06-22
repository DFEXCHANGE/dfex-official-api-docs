# **DFEX**


### Exchange information
```
GET /polarisex/coin/exchangeInfo
```
Current exchange trading rules and symbol information

**Weight:**
1

**Parameters:**
NONE

**Response:**
```javascript
{
  "timezone": "UTC",
  "serverTime": 1508631584636,
  "rateLimits": [
    // These are defined in the `ENUM definitions` section under `Rate limiters (rateLimitType)`.
    // All limits are optional.
  ],
  "exchangeFilters": [
    // There are defined in the `Filters` section.
    // All filters are optional.
  ],
  "symbols": [{
    "symbol": "ETHBTC",
    "status": "TRADING",
    "baseAsset": "ETH",
    "baseAssetPrecision": 8,
    "quoteAsset": "BTC",
    "quotePrecision": 8,
    "orderTypes": [
      // These are defined in the `ENUM definitions` section under `Order types (orderTypes)`.
      // All orderTypes are optional.
    ],
    "icebergAllowed": false,
    "filters": [
      // There are defined in the `Filters` section.
      // All filters are optional.
    ]
  }]
}
```
### Get Currencies

**HTTP Requests**

GET /api/account/v3/currencies

**Request Sample**

GET /polarisex/coin/currencies

**Return Parameters**

Parameters	    
currency	    
name	       
can_deposit	    
can_withdraw	
min_withdrawal

**Response:**
```javascript

{
  "attachment": [
    {
      "can_deposit": 1,
      "can_withdraw": 1,
      "currencyId": 0,
      "currency": "BTC",
      "min_withdrawal": 0.01,
      "name": ""
    },
    {
      "can_deposit": 1,
      "can_withdraw": 1,
      "currencyId": 0,
      "currency": "LTC",
      "min_withdrawal": 0.1,
      "name": ""
    }
  ],
  "status": 200,
  "message": null
}
```