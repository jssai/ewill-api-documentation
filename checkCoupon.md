# Check coupon code

<div class="method method-get">GET</div> <span class="url">https://app.ewill.io/server/api/customers/me/checkCoupon/{code}</span>

> Check coupon code validity

### Parameters in URL

|Name|Description|Type|Required|
| --- | --- | --- |
| `code` | Coupon code | `string` | <div class="required">*</div> |


### Response Example

```json
{
    "usedBy": null,
    "code": "XXXX",
    "discount": 50.00,
    "createdAt": "2018-01-01T12:00:00.000Z",
}
```

### Response Messages

* `200` Success
* `401` Authorization required
* `401` Coupon code unavailable
* `500` Error
