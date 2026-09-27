# 0nceApp discovery

Publishes the Nym address of the 0nceApp discovery server for new clients:

```
GET https://api.0nce.root64.de/api/v1/address
→ {"address": "<id>.<key>@<gateway>"}
```

The client fetches it through the Nym mixnet on first start and stores it.
Update `api/v1/address` only when the server's Nym address changes (loss of
its Nym storage or a gateway change).
