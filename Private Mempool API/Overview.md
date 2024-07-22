---
order: 102
icon: project-roadmap
iconAlign: left   
---

The private mempool API can be used to access non-standard transaction processing and frontrunning protection.

Unlike the public mempool, the hashrate available for block inclusion (confirmation) is expected to be a small subset of the total global hashrate. In addition, premium fee rate is expected to be applied. This makes using this service highly undesirable for transactions which are not non-standard nor require frontrunning protection.

Actual block inclusion cannot be guaranteed, however it is possible to timeout or fully cancel a submitted transaction. 


---

## :warning: Status: in active development

---

## Endpoints

| Network             | URL          |
|---------------------|--------------|
| Mainnet             | Coming Soon  |

| Test Network                     | URL          |
|----------------------------------|--------------|
| Mock API (for integration tests) | Coming Soon  |
| Mainnet beta (no mining)         | Coming Soon  |
| Testnet3                         | Coming Soon  |
| Testnet4                         | Coming Soon  |
| Signet (custom)                  | Coming Soon  |
