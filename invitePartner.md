# Invite partner

<div class="method method-post">POST</div> <span class="url">https://app.ewill.io/server/api/customers/me/invitePartner</span>

> Send an invite to partner to his/her email address

### Parameters in JSON

|Name|Description|Type|Required|
| --- | --- | --- |
| `partnerFullName` | Partner's full name | `string` | <div class="required">*</div> |
| `partnerEmail` | Partner's email address | `string` | <div class="required">*</div> |
| `willId` | ID of the will | `string` | <div class="required">*</div> |
| `referenceId` | Reference of the will | `string` | <div class="required">*</div> |

### Response Messages

* `200` Success
* `401` Authorization required
* `400` Unkown partner
* `500` Error
