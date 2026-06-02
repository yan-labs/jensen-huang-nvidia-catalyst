# Track record - live catalyst ledger

## Purpose

Measure whether Jensen Huang / NVIDIA public signals actually move NVDA and the
AI-infrastructure basket, instead of assuming every quote has edge. Keep this
file append-only once the timer starts.

## Calibration takeaways

- **Most reliable immediate signals:** exact Jensen/NVIDIA primary-source
  comments about product timing, demand, capacity constraints, and named
  customers.
- **Most durable signals:** customer capex + supplier capacity + NVIDIA product
  roadmap all confirming the same theme.
- **Most fade-prone signals:** generic AI-optimism quotes, social clips without
  date/context, and trade-press product hype after a known keynote.
- **Highest policy risk:** China/export-control comments. These can move NVDA
  sharply but need regulatory confirmation.

## Live sightings archive

`data/sightings.json` and `data/sightings.csv` store public items found by the
timer, including items that are not worth adding to the market ledger.

## Live market ledger

Append new confirmed market-relevant signals above this marker after each
refresh.

| Signal UTC | Source/link | Summary | Tier/type | Assets | Prediction | T+1d result | T+1w result | Hit? | Notes |
|---|---|---|---|---|---|---|---|---|---|
| 2026-06-01 01:00 | [NVIDIA GTC 2026 keynote](https://www.nvidia.com/gtc/keynote/?nvid=nv-int-bnr-839023) + [RTX Spark/Microsoft release](https://nvidianews.nvidia.com/news/nvidia-microsoft-windows-pcs-agents-rtx-spark) | Jensen/NVIDIA framed AI factories, agentic systems, physical AI, robotics, and RTX Spark Windows PCs as the new personal AI computer | Tier 1 product/event + customer ecosystem; amps: official source, exact product, Microsoft/OEM partners, Blackwell/Grace/CUDA stack | NVDA primary; MSFT/ARM/DELL/HPQ and AI-PC ecosystem secondary | NVDA and AI-PC/agentic-PC basket up or narrative-strengthening over 1-2w; durability depends on partner follow-through and broader AI risk appetite |  |  |  | Initial primary-source seed row from repo creation. |
| TIMER_LEDGER_START |  |  |  |  |  |  |  |  |  |

## Rolling hit-rate

| Pattern | Calls logged | Directional hits | T+1w held | Notes |
|---|---:|---:|---:|---|
| Tier 1 product roadmap | 0 | 0 | 0 | Seed empty; fill from timer. |
| Tier 1 demand/capacity | 0 | 0 | 0 | Seed empty; fill from timer. |
| Tier 2 customer/supplier confirmation | 0 | 0 | 0 | Seed empty; fill from timer. |
| Tier 3 policy/export-control | 0 | 0 | 0 | Seed empty; fill from timer. |
| Tier 4 social/rumor lead | 0 | 0 | 0 | Do not count until verified. |

## Scoring rules

- Score only confirmed public items with source, timestamp, URL, and affected
  asset list.
- Use public quotes only as market context and label provider/timestamp.
- Define a hit as the predicted direction showing up over the expected window.
- Record durability separately. A keynote spike that fully fades is not a
  durable hit.
- Do not rewrite history. Corrections should be appended in Notes.
