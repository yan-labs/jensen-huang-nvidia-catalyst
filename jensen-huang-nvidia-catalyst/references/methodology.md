# Methodology - reading Jensen Huang / NVIDIA public signals

## Purpose

Classify public Jensen Huang and NVIDIA dynamics by how directly they can move
NVDA, semiconductor suppliers, AI infrastructure stocks, cloud capex names, and
related themes. Rank signals by immediate market reliability and separately
label durability.

## Signal tiers

### Tier 1 - Direct Jensen / NVIDIA primary-source signal

Use when Jensen, NVIDIA Newsroom, Investor Relations, an earnings call, official
keynote, or official transcript gives a concrete statement.

Common subtypes:
- Product-roadmap timing: Blackwell, Rubin, Vera/Rubin, GB200/GB300, NVL,
  Spectrum-X, CUDA, software stack.
- Demand/capacity: supply constrained, sold out, lead times, wafer capacity,
  HBM constraints, networking bottlenecks.
- Customer/platform: named cloud, sovereign AI, enterprise/robotics/auto wins.
- Policy: China/export controls, sovereign AI, country-level AI infrastructure.

Reliability: highest when there is a timestamp, exact quote, product/customer
detail, and a public source link.

### Tier 2 - Confirmed partner/customer/supplier signal

Use when a customer, supplier, regulator, or partner confirms a Jensen/NVIDIA
theme but Jensen himself is not the source.

Examples:
- Cloud capex guidance confirming GPU demand.
- TSMC/HBM/networking capacity comments confirming constraints.
- Dell/Supermicro/HPE/NVIDIA server announcements.
- Government sovereign-AI contracts or export-control actions.

Reliability: high for the affected basket when multiple public sources confirm.

### Tier 3 - Major-media interview / policy / market narrative

Use for credible media interviews, public event reports, and policy headlines
where the quote is visible but not yet in an official transcript.

Reliability: medium. Upgrade if the quote is later confirmed by a transcript or
official NVIDIA page. Downgrade if it is paraphrased or ambiguous.

### Tier 4 - Social / rumor / clip lead

Use only for lead generation. Do not score as confirmed until date, source,
speaker, and context are verified.

## Market mapping

## Supply-chain overlay - mandatory

For every market-relevant Jensen/NVIDIA item, answer these before producing a
final read:

1. **What part of the stack changed?** Product roadmap, demand, supply, policy,
   customer capex, server integration, networking, memory, power, or cooling.
2. **Where is the bottleneck?** Foundry/CoWoS, HBM, networking/optics, server
   assembly, power/cooling, export licenses, or customer capex.
3. **Who confirms it?** Official NVIDIA, customer, supplier, integrator,
   regulator, trade press, or social lead.
4. **Who benefits first and second?** NVDA first only when economics accrue to
   NVIDIA; otherwise map the affected supplier/customer basket.
5. **What would invalidate it?** Supplier denial, capacity overbuild, export
   restriction, customer capex cut, integration delay, margin compression, or
   product slip.

Do not raise confidence above medium unless at least one customer, supplier,
integrator, policy, or official NVIDIA source corroborates the supply-chain
implication.

**NVDA primary**
- Product roadmap, demand, gross-margin implications, export controls, customer
  wins, sovereign AI, software/CUDA moat.

**AI server / OEM / integrators**
- DELL, SMCI, HPE, Lenovo, WDC/STX secondary when storage is part of AI factory.

**Semiconductor suppliers**
- TSM for foundry capacity; ASML for advanced lithography; ARM for CPU/IP; AVGO
  and MRVL for networking/custom silicon; MU/Samsung/SK Hynix for HBM/memory.

**Networking and data-center infrastructure**
- ANET, VRT, ETN, CEG, VST, NRG, GE Vernova, Schneider/ABB equivalents where
  available, depending on power/cooling/networking language.

**Cloud / customer capex**
- MSFT, GOOGL, AMZN, META, ORCL, TSLA, CoreWeave when demand or capex is named.

**Policy / China**
- NVDA first; AMD/INTC second-order; Chinese AI hardware/software names only as
  context unless the user's account can trade them.

## Amplifiers

Add conviction when several stack:

1. Exact Jensen quote or official NVIDIA source.
2. Named product generation and launch/timing detail.
3. Named customer, country, supplier, or contract.
4. Verifiable capacity number, revenue guide, order book, or shipment timing.
5. Same theme confirmed by customer/supplier/policy source within the same week.
6. Posted during market hours or just before a major event/earnings.
7. Connects to a known bottleneck: HBM, CoWoS, networking, power, cooling,
   packaging, export licenses.
8. Identifies a supply-chain beneficiary or pressure point beyond NVDA.

## Anti-patterns

Do not over-score:

- Generic "AI is early" vision statements without new details.
- Old clips reposted as current.
- Unsourced Chinese-language summaries without event/date.
- Product hype after the stock has already priced the event.
- Competitor or supply-chain rumors without primary confirmation.
- Paywalled headlines that hide the actual quote or context.
- NVDA-only conclusions that ignore the obvious supply-chain beneficiary,
  bottleneck, or customer-capex read.

## Output shape

Use this compact format:

```text
Signal: <date/time, source, link>
Summary: <one-line public fact>
Tier: <1/2/3/4> | Type: <product/demand/supply/policy/customer/etc.>
Likely movers: <primary assets> | Secondary: <baskets>
Supply chain: <bottleneck / beneficiary / confirmation source>
Reliability: <high/medium/low> | Duration: <intraday/1-3d/1-2w/structural>
Why it may work: <amplifiers>
Why it may fail: <anti-patterns/invalidation>
Data caveat: <source/quote/price freshness>
```

## Scoring outcomes

- For confirmed market-relevant signals, record initial reaction and T+1w
  durability when practical.
- Use public quote sources with provider and timestamp. Do not call data
  broker-authoritative.
- A hit means the expected direction showed up in the stated window. Record
  magnitude separately.
- Preserve misses. They are the guardrail against overfitting Jensen hype.
