# Convert currency

<div class="method method-get">GET</div> <span class="url">https://app.ewill.io/server/api/customers/me/convertCurrency/{amount}/{currentCurrency}/{targetCurrency}</span>

> Convert an amount from one currency to another

### Parameters in URL

|Name|Description|Type|Required|
| --- | --- | --- |
| `amount` | Amount of current currency | `number` | <div class="required">*</div> |
| `currentCurrency` | Current currency code | `string` | <div class="required">*</div> |
| `targetCurrency` | Target currency code | `string` | <div class="required">*</div> |

### Response Example

> https://app.ewill.io/server/api/customers/me/convertCurrency/1/GBP/USD

```json
1.4090857851425995
```

### Response Messages

* `200` Success
* `401` Authorization required
* `500` Error
