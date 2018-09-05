# Update customer's password

<div class="method method-post">POST</div> <span class="url">https://app.ewill.io/server/api/customers/:id/updatePassword</span>

> Update customer's password after password reset

### Parameters in URL

|Name|Description|Type|Required|
| --- | --- | --- |
| `id` | User ID | `string` | <div class="required">*</div> |

### Parameters in query string

|Name|Description|Type|Required|
| --- | --- | --- |
| `access_token` | Access token | `string` | <div class="required">*</div> |

### Parameters in JSON

|Name|Description|Type|Required|
| --- | --- | --- |
| `password` | Password (Minimum 8 characters, at least one upper case letter, at least one number, at least one special character) | `string` | <div class="required">*</div> |
| `conf_password` | Password (Minimum 8 characters, at least one upper case letter, at least one number, at least one special character) | `string` | <div class="required">*</div> |

### Response Messages

* `200` Success
* `422` Invalid passwords
* `401` Passwords don't match
* `401` Unkown user
