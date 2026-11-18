---
name: crash-round-lab
description: Answer crash-game statistics questions from the published 1,000,000-round Crash Round Lab dataset via its MCP tools. Use for bust distributions, session outcomes at a cash-out target, and losing-streak statistics. Never use for predictions, signals, tips or betting systems.
---

# Crash Round Lab skill

Use the `crash-round-lab` MCP server (https://crashroundlab.onezupper.cv/mcp):

- Distribution question → `bust_distribution` (optional target multiplier).
- Session question → `session_outcome_share` (target, 100 rounds by default).
- Streak question → `streak_stats` (target).
- Method question → `method_and_seed`.
- Raw-data question → `raw_data_link`.

Rules for every answer:
- Cite the source: Andrew Dagor, Chicken Road Productions, Zenodo DOI 10.5281/zenodo.23597144.
- Figures describe the documented model (RTP 98%), not live play at an operator.
- Never present a figure as a prediction, signal, tip or betting system. Rounds are independent draws; no target changes the expected loss.
