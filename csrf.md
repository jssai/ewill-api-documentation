# Get CSRF token

<div class="method method-get">GET</div> <span class="url">https://app.ewill.io/server/api/_csrfToken</span>

> Get CSRF (Cross-Site Request Forgery) token which is need in all requests in the header as follow

```
csrf-token: 9oSHBqtU-CJIChGjMcJIh7octwlm5KUY7GxY
```

### Response Example

```json
{
    "csrfToken": "9oSHBqtU-CJIChGjMcJIh7octwlm5KUY7GxY"
}
```

### Response Messages

* `200` Success
* `500` Error
