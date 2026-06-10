---
name: btc-node
title: "IRONCLAW — BTC Settlement Node"
description: "Bitcoin blockchain data, address portfolio, transaction tracing, fee forecasting, whale monitoring, SEC EDGAR filings, URL scraping, AI summarization, and Reddit API — all served from a real Bitcoin Core full node with x402 micropayments."
use_case: "Use for Bitcoin fee estimates, mempool status, block/tx lookup, address portfolio analysis, transaction taint tracing, whale alerts, SEC insider trades, web scraping, and AI summarization — all payable with USDC via x402."
category: data
service_url: https://btcnode.uk
openapi:
  path: openapi.json
---

IRONCLAW BTC Node delivers real Bitcoin Core full node data through 15+ endpoints — mempool, fees, blocks, transactions, address portfolio, transaction tracing, fee forecasting, whale alerts, SEC insider trades, web scraping, AI summarization, and Reddit API — all via x402 micropayments.

No API key, no account, no subscription. Pay per request with USDC and get real data from a live Bitcoin full node.

x402 USDC payment currently accepted on **Base mainnet** (eip155:8453). Solana mainnet support is planned.

## Spend-aware usage

- **Start with `/api/info` or `/api/fees`** for the cheapest calls ($0.003 each) when you need a quick pulse check on the Bitcoin network.
- **Use `/api/tx/{hash}`** for single-transaction lookups ($0.005) — returns confirmations, inputs, outputs, and value in one call.
- **Use `/api/addr/{address}`** for full address portfolio ($0.005) — balance, UTXOs, recent transaction history.
- **Use `/api/trace/{txid}`** for compliance or forensic analysis ($0.008) through 2 hops of fund tracing.
- **Use `/api/whales`** ($0.005) to monitor large fund movements in real-time — pass `min_btc` and `limit` to narrow results.
- **Use `/api/fees/predict`** ($0.005) for fee forecasting before broadcasting a Bitcoin transaction.
- **Use `/api/sec/insider/{ticker}`** ($0.003) for SEC Form 4/3/5 insider trades without an EDGAR API key.
- **Prefer `/api/scrape`** ($0.003) over `/api/summarize` ($0.003) when you only need raw text — both cost the same but scrape returns full content.
- **Use Reddit endpoints** ($0.003 each) for social sentiment — `hot/{subreddit}`, `search`, `comments/{postId}`, and `trending`.
