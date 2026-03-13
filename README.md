# Pyth Pro — Cursor Plugin

Real-time and historical market data from [Pyth](https://pyth.network) — 2000+ price feeds across crypto, equities, FX, metals, commodities, and more.

## What you get

- **MCP server** auto-connected — Cursor's agent can call Pyth tools directly (search feeds, get prices, fetch OHLC data)
- **Rules** encoding Pyth conventions (symbol formats, display prices, API limits)
- **9 skills** for common market data workflows

## Install

Search for `pyth-pro` in the Cursor Marketplace, or add it manually.

## MCP Tools

The plugin connects to `https://mcp.pyth.network/mcp` and provides:

| Tool | Description | Auth Required |
|------|-------------|---------------|
| `get_symbols` | Search and list available price feeds | No |
| `get_latest_price` | Real-time prices for one or more feeds | Yes (access token) |
| `get_historical_price` | Point-in-time price snapshots | No |
| `get_candlestick_data` | OHLC candlestick bars for charting and analysis | No |

Get an access token at [pyth.network/pricing](https://pyth.network/pricing). Only `get_latest_price` requires one.

## Skills

| Skill | Use when... |
|-------|-------------|
| **Alert Conditions** | "Is BTC above $100k?", "Has ETH dropped 5% today?" |
| **Cross-Asset Comparison** | "Compare Bitcoin vs Gold this quarter" |
| **Data Export** | "Export BTC daily OHLC as CSV" |
| **Funding Rate Monitor** | "What's the BTC funding rate?" |
| **FX Converter** | "Convert 1000 EUR to JPY", "5 BTC in EUR" |
| **Integration Helper** | "How do I use Pyth?", "What's the feed ID for AAPL?" |
| **Portfolio Tracker** | "Track my 2 BTC and 50 ETH" |
| **Time-Series Snapshots** | "BTC price at the start of each month" |
| **Volatility Analysis** | "How volatile is SOL?", "Compare BTC vs AAPL volatility" |

## Example queries

Try these in Cursor's agent:

- "What's the current price of Bitcoin?"
- "Compare ETH vs SOL performance over the last 30 days"
- "Export gold daily prices for the past month as CSV"
- "Convert 10,000 USD to EUR"
- "What are the top funding rates right now?"
- "Track a portfolio of 2 BTC, 100 ETH, and 5000 SOL"

## Links

- [Pyth Pro Documentation](https://docs.pyth.network/price-feeds/pro)
- [Get an Access Token](https://docs.pyth.network/price-feeds/pro/acquire-access-token)
- [Pricing](https://pyth.network/pricing)
- [GitHub — MCP Server](https://github.com/pyth-network/pyth-crosschain/tree/main/apps/mcp)
