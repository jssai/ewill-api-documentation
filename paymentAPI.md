# Create payment

<div class="method method-post">POST</div> <span class="url">https://app.ewill.io/server/api/customers/me/paymentAPI</span>

> Create payment through Stripe

### Parameters in JSON

|Name|Description|Type|Required|
| --- | --- | --- |
| `name` | Full name | `string` | <div class="required">*</div> |
| `number` | Card number | `string` | <div class="required">*</div> |
| `cvc` | CVC | `string` | <div class="required">*</div> |
| `expiry` | Card expiry | `string` | <div class="required">*</div> |
| `stripeToken` | Stripe token | `string` | <div class="required">*</div> |
| `code` | Coupon code | `string` | <div class="required">*</div> |
| `amount` | Amount | `number` | <div class="required">*</div> |
| `paymentType` | `simpleLawyer` or `mirrorLawyer` | `string` | <div class="required">*</div> |
| `description` | Description | `string` | - |
| `willType` | `simple` or `null` | `string` | - |

### Response Example

```json
{
    "status": "succeeded"
}
```

### Response Messages

* `200` Success
* `401` Authorization required
* `500` Error
