# Get equity list

<div class="method method-get">GET</div> <span class="url">https://app.ewill.io/server/api/customers/me/getEquityList/{searchQuery}</span>

> Get results for an equity search query

### Parameters in URL

|Name|Description|Type|Required|
| --- | --- | --- |
| `searchQuery` | Search query | `string` | <div class="required">*</div> |


### Response Example

```json
{
    "ResultSet": {
        "Query": "XXX",
        "Result": [{
            "typeDisp": "Equity",
            "name": "Eternity Technology Holdings Limited",
            "symbol": "1725.HK",
            "exchDisp": "Hong Kong",
            "type": "S",
            "exch": "HKG"
        }, {
            "typeDisp": "Equity",
            "name": "Xiaomi Corporation",
            "symbol": "1810.HK",
            "exchDisp": "Hong Kong",
            "type": "S",
            "exch": "HKG"
        }]
    }
}
```

### Response Messages

* `200` Success
* `401` Authorization required
* `500` Error
