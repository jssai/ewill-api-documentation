# Get asset

<div class="method method-get">GET</div> <span class="url">https://app.ewill.io/server/api/customers/{customerId}/assets/{assetId}</span>

> Get assets of the customer

### Parameters in URL

|Name|Description|Type|Required|
| --- | --- | --- |
| `customerId` | Customer ID | `string` | <div class="required">*</div> |
| `assetId` | ID of the asser | `string` | <div class="required">*</div> |


### Response Example

```json
[{
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
}]
```

### Response Messages

* `200` Success
* `401` Authorization required
* `500` Error
