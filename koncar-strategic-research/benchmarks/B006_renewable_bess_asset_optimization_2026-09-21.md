---
benchmark_id: B006
title: Renewable O&M, Inspection, Forecasting & BESS Optimization
status: complete-v1
as_of: 2026-09-21
evidence: high-commercial
tags: [renewables, wind, solar, bess, ems, forecasting, predictive-maintenance, inspection, optimization, portfolio]
---

# B006 — Renewable O&M, Inspection, Forecasting & BESS Optimization

## Scope

Outside-in benchmark of commercially mature digital products and services for:

1. wind and solar inspection;
2. heterogeneous renewable-fleet asset performance management;
3. predictive O&M;
4. BESS state/health monitoring;
5. hybrid plant EMS / PPC;
6. forecasting and portfolio optimization;
7. storage bidding / market optimization;
8. recurring lifecycle service.

The purpose is to determine where KONČAR already has credible native capability and where a commercially meaningful product gap remains.

## Executive conclusion

The market is mature across three connected but distinct layers:

### A. Renewable asset health and inspection
Commercial vendors combine:
- autonomous/drone inspection;
- thermal/RGB data;
- drivetrain/CMS data;
- AI-assisted defect classification;
- digital asset history;
- maintenance workflows.

### B. Portfolio APM and predictive O&M
The value layer increasingly aggregates:
- mixed OEM fleets;
- SCADA;
- condition monitoring;
- alarms/events;
- weather;
- maintenance history;
- performance loss;
- financial impact.

### C. BESS / hybrid plant optimization
Leading platforms operate from:
- cell/module/rack SOH/SOC;
- PCS;
- site controller;
- plant EMS/PPC;
- grid constraints;
- weather/load forecasts;
to portfolio dispatch and, in some markets, automated market bidding.

KONČAR is **already materially present in B and C**:
- KONBAT BESS;
- KONČAR EMS integrating BMS, PCS and safety/auxiliary systems;
- remote SCADA control;
- remote diagnostics and predictive-maintenance positioning;
- Vis solar + BESS microgrid reference;
- Pometeno Brdo and Vis remotely managed from Zagreb;
- KONČAR Digital energy/SCADA/data capability;
- Renewable Energy Sources as owner/developer/operator;
- a pipeline of large solar projects with BESS/hybrid potential.

Therefore the opportunity is not “enter renewables digitalization” or “build a BESS”.

The more specific strategic gap is:

> **vendor-agnostic portfolio intelligence and optimization spanning renewable generation, BESS, inspection, condition, work orders, forecasting and recurring lifecycle service.**

## Market layer A — autonomous inspection / visual intelligence

### SkySpecs — wind

SkySpecs combines:
- autonomous blade drone inspections;
- drivetrain/CMS analytics;
- asset-health intelligence;
- financial/performance analytics.

Current scale positioning:
- ~130 GW served;
- hundreds of thousands of blades inspected;
- major share of North American blades monitored annually;
- tens of billions of dollars of assets under contract.

Inspection model:
- autonomous/repeatable turbine missions;
- rapid capture;
- defect classification/history;
- fleet-level management.

EDF Renewables UK example:
- vendor reports ~25 turbines inspected in one day versus approximately one/day using older rope-access approaches;
- program planned across hundreds of turbines.

Sources:
- https://skyspecs.com/
- https://skyspecs.com/solutions/autonomous-drone-inspections/
- SkySpecs / EDF Renewables UK case material.

### Raptor Maps — solar

Raptor Maps provides:
- solar digital twin;
- aerial/robotic inspection workflows;
- thermal/RGB analysis;
- asset history;
- defect/work-order context;
- autonomous docked-drone integrations.

Commercial scale:
- platform used by hundreds of solar companies;
- portfolio analysis covering hundreds of GWdc;
- autonomous inspection deployments across multi-GW portfolios.

Examples:
- Apex Clean Energy: autonomous drone inspection/response on >2 GW portfolio; tornado-response workflow demonstrated near-real-time condition awareness.
- Madison Energy Infrastructure: ~1 GW / ~800-site portfolio; Raptor Maps used to centralize inspection history and accelerate restoration on acquired assets.

