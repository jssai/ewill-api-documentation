# Change current customer's password

<div class="method method-post">POST</div> <span class="url">https://app.ewill.io/server/api/customers/me/changePassword</span>

> Change current customer's password

### Parameters in query string

|Name|Description|Type|Required|
| --- | --- | --- |
| `access_token` | Access token | `string` | <div class="required">*</div> |

### Parameters in JSON

|Name|Description|Type|Required|
| --- | --- | --- |
| `oldPassword` | Password | `string` | <div class="required">*</div> |
| `newPassword` | Password (Minimum 8 characters, at least one upper case letter, at least one number, at least one special character) | `string` | <div class="required">*</div> |

### Response Messages

* `200` Success
* `400` Invalid password
* `401` Old password doesn't match
* `401` Unkown user
