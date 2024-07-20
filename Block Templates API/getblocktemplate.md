---
order: 100
label: get_block_template
icon: code
iconAlign: left      
---

The `get_block_template` RPC method exposes a non-canonical, potentially higher-value block template.

### Request body example
```json
{
  "jsonrpc": "2.0",
  "id": 1,
  "method": "get_block_template"
}
```
 
+++ CURL
```
curl -s --data '{"jsonrpc": "2.0","id": "1","method": "get_block_template"' -H "Content-Type: application/json" -H "Authorization: Bearer ${TOKEN}" -X POST ${URL}```
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