Sources:
- https://raptormaps.com/
- https://raptormaps.com/platform/
- Raptor Maps Global Solar Report 2026
- Raptor Maps Apex / Madison case studies.

## Market layer B — renewable-fleet predictive analytics

### ONYX Insight

ONYX operates as an OEM-independent wind predictive-analytics specialist.

Current positioning:
- 30k+ turbines monitored;
- 40+ countries;
- multi-OEM fleet support;
- drivetrain condition monitoring;
- SCADA/performance analytics;
- fleet-level predictive maintenance.

Examples:
- EDF Renewables: centralizing monitoring across >6 GW, seven turbine OEMs and multiple existing CMS technologies.
- ERG: 300+ turbines across multiple countries/OEMs under fleetMONITOR.
- GE Vernova relationship: ONYX selected for monitoring across thousands of turbines, including retrofit and new equipment.

Strategic point:
**heterogeneous-fleet normalization and expert monitoring are valuable products independent of the turbine OEM.**

Sources:
- https://onyxinsight.com/
- ONYX fleetMONITOR / EDF Renewables / ERG / GE Vernova case announcements.

### Fluence Nispera

Nispera provides renewable asset-performance-management across:
- wind;
- solar;
- storage.

Example:
Wirtgen Invest uses Nispera for a global ~421 MW wind/solar portfolio.

Value proposition:
- performance loss detection;
- downtime reduction;
- centralized KPI/reporting;
- asset benchmarking;
- automated issue identification.

Sources:
- https://fluenceenergy.com/
- Fluence Nispera / Wirtgen Invest case material.

## Market layer C — BESS / hybrid EMS / asset health

### Wärtsilä GEMS

GEMS is a mature grid-scale energy-management platform covering:
- BESS control;
- hybrid renewable/storage plants;
- grid services;
- cell-to-fleet condition visibility;
- state of charge / state of health;
- alarms and performance;
- plant power control;
- forecasting/optimization.

Current deployments include very large BESS projects and long-term service agreements.

Examples:
- Eraring BESS in Australia: very large multi-GWh storage program using GEMS.
- Bungama: 150 MW / 300 MWh system operational in 2026.
- EDF Renewables UK: multiple BESS projects with long-term service agreements and performance commitments.
- Graciosa hybrid island project: renewables + storage coordinated by GEMS.

Wärtsilä also added more explicit predictive battery analytics through GEMS Pulse.

Sources:
- https://www.wartsila.com/energy/gems
- Wärtsilä Eraring / Bungama / EDF Renewables UK / Graciosa project material.

### Fluence Mosaic

Mosaic focuses more directly on **market/value optimization**:
- technology-agnostic storage/hybrid portfolio;
- price forecasting;
- automated bid/dispatch optimization;
- market participation.

Fluence publishes CAISO case results showing significant performance uplift versus market benchmarks. These are vendor-reported commercial results and must be treated as case evidence rather than universal expected returns.

Source:
- https://fluenceenergy.com/energy-storage/fluence-mosaic/

### Tesla Autobidder

Autobidder provides:
- real-time trading/control;
- portfolio optimization;
- automated market participation;
- operational constraint handling.

Commercial proof includes Hornsdale Power Reserve and other Tesla storage portfolios.

Source:
- https://www.tesla.com/support/energy/tesla-software/autobidder

## Commercial architecture

A modern renewable/BESS intelligence stack can be decomposed into:

### 1. Physical asset
- wind turbine;
- PV inverter/string/module;
- battery cell/module/rack;
- PCS/inverter;
- MV/HV plant.

### 2. Local control
- turbine/plant controller;
- BMS;
- PCS;
- PPC;
- EMS;
- protection.

### 3. Data / SCADA
- live telemetry;
- alarms/events;
- historian;
- weather;
- metering;
- maintenance records.

### 4. Asset health
- drivetrain condition;
- blade defect;
- PV thermal/visual anomaly;
- inverter faults;
- battery SOH/SOC;
- cell imbalance;
- degradation;
- remaining life.

### 5. Portfolio APM
- normalized KPI;
- lost-production analysis;
- issue prioritization;
- work orders;
- cross-site benchmarking;
- financial impact.

### 6. Forecast / optimization
- generation forecast;
- load forecast;
- renewable curtailment;
- storage charge/discharge;
- grid limits;
- energy-price forecast;
- reserve/ancillary service optimization.

