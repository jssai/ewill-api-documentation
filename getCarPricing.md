# Get car price

<div class="method method-get">GET</div> <span class="url">https://app.ewill.io/server/api/customers/me/getCarPricing/{registrationNumber}</span>

> Get car price

### Parameters in URL

|Name|Description|Type|Required|
| --- | --- | --- |
| `registrationNumber` | Car registration number | `string` | <div class="required">*</div> |

### Response Example

```json
{
    "Vrm": "XXXXX",
    "Mileage": "110,000",
    "PlateYear": "2005-54",
    "ValuationList": {
        "OTR": "57797",
        "Dealer forecourt": "7460",
        "Trade Retail": "7040",
        "Private Clean": "6200",
        "Private Average": "6200",
        "Part Exchange": "4650",
        "Auction": "5120",
        "Trade Average": "5440",
        "Trade Poor": "5120"
    },
    "ValuationTime": "2018-09-01T00:00:00.00",
    "VehicleDescription": "LAND ROVER RANGEROVER SPT V8SC STD A"
}
```

### Response Messages

* `200` Success
* `401` Authorization required
* `500` Error
