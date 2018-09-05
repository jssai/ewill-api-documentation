# Customer login

<div class="method method-post">POST</div> <span class="url">https://app.ewill.io/server/api/customers/login</span>

> Customer login, returns customer details and access token

### Parameters in JSON

|Name|Description|Type|Required|
| --- | --- | --- |
| `email` | Email address | `string` | <div class="required">*</div> |
| `password` | Password | `string` | <div class="required">*</div> |
| `deviceID` | Device ID | `string` | <div class="required">*</div> |
| `deviceName` | Device Name | `string` | <div class="required">*</div> |
| `deviceOS` | Device OS | `string` | <div class="required">*</div> |
| `deviceType` | Device type | `string` | <div class="required">*</div> |
| `gRecaptchaResponse` | Google Recaptcha response | `string` | <div class="required">*</div> |


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
* `422` Missing or invalid fields
* `423` Verification required
* `404` Captcha error
