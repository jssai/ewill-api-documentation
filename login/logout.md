# Customer signup

<div class="method method-post">POST</div> <span class="url">https://app.ewill.io/server/api/customers/logout</span>

> Logout a customer, unvalidate access token

### Parameters in query string

|Name|Description|Type|Required|
| --- | --- | --- |
| `access_token` | Access token | `string` | <div class="required">*</div> |

### Response Messages

* `204` Success
* `401` Unkown access token
