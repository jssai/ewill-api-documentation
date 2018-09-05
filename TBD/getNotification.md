# Get notifications

<div class="method method-get">GET</div> <span class="url">https://app.ewill.io/server/api/consumers/me/getNotification</span>

> Get notifications

### Response Example

```json
[
    {
        "destUserId": "XXXXXXXXXXXXXXXXXXXXXXXX",
        "srcUserId": "YYYYYYYYYYYYYYYYYYYYYYYY,
        "notifType": "request",
        "message": "accepted your request.",
        "timestamp": "2018-01-01T12:00:00.000Z",
        "isRead": false,
        "decline": false,
        "customerData": {},
    }
]
```

### Response Messages

* `401` Authorization required
* `200` Success
* `500` Error
