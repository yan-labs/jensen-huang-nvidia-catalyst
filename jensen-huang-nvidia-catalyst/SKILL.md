---
name: jensen-huang-nvidia-catalyst
description: >
  Decision-support lens for tracking Jensen Huang / Huang Renxun / 黄仁勋 public
  dynamics across NVIDIA official sources, interviews, events, major media,
  policy headlines, customer/supplier signals, and market reactions. Use this
  skill when the user mentions Jensen Huang, NVIDIA CEO, NVDA, Blackwell, Rubin,
  CUDA, AI factories, sovereign AI, GPU export controls, China chips, DGX,
  GB200/GB300, NVL, Spectrum-X, InfiniBand, robotics, HBM, TSMC capacity, or asks
  what a Jensen/NVIDIA public signal means for NVDA, semiconductor suppliers,
  data-center infrastructure, AI power, cloud capex, or related US stocks.
  Decision-support only; never auto-trades and never places, amends, sizes, or
  cancels orders.
---

# Jensen Huang / NVIDIA Catalyst Lens

## Overview

Use this lens to turn public Jensen Huang and NVIDIA dynamics into calibrated
short-horizon market context. Treat the output as decision support, not a trade
instruction or long-term thesis.

## Step 0 - Refresh First

Jensen signals come from many places, not one canonical feed.

1. Pull the latest `yan-labs/jensen-huang-nvidia-catalyst` repo.
2. Load `references/source-map.md` and check the relevant official NVIDIA source
   first: Newsroom, Blog, Investor Relations, events, YouTube/on-demand, or SEC.
3. Search recent web/news for the user's topic and for fresh broad terms:
   `Jensen Huang NVIDIA interview`, `黄仁勋 英伟达 最新`, `Jensen Huang export
   controls`, `NVIDIA Blackwell Rubin`, `NVIDIA sovereign AI`, and related
   ticker/theme terms.
4. Dedupe any new item against `data/sightings.json` and
   `references/track-record.md`.
5. Never call an item "latest" unless the timestamp/source was observed in the
   current run.

## Core Workflow

1. Load `references/methodology.md` to classify the signal tier and affected
   market basket.
2. Load `references/source-map.md` to choose source reliability and follow-up
   searches.
3. Load `references/track-record.md` to weight the signal by observed base rate.
4. Output timestamp, source, link, signal type, affected assets, likely
   direction, reliability, duration, invalidation trigger, and data caveats.
5. Keep broker/account language separate: public news and public quotes are
   market context only, never uSMART account truth or fill confirmation.

## Navigation

| File | Use it for |
|---|---|
| `references/source-map.md` | Source hierarchy, search queries, official URLs, and source-specific caveats |
| `references/methodology.md` | Signal tiers, ticker/theme mapping, amplifiers, anti-patterns, output shape |
| `references/track-record.md` | Live ledger, seed priors, and hit-rate calibration rules |
| `references/maintenance.md` | Scheduled refresh, dedupe, scoring, and commit convention |
| `../data/sightings.json` | Public-dynamics archive when using the full repo checkout |

## Risk Framing

- State that the analysis is decision support only and not financial advice.
- Separate "can move NVDA today" from "is a durable investment thesis."
- Label sources by reliability; do not treat rumors or unsourced social clips as
  confirmed Jensen statements.
- Distinguish product-cycle demand, policy risk, customer capex, and supplier
  capacity. They move different baskets.
- Never place, amend, cancel, or size trades from this skill.

