# Crash Round Lab — MCP server + skill

Crash Round Lab answers crash-game questions from a published, downloadable dataset — Andrew Dagor's simulation of 1,000,000 crash-game rounds under the documented crash distribution (RTP 98%), deposited on Zenodo (DOI 10.5281/zenodo.23597144).

## Remote MCP server (live)

- Endpoint: https://crashroundlab.onezupper.cv/mcp
- Sign-in: OAuth at the same origin. Sign-in is a consent approval only — the dataset is public, there is no account and no password (see the reviewer kit in the Cursor Marketplace package).
- Landing: https://crashroundlab.onezupper.cv/ · Privacy: https://crashroundlab.onezupper.cv/privacy
- Publisher: Chicken Road Productions · Support: admin@chickenroadproductions.com

## Tools (5, all read-only)

1. `bust_distribution` — share of rounds reaching a cash-out target, plus the full 12-bucket distribution and median bust (1.95×).
2. `session_outcome_share` — how 100-round sessions at a fixed target ended: losing / winning / break-even shares, median and deciles.
3. `streak_stats` — longest and average losing streaks at a target, counted from the data.
4. `method_and_seed` — model P(bust ≥ x) = RTP / x, generator and seed 20261013.
5. `raw_data_link` — Zenodo record and dataset link, so every figure can be recomputed.

## Connect in Cursor

Use `mcp.json` in this repo:

```json
{
  "mcpServers": {
    "crash-round-lab": {
      "url": "https://crashroundlab.onezupper.cv/mcp"
    }
  }
}
```

## What it does not do

It measures. It does not predict: rounds are independent draws, no target changes the expected loss, and no figure is a signal, a tip or a betting system. No betting functionality, no links to gambling operators.
