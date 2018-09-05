# Get worth metrics

<div class="method method-get">GET</div> <span class="url">https://app.ewill.io/server/api/customers/me/getWorthMetrics</span>

> Get worth metrics logged

### Response Example

```json
[
    {
        "email": "john.doe@gmail.com",
        "worth": 200000,
        "customerId": "XXXXXXXXXXXXXXXXXXXXXXXX",
        "currency": "GBP",
        "loggedTime": "2018-01-01T00:00:00.00"
    }
]
```

### Response Messages

* `200` Success
* `401` Authorization required
* `500` Error
