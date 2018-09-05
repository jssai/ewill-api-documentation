# Send will to email address

<div class="method method-post">POST</div> <span class="url">https://app.ewill.io/server/api/consumers/me/emailCopy</span>

> Send customer's will to email address

### Parameters in JSON

|Name|Description|Type|Required|
| --- | --- | --- |
| `subject` | Email subject | `string` | <div class="required">*</div> |
| `recipients` | List of email addresses | `Array<string>` | <div class="required">*</div> |
| `message` | Email body | `string` | <div class="required">*</div> |
| `willId` | Will ID | `string` | <div class="required">*</div> |

### Response Messages

* `401` Authorization required
* `204` Success
* `500` Error
