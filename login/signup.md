# Customer signup

<div class="method method-post">POST</div> <span class="url">https://app.ewill.io/server/api/customers/signup</span>

> Sign up a new customer, returns customer details

### Parameters in JSON

|Name|Description|Type|Required|
| --- | --- | --- |
| `email` | Email address | `string` | <div class="required">*</div> |
| `password` | Password (Minimum 8 characters, at least one upper case letter, at least one number, at least one special character) | `string` | <div class="required">*</div> |
| `firstName` | Firstname | `string` | <div class="required">*</div> |
| `lastName` | Lastname | `string` | <div class="required">*</div> |
| `fullLegalName` | Full name | `string` | <div class="required">*</div> |
| `deviceID` | Device ID | `string` | <div class="required">*</div> |
| `deviceName` | Device Name | `string` | <div class="required">*</div> |
| `deviceOS` | Device OS | `string` | <div class="required">*</div> |
| `deviceType` | Device type | `string` | <div class="required">*</div> |
| `gRecaptchaResponse` | Google Recaptcha response | `string` | <div class="required">*</div> |


### Response Example

```json
{
    "lastName": "John",
    "firstName": "Doe",
    "email": "john.doe@gmail.com",
    "fullLegalName": "John Doe",
    "customerNumber": "AV-11111111",
    "id": "XXXXXXXXXXXXXXXXXXXXXXXX",
    "isCustomerCodeVerified": true,
    "deviceID": "1268624223Chrome",
    "deviceName": "Chrome",
    "deviceType": "Browser",
    "deviceOS": "Mac/iOS",
    "gRecaptchaResponse": "03AHqfIOmg42HfQU5yJVMEDEe38e9UhWh1dOnyZKs1B-ZYcvczptnTeUnHDzmnEY2YId6eAYoiu57XT5_rZMQs_9VqstVFEhVmkcP_JNKMmXERc2Gl3PSmwNtqJGpTpJ3KkVHG01nMobBv8u-Rx5dxQB4TFmOmH4ujaX3F51BCImWLzDkB4MJBUFsLT8HUFfb1ESXa5i3xvnDAKpBXlsrAlNrUJq-TRbj88HCfjrjEqvImdOPUI20OPfwe2GOxd6omXlgznTRwNnXkEoPLUjjsErlWnuMiv2u-eg",
    "createdAt": "2018-01-01T12:00:00.000Z"
}
```

### Response Messages

* `200` Success
* `422` Missing or invalid fields
* `404` Captcha error
