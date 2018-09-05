# Send password reset request

<div class="method method-post">POST</div> <span class="url">https://app.ewill.io/server/api/customers/reset</span>

> Send a request to reset customer's password

### Parameters in JSON

|Name|Description|Type|Required|
| --- | --- | --- |
| `email` | Email address | `string` | <div class="required">*</div> |
| `gRecaptchaResponse` | Google Recaptcha response | `string` | <div class="required">*</div> |

### Response Messages

* `204` Success
* `400` Email required
* `404` Email not found
* `401` Reset failed due to lack of email verification
