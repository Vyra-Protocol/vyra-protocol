# x402 — Payment Required (on-chain)

Servers may respond with HTTP 402 including a JSON bill:

```json
{
  "protocol": "x402",
  "chain": "solana",
  "amount": "0.01",
  "memo": "article_42"
}
