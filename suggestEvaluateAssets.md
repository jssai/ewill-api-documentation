# Get value suggestion

<div class="method method-post">POST</div> <span class="url">https://app.ewill.io/server/api/customers/me/suggestEvaluateAssets</span>

> Get value suggestion, returns asset with evaluated market value using external services

### Parameters in JSON

|Name|Description|Type|Required|
| --- | --- | --- |
| `asset` | Asset object | `object` | <div class="required">*</div> |


### Response Example

```json
{
    "evaluatedMarketValue": 1200,
    "marketValue": 1200,
    "sourceMarketValue": "External",
    "description": "",
    "value": 1000,
    "marketValue": 1000,
    "displayValue": 1000,
    "convertedPurchaseValue": 886.6012867761883,
    "convertedMarketValue": 887,
    "category": "Property",
    "subCategory": "House",
    "images": [],
    "thumbnails": [],
    "title": "House",
    "subTitle": "house",
    "assetUniqueId": "_AV43453_PRO_HOU_undefined_EA2536D8",
    "id": "XXXXXXXXXXXXXXXXXXXXXXXX",
    "customerId": "XXXXXXXXXXXXXXXXXXXXXXXX",
    "referenceId": "XXXXXXXXXXXX",
    "idM": "asset1",
    "currency": "EUR",
    "yourOwnershipShared": {
        "isShared": false,
        "sharedWith": "",
        "ownershipPercentage": ""
    },
    "yourLiabilitiesEncumbrances": {
        "isLiabilitiesEncumbrances": false,
        "typeOf": "",
        "value": "",
        "currency": "GBP"
    },
    "location": "",
    "entityDescription": "house",
    "assetType": "NonFinancial",
    "sourceMarketValue": "None",
    "convalue": "marketValue",
    "isCreatedFromWill": true
}
```

### Response Messages

* `200` Success
* `401` Authorization required
* `500` Error