### 7. Commercial/lifecycle layer
- remote monitoring;
- expert service;
- availability/performance SLA;
- optimization fee;
- shared upside/revenue share in some markets.

## KONČAR current capability evidence

### KONBAT BESS / EMS

Legacy KONČAR INEM product material documents a complete BESS/EMS capability:

- grid stabilization;
- peak shaving;
- renewable integration;
- backup;
- black start;
- containerized/custom configurations;
- integration across MV/LV;
- EMS integrating BMS, safety/monitoring sensors and PCS;
- DC and AC-side monitoring;
- autonomous configurable algorithms;
- remote SCADA operation;
- IEC 60870-5-104 / Modbus communication;
- continuous remote diagnostics;
- predictive-maintenance positioning.

Important organizational note:
the public product information remains under former INEM lineage. After the 2026 restructuring, the exact current owner of KONBAT product/IP/team must be traced before assigning O006 organizational responsibility.

Sources:
- KONČAR battery-energy-storage-system / KONBAT product pages under legacy INEM material.

### Vis solar + BESS / microgrid

KONČAR delivered:
- engineering/design;
- bidirectional converter;
- EMS;
- BESS integration
for the Vis solar/microgrid project.

Reference configuration:
- ~3.5 MW solar;
- ~1 MW / 1.44 MWh BESS.

Use cases include:
- peak shaving;
- balancing;
- voltage regulation;
- smoothing/forecasting;
- microgrid/grid-support functions;
- future reserve/arbitrage potential.

This is direct evidence of an operational hybrid-energy integration reference.

### Renewable Energy Management Center

KONČAR Digital material documents remote management from Zagreb of:
- Pometeno Brdo wind farm;
- Vis solar/BESS assets.

Pometeno Brdo:
- 17 turbines;
- ~20 MW;
- remote monitoring/control;
- weather;
- blade speed;
- yaw/tilt;
- vibration;
- lubrication;
- hydraulic brakes;
- converter heating/cooling;
- remote activation/output control.

Vis:
- ~3.5 MW solar;
- ~11,200 PV modules;
- integrated storage;
- monitored/managed through the same renewable-energy-management concept.

This is meaningful because KONČAR already has a real **multi-technology remote-operations base**, not only plant SCADA components.

### KONČAR Renewable Energy Sources

Current role includes:
- development;
- management;
- maintenance
of wind, solar and small-hydro assets.

Pometeno Brdo and other assets can serve as internal proving grounds.

### Development pipeline

Current projects include large PV developments in the tens of MW to ~100 MWp range, some explicitly designed with future BESS/hybrid potential.

This creates a plausible internal testbed for:
- portfolio forecasting;
- BESS dispatch;
- centralized APM;
- autonomous inspection;
- lifecycle optimization.

### KONČAR Digital

Adjacent/current:
- PROZA SCADA;
- IIoT;
- predictive energy management;
- HEDGE-IoT;
- data integration;
- cybersecurity;
- remote control;
- custom algorithms.

### NEOS

Adjacent:
- time-series forecasting;
- data engineering;
- ML/AI;
- real-time platforms;
- cloud/data integration.

## Gap analysis — market expectation vs KONČAR

| Layer | KONČAR evidence | Gap |
|---|---|---|
| Wind/solar/BESS domain | strong | G0 |
| Wind/solar asset ownership/operation | strong | G0 |
| SCADA / remote control | strong | G0 |
| BESS EMS / BMS/PCS integration | explicit KONBAT | G0 |
| Hybrid microgrid reference | Vis | G0 |
| Remote diagnostics | explicit | G0/G1 |
| Predictive-maintenance concept | explicit, production depth by asset type to validate | G1 |
| Multi-site renewable control center | explicit | G0/G1 |
| Time-series forecasting capability | NEOS/Digital adjacent | G1 |
| Vendor-neutral fleet APM | not evidenced at ONYX/Nispera breadth | G2 |
| Normalized multi-OEM wind analytics | not evidenced | G2/G3 |
| Autonomous wind blade inspection | not evidenced | G3 partner |
| Solar autonomous/thermal inspection | not evidenced | G2/G3 |
| Unified inspection → work-order workflow | not evidenced | G2 |
| Fleet-level battery SOH/RUL | site EMS evidence; portfolio analytics unclear | G1/G2 |
| Hybrid portfolio optimizer | local EMS capability; portfolio layer unclear | G2 |
| Market bidding/trading optimizer | not evidenced | G2/G3 |
| Long-term digital performance SLA | not evidenced as standardized offer | G2 |
| Unified renewable+BESS commercial P&L | not evidenced | organizational gap |
| Current KONBAT product owner after INEM restructuring | unresolved | organizational/legal gap |

