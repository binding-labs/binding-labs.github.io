---
order: 97
label: get_status
icon: code
iconAlign: left      
---

# get_status

The `get_status` RPC method provides status about a previously-submitted transaction.

| Name    | Type     | Description                                          |
|---------|----------|------------------------------------------------------|
| `tx_id` | `String` | Transaction ID (TXID) in hex-encoded string format.  |

### Request body example
```json
{
  "jsonrpc": "2.0",
  "id": 1,
  "method": "get_status",
  "params": {
    "tx_id": "0x……ff"
  }
}
```

+++ CURL
```
curl -s --data '{"jsonrpc": "2.0","id": "1","method": "get_status","params": {"tx_id": "0x……ff"}' -H "Content-Type: application/json" -H "Authorization: Bearer ${TOKEN}" -X POST ${URL}```
```
+++ Javascript
Coming soon
+++ Go
Coming soon
+++ Rust
Coming soon
+++
### Response body example

Coming soon 