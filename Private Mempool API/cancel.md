---
order: 97
label: cancel
icon: code
iconAlign: left      
---

# cancel

The `cancel` RPC method cancels previously submitted transaction.

### Request body example

```json
{
  "jsonrpc": "2.0",
  "id": 1,
  "method": "send_raw_transaction",
  "params": {
    "tx_id": "0x……ff" // Transaction ID (TXID) hex-encoded string
  }
}
```


+++ CURL
```
curl -s --data '{"jsonrpc": "2.0","id": "1","method": "cancel","params": {"tx_id": "0x……ff"}' -H "Content-Type: application/json" -H "Authorization: Bearer ${TOKEN}" -X POST ${URL}```
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
  "result": "ok"
}
```
