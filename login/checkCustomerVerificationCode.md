# Check customer's verification code

<div class="method method-post">POST</div> <span class="url">https://app.ewill.io/server/api/customers/me/checkCustomerVerificationCode</span>

> Check customer's verification code to verify the account

### Parameters in JSON

|Name|Description|Type|Required|
| --- | --- | --- |
| `email` | Email address | `string` | <div class="required">*</div> |
| `inviteCode` | Verfication code | `string` | <div class="required">*</div> |

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
    "gRecaptchaResponse": "03AHqfIOnZwBQQuahMH4-MAGhwU7Sy55nTn5Dwz4z-WRBin2BopSK8VExRk01NRmR8Gqghe2QH5PeVAaDJ_HbXrFUwM1gi7gSJtMIOC1SPEeYjqwpvrL2co-i2wDeTzQLpYhvqCI0E5G1CXvMB0JEYTyxNkonrHub9KdRVxXhrLFIR8JtCeQu82sBZxOyw3HmhGSpIHrH70JLBVMxaUVdrQfMhX4a0zPApvN69eHpjFSsXvn8OyEBk1UNnhQW1cpS5I1nFn59wMiXDYmCxVy5dXqt-_PYT2RsHtA",
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
* `401` Authorization required
* `401` Verification code failed
* `500` Error
