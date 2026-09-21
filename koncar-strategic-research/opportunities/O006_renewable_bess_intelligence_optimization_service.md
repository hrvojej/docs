---
opportunity_id: O006
title: KONČAR Renewable & BESS Intelligence / Optimization Lifecycle Service
status: candidate-validation
as_of: 2026-09-21
market_evidence: E3
koncar_fit_evidence: E4
commercial_validation: not-yet-E5
benchmark: B006
tags: [renewables, bess, ems, asset-performance-management, forecasting, optimization, inspection, lifecycle-service]
---

# O006 — KONČAR Renewable & BESS Intelligence / Optimization Lifecycle Service

## Thesis

Evolve existing KONČAR renewable-control and BESS capabilities into a **vendor-agnostic portfolio-level intelligence, optimization and lifecycle service**.

Conceptual product:

**SCADA/EMS + weather + inspection + condition monitoring + battery SOH + forecasting → portfolio health → work orders → hybrid dispatch → recurring remote O&M/SLA**

This should sit above individual plant controllers rather than replace them.

## Why this is credible

KONČAR already has:
- renewable asset development/O&M;
- wind and solar references;
- multi-technology remote management;
- KONBAT BESS + EMS;
- BMS/PCS integration;
- hybrid solar+BESS reference;
- remote diagnostics;
- SCADA;
- Digital/NEOS forecasting/data/AI capability;
- owned/controlled assets suitable for pilots.

Therefore O006 is primarily a **productization and portfolio-optimization problem**, not a fundamental technology feasibility problem.

## Customer groups

Primary:
1. renewable IPPs;
2. utilities;
3. mixed wind/solar/BESS portfolio owners;
4. industrial microgrids;
5. municipal/critical-infrastructure energy systems;
6. KONČAR-developed/operated renewable projects.

## Jobs-to-be-done

Customer outcomes:
- know which asset loses revenue and why;
- prioritize maintenance;
- detect degradation before failure;
- centralize mixed-OEM fleets;
- automate inspection evidence;
- improve renewable forecast;
- optimize storage dispatch;
- manage grid constraints;
- reduce curtailment/imbalance;
- extend battery life;
- measure availability/lost production;
- coordinate site and portfolio operations;
- reduce manual reporting.

## Product modules

### P1 — Portfolio Operations
- site/fleet overview;
- normalized KPIs;
- alarms/events;
- availability;
- lost production;
- asset hierarchy/history;
- multi-OEM normalization.

### P2 — Asset Health
Wind:
- drivetrain/CMS;
- vibration;
- gearbox/bearing health;
- turbine alarms.

Solar:
- inverter/string/module performance;
- thermal/visual anomaly;
- degradation.

BESS:
- SOC/SOH;
- cell/module/rack imbalance;
- degradation/RUL;
- PCS/BMS alarms.

### P3 — Inspection Intelligence
- drone/thermal/RGB ingestion;
- blade/PV defect taxonomy;
- asset-linked evidence;
- repeat inspection comparison;
- maintenance work orders.

Use partner capture hardware initially.

### P4 — Forecasting
- wind;
- solar;
- load;
- weather;
- storage availability;
- uncertainty bands.

NEOS/Data Science capability is directly relevant.

### P5 — Hybrid EMS / Dispatch
- renewable generation;
- BESS charge/discharge;
- SOC reserve;
- grid connection;
- curtailment;
- PV/wind forecast;
- peak shaving;
- ancillary/grid-support logic.

KONBAT/Vis provides a native starting point.

### P6 — Economic Optimization
Later:
- tariff-aware dispatch;
- imbalance minimization;
- reserve-market optimization;
- merchant bidding.

This layer may require market-specific partners/licensing and should not be the first product in every country.

### P7 — Remote O&M / Lifecycle Service
- expert remote monitoring;
- periodic performance reports;
- event triage;
- maintenance planning;
- defined SLA;
- optional performance commitments after sufficient evidence.

## Internal capability hypothesis

| Layer | Candidate KONČAR owner |
|---|---|
| Renewable asset/operator domain | Renewable Energy Sources |
| Plant SCADA / remote control | Digital |
| BESS / EMS product | former INEM capability lineage — current owner to resolve |
| PCS/power electronics | former INEM/KONČAR capability lineage |
| Forecasting/data engineering | NEOS + Digital |
| AI/analytics | NEOS + Digital |
| Electrical diagnostics | Institute |
| Field service | renewable O&M + HELB / relevant entities |
| Commercial customer relationship | Renewable Energy Sources / Digital / Group |

## Organizational blocker to resolve first

The most important immediate question is:

**Where does KONBAT now live after the 2026 INEM demerger/merger?**

Because the former INEM Power Supply business unit moved into HELB before the remaining INEM merger, some or all BESS/power-electronics capability may have moved organizationally.

