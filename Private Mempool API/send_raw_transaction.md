---
order: 98
label: send_raw_transaction
icon: code
iconAlign: left      
---

# send_raw_transaction

The `send_raw_transaction` RPC method submits a raw transaction.

Both Replace by Fee (RBF) and Child Pays for Parent (CPFP) are supported.

### Parameters

| Name               | Type     | Description                                             |
|--------------------|----------|---------------------------------------------------------|
| `tx`               | `String` | Signed raw transaction in hex-encoded string format.    |
| `max_block_height` | `Number` | Max block height to attempt inclusion, cancel otherwise |


### Request body example

```json
{
  "jsonrpc": "2.0",
  "id": 1,
  "method": "send_raw_transaction",
  "params": {
    "tx": "0x……ff",
    "max_block_height": 852971
  }
}
```


+++ CURL
```
curl -s --data '{"jsonrpc": "2.0","id": "1","method": "send_raw_transaction","params": {"tx": "0x……ff","max_block_height":852971}' -H "Content-Type: application/json" -H "Authorization: Bearer ${TOKEN}" -X POST ${URL}```
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
