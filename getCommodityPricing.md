# Get commodity pricing

<div class="method method-post">POST</div> <span class="url">https://app.ewill.io/server/api/customers/me/getCommodityPricing</span>

> Get commodity pricing

### Parameters in JSON

|Name|Description|Type|Required|
| --- | --- | --- |
| `searchString` | Search query | `string` | <div class="required">*</div> |


### Response Example

```json
{
    "dataset_data": {
        "limit": 1,
        "transform": null,
        "column_index": null,
        "column_names": ["Date", "Open", "High", "Low", "Close", "Volume", "Ex-Dividend", "Split Ratio", "Adj. Open", "Adj. High", "Adj. Low", "Adj. Close", "Adj. Volume"],
        "start_date": "2012-05-18",
        "end_date": "2018-03-27",
        "frequency": "daily",
        "data": [
            ["2018-03-27", 156.31, 162.85, 150.75, 152.19, 76787884.0, 0.0, 1.0, 156.31, 162.85, 150.75, 152.19, 76787884.0]
        ],
        "collapse": null,
        "order": null
    }
}
```

### Response Messages

* `200` Success
* `401` Authorization required
* `500` Error
