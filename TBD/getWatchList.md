# Get watch list

<div class="method method-get">GET</div> <span class="url">https://app.ewill.io/server/api/customers/me/getWatchList/{searchQuery}</span>

> Get watch list

### Parameters in URL

|Name|Description|Type|Required|
| --- | --- | --- |
| `searchQuery` | Search query | `string` | <div class="required">*</div> |


### Response Example

```json
{
    "ResultSet": {
        "Query": "apple",
        "Result": [{
            "symbol": "AAPL",
            "name": "Apple Inc.",
            "exch": "NAS",
            "type": "S",
            "exchDisp": "NASDAQ",
            "typeDisp": "Equity"
        }, {
            "symbol": "APLE",
            "name": "Apple Hospitality REIT, Inc.",
            "exch": "NYQ",
            "type": "S",
            "exchDisp": "NYSE",
            "typeDisp": "Equity"
        }, {
            "symbol": "AAPL.MX",
            "name": "Apple Inc.",
            "exch": "MEX",
            "type": "S",
            "exchDisp": "Mexico",
            "typeDisp": "Equity"
        }, {
            "symbol": "APC.F",
            "name": "Apple Inc.",
            "exch": "FRA",
            "type": "S",
            "exchDisp": "Frankfurt",
            "typeDisp": "Equity"
        }, {
            "symbol": "APRU",
            "name": "Apple Rush Company, Inc.",
            "exch": "PNK",
            "type": "S",
            "exchDisp": "OTC Markets",
            "typeDisp": "Equity"
        }, {
            "symbol": "AAPL.SW",
            "name": "Apple Inc.",
            "exch": "EBS",
            "type": "S",
            "exchDisp": "Swiss",
            "typeDisp": "Equity"
        }, {
            "symbol": "APC.DE",
            "name": "Apple Inc.",
            "exch": "FRA",
            "type": "S",
            "exchDisp": "Frankfurt",
            "typeDisp": "Equity"
        }, {
            "symbol": "AAPL.BA",
            "name": "Apple Inc.",
            "exch": "BUE",
            "type": "S",
            "exchDisp": "Buenos Aires",
            "typeDisp": "Equity"
        }, {
            "symbol": "AAPL-EUR.SW",
            "name": "Apple",
            "exch": "EBS",
            "type": "S",
            "exchDisp": "Swiss",
            "typeDisp": "Equity"
        }, {
            "symbol": "0R2V.L",
            "name": "Apple Inc.",
            "exch": "LSE",
            "type": "S",
            "exchDisp": "London",
            "typeDisp": "Equity"
        }]
    }
}
```

### Response Messages

* `200` Success
* `401` Authorization required
* `500` Error
