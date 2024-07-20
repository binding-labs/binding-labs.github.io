---
order: 99
label: get_estimation
---

# get_estimation

The `get_estimation` RPC method provides the estimated confirmation time (in block intervals) for a given transaction, given its fee and the current available hashrate. 

### Request body example

```json
{
  "jsonrpc": "2.0",
  "id": 1,
  "method": "get_estimation",
  "params": {
    "tx": "0x……ff" // Signed raw tx's hex-encoded string
  }
}
```


+++ CURL
```
curl -s --data '{"jsonrpc": "2.0","id": "1","method": "get_estimation","params":{"tx":"0x……ff" }' -H "Content-Type: application/json" -X POST ${URL}```
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
