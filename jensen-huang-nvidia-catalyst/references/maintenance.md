# Maintenance playbook

## Purpose

Keep the Jensen Huang / NVIDIA catalyst lens current by tracking public dynamics,
deduping sightings, classifying market-relevant signals, and scoring outcomes.

## Scheduled run

1. Pull the skill repository first with fast-forward only.
2. Read `source-map.md`, `methodology.md`, and `track-record.md`.
3. Check official NVIDIA sources first: Newsroom, Blog, Investor Relations,
   Events/GTC/On-Demand, YouTube, and SEC EDGAR.
4. Run recent web/news searches from `source-map.md`, in both English and
   Chinese, for the last 24 hours and last 7 days.
5. Add new public items to `data/sightings.json` and `data/sightings.csv`,
   deduping by canonical URL first, then by normalized title + date.
6. Update `data/source_stats.txt`.
7. Classify each market-relevant item with `methodology.md`.
8. Append confirmed tradable signals above `TIMER_LEDGER_START` in
   `track-record.md`.
9. Score matured rows after one trading day and one week where public quote data
   is available.
10. Update calibration takeaways only when measured evidence changes the base
    rate for a pattern.

## Sightings fields

Store compact records:

```json
{
  "date_utc": "2026-06-03T00:00:00Z",
  "source": "NVIDIA Newsroom",
  "url": "https://...",
  "title": "...",
  "summary": "...",
  "signal_type": "product|demand|supply|policy|customer|event|other",
  "primary_assets": ["NVDA"],
  "secondary_assets": ["TSM", "MU"],
  "confidence": "high|medium|low",
  "notes": "why it matters / why skipped"
}
```

## Commit hygiene

- Keep `.local/` ignored unless the user explicitly asks otherwise.
- Commit tracked updates only after confirming no secrets, account identifiers,
  screenshots, broker statements, cookies, or `.env` data are staged.
- Use public facts only: official NVIDIA pages, public interviews, public
  filings, public quotes, public policy documents, public customer/supplier
  disclosures, and public news.
- Do not commit paywalled article text, private transcripts, private screenshots,
  or broker data.

## Commit convention

- `data: jensen catalyst sightings update (+<n>) <UTC ISO>` for sightings-only
  updates.
- `data: jensen catalyst ledger update (+<n> signals) <UTC ISO>` when market
  ledger rows are added or scored.
- `skill: jensen catalyst calibration update <UTC ISO>` when methodology or
  calibration changes.
- Do not create empty commits.

## Notification rules

Notify only when:

- new sightings are archived and pushed;
- market ledger rows are appended or scored;
- calibration changes;
- a repeated data-source failure needs user action.

For no-change runs, already-known items, low-quality social leads, or ordinary
successful checks with no durable update, return heartbeat DONT_NOTIFY XML only.

