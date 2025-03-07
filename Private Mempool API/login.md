---
order: 101
label: login
icon: code
iconAlign: left      
---

The `login` RPC method initiates an authenticated session using a JSON Web Token (JWT). Subsequent requests should include the returned JWT in the request headers (Authorization header).

For signup inquiries, please contact us via onboard@bindinglabs.io

### Parameters

| Name       | Type     | Description |
|------------|----------|-------------|
| `user`     | `String` | Username    |
| `password` | `String` | Password    |

### Request body example
```json
{
  "jsonrpc": "2.0",
  "id": 1,
  "method": "login",
  "params": {
    "username": "user",
    "password": "pw"
  }
}
```

+++ CURL
```
curl -s --data '{"jsonrpc": "2.0","id":"1","method":"login","params":{"username":"user","password":"pw"}}' -H "Content-Type: application/json" -X POST ${URL}```
```
+++ Javascript
Coming soon
+++ Go
Coming soon
+++ Rust
Coming soon
+++
### Response body example

```json
{
  "jsonrpc": "2.0",
  "id": 1,
  "error": null,
  "result": {
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiJleGFtcGxlVXNlciIsImlhdCI6MTYzMDY1NjYzNCwiZXhwIjoxNjMwNjYwMjM0fQ.FOY1MnB3oJD7j5l5So9VKdIb4mmbN6x5NkAvGz1gn1k"
  }
}
```

