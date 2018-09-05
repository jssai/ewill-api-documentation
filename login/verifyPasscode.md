# Verify passcode

<div class="method method-post">POST</div> <span class="url">https://app.ewill.io/server/api/customers/verifyPasscode</span>

> Verify passcode for two factor authentication

### Parameters in JSON

|Name|Description|Type|Required|
| --- | --- | --- |
| `email` | Email address | `string` | <div class="required">*</div> |
| `password` | Password | `string` | <div class="required">*</div> |
| `verificationCode` | 6 digits code | `string` | <div class="required">*</div> |
| `deviceID` | Device ID | `string` | <div class="required">*</div> |
| `deviceName` | Device Name | `string` | <div class="required">*</div> |
| `deviceOS` | Device OS | `string` | <div class="required">*</div> |
| `deviceType` | Device type | `string` | <div class="required">*</div> |

### Response Example

```json
{
    "lastName": "Doe",
    "email": "john.doe@gmail.com",
    "fullLegalName": "John Doe",
    "firstName": "John",
    "customerNumber": "AV-11111111",
    "emailVerified": true,
    "id": "XXXXXXXXXXXXXXXXXXXXXXXX",
    "isCustomerCodeVerified": true,
    "deviceID": "1268624223Chrome",
    "deviceName": "Chrome",
    "deviceType": "Browser",
    "deviceOS": "Mac/iOS",
    "createdAt": "2018-01-01T12:00:00.000Z",
    "lastLoggedIn": "2018-01-01T12:00:00.000Z",
    "accessToken": "XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX",
    "userId": "XXXXXXXXXXXXXXXXXXXXXXXX",
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
* `401` Verification code rejected
