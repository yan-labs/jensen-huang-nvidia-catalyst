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
| 2026-05-31 00:00 | [NVIDIA DSX AI-factory playbook](https://nvidianews.nvidia.com/news/nvidia-dsx-gives-infrastructure-builders-the-playbook-for-ai-factories) + [DSX platform page](https://www.nvidia.com/en-au/data-center/products/dsx/) | NVIDIA announced DSX as an AI-factory design, simulation and operations platform connecting compute, networking, energy, power and cooling signals | Tier 1 AI-factory infrastructure / supply-chain platform; amps: official source, named cloud builders, named OEM/ODM partners, explicit power/cooling/facility layer | NVDA primary; CRWV/IREN/NBIS/Lambda/Nscale, DELL/HPE/SMCI/LNVGY/Taiwan ODMs, CDNS/Siemens/PTC secondary | NVDA AI-factory platform narrative up; strongest secondary read-through to AI-cloud buildout and power/cooling/facility software names if partner deployments translate into capacity coming online | NVDA +6.3%; AI-infra/cloud basket avg +8.8%, med +9.2% on 2026-06-01 vs 2026-05-29 close; Yahoo Finance daily chart API fetched 2026-06-02T20:50Z |  | hit | Supply-chain confirmation attempts: NVIDIA DSX product page and GTC Taipei MGX/800 VDC live-blog section; watch whether DSX Flex/OS turns into measurable utilization or power-constraint mitigation. |
| 2026-06-01 00:00 | [Vera Rubin full production](https://nvidianews.nvidia.com/news/vera-rubin-full-production-agentic-ai-factory) + [GTC Taipei supply-chain live blog](https://blogs.nvidia.com/blog/nvidia-gtc-taipei-computex-2026-news/) | NVIDIA framed Vera Rubin as a full-production AI-factory platform spanning compute, CPU, storage, networking, power and cooling | Tier 1 demand/capacity; amps: official source, full-production timing, supply-chain scale, power/cooling detail | NVDA primary; DELL/HPE/SMCI/LNVGY/Taiwan ODMs/HBM suppliers/power and cooling secondary | NVDA and AI-infrastructure basket up or narrative-strengthening over 1d-1w; durable only if HBM/advanced packaging, OEM capacity and power/cooling confirmations keep lining up | NVDA +6.3%; AI-infra/OEM basket avg +8.8%, med +9.2%; power/cooling sample mixed on 2026-06-01 vs 2026-05-29 close; Yahoo Finance daily chart API fetched 2026-06-02T20:50Z |  | hit | Supply-chain confirmation attempts: Foxconn Computex release, Supermicro Vera Rubin IR release, TrendForce HBM4 validation coverage. |
| 2026-06-01 00:00 | [Vera CPU for agents](https://nvidianews.nvidia.com/news/nvidia-unveils-vera-the-cpu-for-agents) + [DGX Station for Windows](https://nvidianews.nvidia.com/news/nvidia-dgx-station-for-windows-puts-a-trillion-parameter-ai-supercomputer-on-every-enterprise-desk) | NVIDIA pushed agentic AI infrastructure into CPUs, GB300 deskside systems and Windows enterprise workflows | Tier 1 product/customer; amps: official product timing, named AI labs/clouds/OEMs, Microsoft ecosystem | NVDA primary; MSFT/ORCL/CRWV/DELL/HPE/SMCI/LNVGY secondary | NVDA platform narrative up; OEM and agentic-PC/deskside AI basket may benefit if Q4 system availability and enterprise adoption remain credible | NVDA +6.3%; OEM/cloud/Windows basket avg +8.1%, med +9.2% on 2026-06-01 vs 2026-05-29 close; Yahoo Finance daily chart API fetched 2026-06-02T20:50Z |  | hit | Supply-chain overlay: OEM/ODM list confirms midstream buildout; upstream memory/package capacity remains the risk to watch. |
| 2026-06-01 00:00 | [Cosmos 3](https://nvidianews.nvidia.com/news/nvidia-launches-cosmos-3-the-open-frontier-foundation-model-for-physical-ai) + [Isaac GR00T](https://nvidianews.nvidia.com/news/nvidia-announces-nvidia-isaac-gr00t-reference-humanoid-robot-for-academic-research) + [Alpamayo 2](https://nvidianews.nvidia.com/news/nvidia-alpamayo-2-super-robotaxis) + [DRIVE Hyperion](https://nvidianews.nvidia.com/news/nvidia-drive-hyperion-becomes-the-global-platform-for-a-robotaxi-ready-world) | NVIDIA clustered physical-AI, robotics and robotaxi releases around Cosmos, Jetson/Isaac, Alpamayo and DRIVE Hyperion partners | Tier 1 product roadmap + Tier 2 customer ecosystem; amps: official source, multiple product surfaces, Foxconn/Uber/VinFast/HUMAIN ecosystem | NVDA primary; UBER/Foxconn/robotics and AV ecosystem secondary | NVDA physical-AI narrative up; secondary robotics/AV names mixed and lower conviction until commercial deployments move beyond announcements | NVDA +6.3%; UBER +4.8% on 2026-06-01 vs 2026-05-29 close; several robotics/AV ecosystem names unlisted or not cleanly comparable; Yahoo Finance daily chart API fetched 2026-06-02T20:50Z |  | hit (NVDA-led) | Supply-chain overlay: downstream robotics/AV demand confirmed; edge compute, sensors and EV/robot manufacturing are the bottlenecks to monitor. |
| 2026-06-01 00:00 | [Enterprise software leaders build AI agents with NVIDIA](https://nvidianews.nvidia.com/news/enterprise-software-leaders-build-ai-agents-with-nvidia) | NVIDIA announced Agent Toolkit, NemoClaw, Nemotron 3 Ultra, OpenShell and CUDA-X agent skills with enterprise software partners | Tier 2 downstream software/customer confirmation; amps: official source, named CAD/security/software partners, platform pull-through | NVDA primary; CDNS/SNPS/PLTR/CRWD/MSFT/SAP/NOW/RHT secondary | NVDA software/platform narrative strengthened; secondary software names may see sentiment lift but hardware pull-through is indirect | NVDA +6.3%; enterprise-software basket avg +6.1%, med +7.0% on 2026-06-01 vs 2026-05-29 close; Yahoo Finance daily chart API fetched 2026-06-02T20:50Z |  | hit | Supply-chain overlay: this is demand-side confirmation, not capacity confirmation; ties back to DGX/RTX/Vera hardware demand. |
| 2026-06-01 01:00 | [NVIDIA GTC 2026 keynote](https://www.nvidia.com/gtc/keynote/?nvid=nv-int-bnr-839023) + [RTX Spark/Microsoft release](https://nvidianews.nvidia.com/news/nvidia-microsoft-windows-pcs-agents-rtx-spark) | Jensen/NVIDIA framed AI factories, agentic systems, physical AI, robotics, and RTX Spark Windows PCs as the new personal AI computer | Tier 1 product/event + customer ecosystem; amps: official source, exact product, Microsoft/OEM partners, Blackwell/Grace/CUDA stack | NVDA primary; MSFT/ARM/DELL/HPQ and AI-PC ecosystem secondary | NVDA and AI-PC/agentic-PC basket up or narrative-strengthening over 1-2w; durability depends on partner follow-through and broader AI risk appetite | NVDA +6.3%; AI-PC/OEM basket avg +9.3%, med +9.6% on 2026-06-01 vs 2026-05-29 close; Yahoo Finance daily chart API fetched 2026-06-02T20:50Z |  | hit | Initial primary-source seed row from repo creation. |
| TIMER_LEDGER_START |  |  |  |  |  |  |  |  |  |

## Rolling hit-rate

| Pattern | Calls logged | Directional hits | T+1w held | Notes |
|---|---:|---:|---:|---|
| Tier 1 product roadmap | 3 | 3/3 | 0 | GTC/RTX Spark, Vera CPU/DGX Station, and physical-AI/robotaxi clusters all hit T+1d on NVDA-led public quote context; durability pending. |
| Tier 1 demand/capacity | 2 | 2/2 | 0 | Vera Rubin full-production and DSX AI-factory infrastructure rows hit T+1d; power/cooling secondaries were more mixed than AI-cloud/OEM names. |
| Tier 2 customer/supplier confirmation | 1 | 1/1 | 0 | Enterprise software-agent partner row hit T+1d; secondary software impact remains lower conviction than NVDA platform signal. |
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
