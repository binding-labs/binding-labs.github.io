---
order: 99
label: get_estimation
icon: code
iconAlign: left      
---

# get_estimation

The `get_estimation` RPC method provides the estimated confirmation time (in block intervals) for a given transaction, given its fee and the current available hashrate. 

### Parameters

| Name | Type     | Description                                          |
|------|----------|------------------------------------------------------|
| `tx` | `String` | Signed raw transaction in hex-encoded string format. |
 

### Request body example

```json
{
  "jsonrpc": "2.0",
  "id": 1,
  "method": "get_estimation",
  "params": {
    "tx": "0x……ff"
  }
}
```


+++ CURL
```
curl -s --data '{"jsonrpc": "2.0","id": "1","method": "get_estimation","params":{"tx":"0x……ff" }' -H "Content-Type: application/json" -H "Authorization: Bearer ${TOKEN}" -X POST ${URL}```
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
    "block_intervals": 38
  }
}
```
