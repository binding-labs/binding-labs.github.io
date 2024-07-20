---
order: 100
label: get_status
icon: code
iconAlign: left      
---

# get_status

The `get_status` RPC method provides the latest available information on:
* Current available hashrate.
* Current number of pending transactions awaiting confirmation.
* Minimum acceptable transaction fee (sat/byte).
* Recommended transaction fee (sat/byte) for timely confirmation given the current available hashrate.

### Request body example
```json
{
  "jsonrpc": "2.0",
  "id": 1,
  "method": "get_status"
}
```

+++ CURL
```
curl -s --data '{"jsonrpc": "2.0","id": "1","method": "get_status"' -H "Content-Type: application/json" -H "Authorization: Bearer ${TOKEN}" -X POST ${URL}```
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
    "available_hashrate": 0.02,
    "pending_transactions": 47,
    "minimum_fee": 100,
    "recommended_fee": 120
  }
}
```