## Strategic inference

The most credible opportunity is not a new standalone EMS.

KONČAR already has:
- control;
- BESS integration;
- SCADA;
- remote operations;
- owned/operated renewable assets;
- forecasting/data/AI adjacency.

The productization gap appears to be:

> **move from site-level control and project engineering to a vendor-agnostic, portfolio-level renewable+BESS intelligence and optimization service.**

That service can combine:
- site SCADA;
- wind/solar health;
- inspection data;
- battery health;
- generation forecasting;
- BESS dispatch;
- maintenance work orders;
- financial/availability KPIs;
- expert remote operations;
- recurring service/SLA.

## Build / partner / acquire

### Build / own
KONČAR should seek to own:
- energy asset model;
- renewable+BESS portfolio data layer;
- customer-facing APM;
- cross-site analytics;
- forecasting integration;
- plant/BESS control interfaces;
- work-order/lifecycle integration;
- service operations;
- KPI/financial-loss model.

### Partner
Initially partner for:
- drone hardware;
- blade-inspection capture;
- specialized wind CMS where third-party/OEM systems dominate;
- selected battery-cell analytics if proprietary to cell/BMS vendor;
- merchant bidding/market access where jurisdiction-specific trading capability is required.

### Acquire
No acquisition is required for MVP.

Acquisition becomes strategically relevant only if external validation shows a persistent gap in:
- heterogeneous wind analytics/CMS normalization;
- advanced BESS market optimization;
- global renewable remote operations;
and buying capability materially accelerates scale.

## What not to do first

- Do not build battery cells.
- Do not compete as a generic drone-inspection operator.
- Do not create another isolated solar/wind dashboard.
- Do not develop a merchant-trading platform before target-market/market-access economics are proven.
- Do not design O006 without first resolving where KONBAT capability resides post-INEM.
- Do not assume owned renewable assets automatically provide rights to all OEM turbine/CMS data.

## Evidence level

- renewable inspection: E3;
- multi-OEM renewable APM: E3;
- BESS/hybrid EMS/PPC: E3;
- BESS market optimization: E3 in applicable markets;
- KONČAR fit: E4, with concrete internal assets and pilot environments;
- unified portfolio product commercialization: not E5.

## Open questions

1. Who currently owns KONBAT product/IP/team after INEM restructuring?
2. How many KONBAT/BESS systems exist beyond Vis?
3. What exact EMS algorithms are proprietary to KONČAR?
4. How is battery SOH/RUL handled today?
5. Which battery cell/BMS/PCS vendors are integrated?
6. Is Pometeno Brdo SCADA data stored centrally at turbine-resolution over full history?
7. What wind OEM/CMS data is contractually accessible?
8. What analytics/forecasting currently run in the Renewable Energy Management Center?
9. Is there a maintenance/work-order system integrated with PROZA?
10. What current O&M KPIs and lost-production analytics are used?
11. Are drone/thermal inspections already used on KONČAR-owned solar/wind assets?
12. Can owned assets be used for autonomous-inspection pilots?
13. Is BESS dispatch optimized only technically or also economically?
14. Which target markets allow/need automated market bidding?
15. What recurring digital/O&M revenue exists today?
16. Can the same platform become a broader Group asset-intelligence layer shared with O001/O002/O005?

## Next validation

Create O006 and validate:
- KONBAT capability lineage/product ownership;
- current Renewable Energy Management Center architecture;
- owned-asset telemetry/data rights;
- existing forecasting and maintenance workflows;
- BESS SOH/dispatch maturity;
- one owned-asset pilot combining APM + inspection + forecasting + storage optimization;
- external utility/IPP commercial packaging.