Do not assign O006 product ownership until:
- product IP;
- engineers;
- sales;
- references;
- service responsibility
are mapped.

## Gap classification

### G0 native
- SCADA;
- renewable O&M/domain;
- BESS integration;
- EMS;
- BMS/PCS integration;
- hybrid microgrid;
- remote control;
- owned renewable assets;
- electrical/power engineering.

### G1 adjacent
- time-series forecasting;
- ML/data engineering;
- multi-site dashboards;
- predictive maintenance;
- remote diagnostics.

### G2 build/productize
- normalized multi-OEM APM;
- unified renewable+BESS asset model;
- inspection-to-work-order flow;
- battery fleet SOH/RUL;
- portfolio dispatch;
- financial lost-production model;
- standardized remote O&M SLA.

### G3 partner
- autonomous inspection hardware;
- specialized wind blade CV initially;
- third-party turbine CMS normalization;
- proprietary cell/BMS models;
- merchant bidding/market access where required.

### G4 acquire
No acquisition required for MVP.

### G5 potential blockers
- OEM turbine data access;
- battery supplier data/IP;
- market/trading licenses;
- KONBAT organizational ownership;
- cyber/critical-infrastructure requirements.

## Pilot path

### Pilot 1 — internal asset-data consolidation
Use owned/controlled assets:
- Pometeno Brdo;
- Vis;
- one selected solar project;
- one BESS.

Create:
- common asset model;
- normalized KPIs;
- alarms/events;
- maintenance history;
- weather/forecast;
- inspection evidence.

### Pilot 2 — inspection integration
Add:
- drone/thermal inspection on wind/solar;
- asset-linked defects;
- work-order flow.

Hardware can be partner supplied.

### Pilot 3 — BESS health + forecast
Add:
- SOC/SOH;
- degradation;
- PV/wind forecast;
- site/load/grid limit.

### Pilot 4 — optimization
Optimize:
- renewable + storage dispatch;
- peak/curtailment;
- reserve policy;
- battery-life tradeoff.

### Pilot 5 — recurring service
Package:
- portfolio software;
- remote expert monitoring;
- monthly performance/loss report;
- maintenance workflow;
- SLA.

## Business model hypotheses

Revenue:
1. implementation/integration;
2. annual per-MW / per-site platform fee;
3. remote O&M fee;
4. inspection service;
5. BESS optimization fee;
6. lifecycle/service contract;
7. later shared savings/performance fee;
8. market-optimization fee where legally/commercially appropriate.

No price/margin is yet validated.

## Cross-opportunity leverage

O006 should not become a separate software island.

Shared foundations with other opportunities:
- O001 transformer asset intelligence;
- O002 inspection intelligence;
- O005 rail/battery intelligence.

Potential reusable Group platform layers:
- asset model;
- time-series ingestion;
- alarm/event model;
- inspection evidence;
- work order;
- health index;
- forecasting;
- battery analytics;
- remote expert workflow.

This is a strong argument for an eventual **common industrial asset-intelligence platform**, while keeping domain products separate.

## What not to do first

- do not build battery cells;
- do not build a proprietary inspection drone;
- do not launch merchant trading before local market economics/permissions are validated;
- do not rebuild site SCADA;
- do not create a generic “AI energy dashboard”;
- do not assume all OEM turbine data is contractually available.

## Evidence state

- external category: E3;
- KONČAR fit: E4;
- owned-asset pilot path: concrete;
- unified commercial product: E5 pending.

## Validation gates

### Organization
- current KONBAT owner/team/IP;
- Renewable Energy Management Center product ownership;
- Digital/RES/HELB responsibilities.

### Data
- Pometeno telemetry/historian;
- Vis BESS/solar telemetry;
- maintenance records;
- OEM CMS access;
- BMS data rights.

### Technical
- existing forecasting algorithms;
- battery SOH/RUL;
- dispatch algorithms;
- asset hierarchy/data model;
- work-order integration.

### Commercial
- current O&M contracts;
- recurring software/service revenue;
- external IPP interest;
- willingness to pay per MW/site;
- performance/SLA risk.

## Linked evidence

- [B006](../benchmarks/B006_renewable_bess_asset_optimization_2026-09-21.md)
- [E012 Renewable Energy Sources](../entities/E012_renewable_energy_sources.md)
- [E002 Digital](../entities/E002_koncar_digital.md)
- [E003 NEOS](../entities/E003_neos_capability_lineage.md)
- [E004 former INEM](../entities/E004_former_inem_capability_lineage.md)
- [E005 HELB](../entities/E005_helb.md)

## Next action

Resolve KONBAT lineage and map the actual current Renewable Energy Management Center + Vis/Pometeno data architecture before designing a new platform.
