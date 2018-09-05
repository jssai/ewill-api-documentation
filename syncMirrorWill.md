# Sync mirror will

<div class="method method-post">POST</div> <span class="url">https://app.ewill.io/server/api/customers/me/syncMirrorWill</span>

> Sync mirror will between partners

### Parameters in JSON

|Name|Description|Type|Required|
| --- | --- | --- |
| `partnerFullName` | Partner's full name | `string` | <div class="required">*</div> |
| `partnerEmail` | Partner's email address | `string` | <div class="required">*</div> |
| `willId` | ID of the will | `string` | <div class="required">*</div> |
| `referenceId` | Reference of the will | `string` | <div class="required">*</div> |

### Response Example

```json
{
    "lastName": "Doe",
    "email": "jane.doe@gmail.com",
    "fullLegalName": "Jane Doe",
    "firstName": "Jane",
    "customerNumber": "AV-22222222",
    "emailVerified": true,
    "id": "YYYYYYYYYYYYYYYYYYYYYYYY",
    "isCustomerCodeVerified": true,
    "deviceID": "1268624223Chrome",
    "deviceName": "Chrome",
    "deviceType": "Browser",
    "deviceOS": "Mac/iOS",
    "createdAt": "2018-01-01T12:00:00.000Z",
    "lastLoggedIn": "2018-01-01T12:00:00.000Z",
    "userId": "YYYYYYYYYYYYYYYYYYYYYYYY",
    "ttl": 1209600,
    "loggedInCount": 1,
    "policies": [],
    "warranties": [],
    "assets": [],
    "dependents": [],
    "beneficiaries": [],
    "claims": [],
    "wishlists": [],
    "wills": [],
    "etrusts": []
}
```

### Response Messages

* `200` Success
* `401` Authorization required
* `500` Error
