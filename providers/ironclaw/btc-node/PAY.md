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

- **Start with `/api/info`, `/api/fees` or `/api/mempool`** for the cheapest calls ($0.001 each) when you need a quick pulse check on the Bitcoin network.
- **Use `/api/tx/{hash}`** for single-transaction lookups ($0.001) — returns confirmations, inputs, outputs, and value in one call.
- **Use `/api/addr/{address}`** for full address portfolio ($0.002) — balance, UTXOs, recent transaction history.
- **Use `/api/trace/{txid}`** for compliance or forensic analysis ($0.005) through 2 hops of fund tracing.
- **Use `/api/whales`** ($0.001) to monitor large fund movements in real-time — pass `min_btc` and `limit` to narrow results.
- **Use `/api/fees/predict`** ($0.001) for fee forecasting before broadcasting a Bitcoin transaction.
- **Use `/api/sec/insider/{ticker}`** ($0.005) for SEC Form 4/3/5 insider trades without an EDGAR API key.
- **Use `/api/scrape`** ($0.001) to extract clean text from any URL; use `/api/agent/scrape` ($0.003) for cached results with 1h SSD retention.
- **Use `/api/summarize`** ($0.001) for AI text summarization.
- **Use `/api/systems-theory`** ($0.01), **`/api/game-theory`** ($0.01), or **`/api/omni-theory`** ($0.03 — all 6 lenses) for deep analysis.
- **Use `/api/capital-flows`** ($0.02) to trace money flows across systems.
- **Use Reddit endpoints** ($0.001 each) for social sentiment — `hot/{subreddit}`, `search`, `comments/{postId}`, and `trending`.
- **Use Agent Surveillance endpoints** for heavier analysis — address surveillance ($0.05), whale alerts ($0.02), coin taint ($0.10), Barbarian API ($0.01), agent scrape ($0.003).
