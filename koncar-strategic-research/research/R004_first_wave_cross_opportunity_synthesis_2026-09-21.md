---
research_id: R004
title: First-Wave Cross-Opportunity Synthesis
status: complete-v1
as_of: 2026-09-21
inputs: [B001, B002, B003, B004, B005, B006, O001, O002, O003, O004, O005, O006]
evidence: synthesis-of-E3-market-and-E4-fit-evidence
tags: [synthesis, strategy, productization, servitization, common-platform, validation]
---

# R004 — First-Wave Cross-Opportunity Synthesis

## Purpose

Synthesize the first six outside-in benchmark families and identify:
- repeated strategic patterns;
- shared capabilities;
- distinct business models;
- common gaps;
- validation sequence;
- what should **not** be prematurely unified.

This document does **not** declare a winner. None of O001–O006 has reached E5 commercial validation.

## Inputs

- B001 / O001 — Transformer Intelligence & Lifecycle Service
- B002 / O002 — Grid Inspection Intelligence & Remote Inspection
- B003 / O003 — Hydro Underwater Inspection & Lifecycle Service
- B004 / O004 — Adaptive Heavy Fabrication & Digital Quality
- B005 / O005 — Rail Fleet & Battery Intelligence
- B006 / O006 — Renewable & BESS Intelligence / Optimization

## Core finding #1 — KONČAR often already owns the difficult domain layer

Across five external-facing opportunity families, the initial research repeatedly found that KONČAR is **not starting from zero**.

### O001 transformers
Already has:
- transformer OEM capability;
- TMS;
- vendor-neutral retrofit;
- condition models;
- partial-discharge ML;
- international monitoring references;
- field diagnostics/service.

### O002 grid inspection
Already has:
- grid EPC/domain;
- drone use;
- optical/thermal/laser capture;
- condition analysis;
- SCADA/OT;
- field maintenance/commissioning.

### O003 hydro
Already has:
- turbine engineering;
- diagnostics;
- lifecycle service;
- refurbishment;
- hydro customer access.

### O005 rail
Already has:
- trains;
- battery trains;
- charging stations;
- maintenance;
- centralized coordination platform under development;
- data/AI capability elsewhere in Group.

### O006 renewables/BESS
Already has:
- wind/solar asset operations;
- renewable control center;
- BESS/EMS;
- solar+BESS microgrid;
- SCADA;
- remote diagnostics;
- forecasting/data capability.

This is strategically important because many opportunities are **productization gaps**, not basic technology gaps.

## Core finding #2 — repeated missing value layer is “servitization”

Across O001, O002, O003, O005 and O006, leading external competitors increasingly monetize:

**hardware/domain asset → telemetry/inspection → analytics → expert workflow → maintenance action → multi-year service/SLA**

The recurring KONČAR gap appears to be:
- cross-asset software productization;
- fleet/portfolio view;
- persistent asset history;
- normalized health/risk;
- remote expert operations;
- work-order integration;
- recurring subscription/service contract;
- explicit end-to-end product owner;
- recurring P&L.

This does not mean every opportunity should use the same application. It means the business-model pattern is repeated.

## Core finding #3 — robots are usually capture tools, not the defensible product

B002 and B003 reached the same conclusion independently.

### Grid
Strong commercial robot/drone suppliers already exist:
- Skydio;
- Percepto;
- ANYbotics;
- others.

### Hydro
Strong ROV/crawler suppliers already exist:
- Deep Trekker;
- VideoRay;
- Eddyfi/Inuktun;
- others.

KONČAR's differentiated layer is more plausibly:
- engineering domain;
- inspection procedure;
- defect taxonomy;
- asset context/history;
- validation;
- maintenance workflow;
- field intervention;
- lifecycle relationship.

### Strategic rule
**Partner for robotic mobility first. Own the domain-intelligence and service layer.**

Build proprietary robotics only if repeated customer missions reveal a high-value gap that partners cannot economically solve.

This preserves the option for later robotics R&D without making it the prerequisite for revenue.

## Core finding #4 — O004 is economically different

O004 is primarily an **internal operating-leverage program**.

Its initial value is:
- factory capacity;
- throughput;
- scarce skilled-labour leverage;
- quality;
- traceability;
- rework reduction;
- delivery performance.

It does not need an external customer to create value.

This makes O004's validation mechanism different:
- OEE;
- arc-on time;
- changeover/programming time;
- bottleneck hours;
- NDT cycle;
- rework;
- contribution margin enabled.

O004 should therefore not be evaluated by the same sales/ARR criteria as O001/O002/O003/O005/O006.

## Opportunity comparison — current evidence, not ranking

| Opportunity | Market maturity | KONČAR fit | Initial business model | Core missing layer | First validation source |
|---|---|---|---|---|---|
| O001 Transformer Intelligence | E3 | E4 | software + expert monitoring + SLA | fleet APM / service packaging | existing TMS customers & internal product architecture |
| O002 Grid Inspection | E3 | E4-candidate | managed inspection + software + field service | autonomy/CV/workflow/BVLOS | Dalekovod current drone workflow + utility economics |
| O003 Hydro Underwater | E3 basic / E1-E2 advanced | E4-candidate | inspection engineering + lifecycle service | underwater operations/product packaging | current hydro subcontracting & outage economics |
| O004 Heavy Fabrication | E3 technology | E4 | internal productivity/capacity | adaptive high-mix automation/data thread | factory OEE / weld-hour Pareto |
| O005 Rail/Battery | E3 | E4 | digital fleet/battery + maintenance SLA | SOH/RUL / orchestration / service packaging | existing centralized-platform architecture |
| O006 Renewable/BESS | E3 | E4 | portfolio APM/optimization + remote O&M | portfolio layer / multi-OEM / service packaging | existing control center + KONBAT lineage + owned assets |

## Common platform primitives

Four opportunities strongly reuse software/data primitives:
- O001;
- O002;
- O005;
- O006.

O003 can reuse some; O004 has a separate manufacturing context but may reuse data/AI infrastructure.

### Potential shared primitives

#### Asset identity / hierarchy
- company;
- site;
- plant;
- fleet;
- system;
- asset;
- component.

#### Time-series ingestion
- sensors;
- SCADA;
- BMS;
- vehicle telemetry;
- CMS;
- weather;
- operational state.

#### Event / alarm model
- raw events;
- normalized event taxonomy;
- severity;
- acknowledgement;
- root-cause links.

#### Inspection evidence
- image;
- thermal image;
- video;
- sonar;
- 3D;
- NDT measurement;
- technician note;
- model result.

#### Asset history
- installations;
- interventions;
- failures;
- inspections;
- maintenance;
- part replacement;
- configuration/version.

#### Health / risk
- condition indicators;
- health index;
- anomaly;
- predicted failure;
- remaining life;
- confidence/uncertainty.

#### Workflow
- issue;
- engineering review;
- recommended action;
- work order;
- intervention;
- closure;
- verification.

#### Expert remote operations
- monitoring queue;
- escalation;
- SLA;
- report;
- customer communication.

#### Analytics / AI
- forecasting;
- anomaly detection;
- classification;
- optimization;
- remaining-life models;
- CV.

#### Cyber / identity / audit
Critical across:
- grid;
- rail;
- renewables;
- transformer monitoring.

## Important architecture warning

Do **not** respond to this commonality by immediately building one giant “KONČAR AI platform”.

That would be premature.

Reasons:
- different safety/regulatory contexts;
- different data rates;
- different latency/control requirements;
- different ownership across subsidiaries;
- different buyer workflows;
- different deployment models (edge/on-prem/cloud);
- rail and critical-grid cyber constraints;
- existing products must be integrated, not replaced.

### Better approach
First define:
- common data contracts;
- identity/asset model;
- event/evidence/work-order interfaces;
- shared telemetry/data services where useful.

Keep domain products independently shippable.

A future R005 can define common architecture **after** O001–O006 validation clarifies real requirements.

## Organizational pattern — repeated cross-subsidiary product ownership problem

Technical capabilities are distributed by design:

- Institute — diagnostics/sensing/domain models;
- Digital — SCADA/OT/platform/cyber;
- NEOS — data engineering/ML;
- OEM companies — hardware/domain/customer;
- HELB/Dalekovod/service organizations — field execution;
- former INEM lineage — converters/embedded/BESS/power electronics.

This produces a repeated risk:
**the product sits between companies, so nobody owns the entire commercial outcome.**

For each O###, validation must identify:
1. executive sponsor;
2. product owner;
3. P&L owner;
4. IP owner;
5. sales owner;
6. service/SLA owner;
7. data controller;
8. engineering contributors.

Without this, technical fit does not become a business.

## Recurring revenue pattern

O001, O002, O003, O005 and O006 all have plausible recurring layers:

- monitoring subscription;
- fleet/portfolio software;
- remote expert service;
- periodic inspection;
- lifecycle contract;
- SLA;
- maintenance;
- optimization fee.

This is strategically relevant because KONČAR has production-capacity and specialist-labour constraints.

A lifecycle/software/service layer can potentially:
- increase revenue per installed asset;
- increase customer lifetime value;
- add revenue without proportional new factory output;
- improve visibility into future service demand;
- strengthen replacement/upgrade sales.

This is a hypothesis until unit economics are validated.

## Installed base and owned assets are an underused validation advantage

KONČAR does not need to validate everything on greenfield external customers.

Potential controlled/reference environments already exist:

### Transformers
- existing TMS installed base;
- D&ST customer relationships.

### Grid
- Dalekovod's current drone/project workflows.

### Hydro
- current service/refurbishment projects.

### Manufacturing
- KMK and KTK factories.

### Rail
- current battery train / charging deployment.

### Renewables
- Pometeno Brdo;
- Vis;
- renewable project portfolio.

This can materially reduce pilot acquisition cost and shorten learning cycles.

## Validation sequence — based on evidence accessibility, not attractiveness ranking

### Track A — existing-product productization
#### O001
Immediate evidence:
- TMS installed base;
- existing customers;
- existing product.

Validate:
- fleet platform;
- attach rate;
- SLA;
- ARR/customer willingness-to-pay.

#### O005
Immediate evidence:
- centralized platform already under development;
- BEMU/charging deployment.

Validate:
- architecture/data rights;
- SOH/RUL;
- charging optimizer;
- maintenance workflow.

#### O006
Immediate evidence:
- control center;
- owned assets;
- KONBAT/Vis.

Validate:
- KONBAT current ownership;
- portfolio data model;
- APM/forecast/BESS integration.

### Track B — service/inspection productization
#### O002
Start with existing Dalekovod drone workflow before autonomy.

Validate:
- current inspection cost;
- data/workflow;
- buyer pain;
- value of dock/BVLOS.

#### O003
Start with current hydro inspection/subcontracting.

Validate:
- diver/dewatering cost;
- routine ROV demand;
- attach to refurbishment.

### Track C — internal operating leverage
#### O004
No customer discovery required for first gate.

Validate:
- weld-hour Pareto;
- robot utilization;
- factory bottleneck;
- NDT cycle;
- contribution margin released.

## Acquisition conclusion — current stage

Across first six opportunities, **no acquisition is required for an MVP/pilot based on current evidence**.

This is not a statement that acquisitions will never be useful.

Potential future acquisition triggers:
- external partner controls strategically critical IP/data;
- capability cannot be built in 12–24 months;
- recurring revenue/category scale is proven;
- acquisition materially accelerates global commercial scale.

Potential acquisition domains to revisit later:
- specialized grid inspection analytics;
- robotics/autonomy if cross-vertical;
- heterogeneous renewable APM;
- battery optimization;
- monitoring/service operations.

## What should happen next

The program should now shift from broad discovery to **evidence destruction**: attempt to disprove each opportunity with internal data and customer economics.

### Required outputs per opportunity
- current internal architecture;
- current revenue/service baseline;
- customer problem;
- pricing;
- pilot;
- unit economics;
- product/P&L owner;
- data/IP rights;
- regulatory constraints.

Only after those exist should O### receive:
- E5 status;
- investment case;
- rollout plan.

## Research backlog generated by R004

### R005 candidate
Common Industrial Asset Intelligence Architecture — only after validation captures actual domain requirements.

### Validation artifacts
- V/O001 — Transformer customer/service economics
- V/O002 — Dalekovod drone workflow and grid inspection economics
- V/O003 — Hydro inspection/subcontract/outage economics
- V/O004 — Factory weld/NDT bottleneck and ROI
- V/O005 — Rail central platform/BMS/charging architecture
- V/O006 — KONBAT/control-center/data architecture

Validation artifacts should be created as R### or O### revisions rather than introducing a new artifact prefix unless needed.

## Bottom line

The first six benchmarks do **not** point to a single technology such as AI, ROVs or robotics.

They point to a repeated KONČAR strategic pattern:

> **take existing industrial hardware/domain/service assets and wrap them in a persistent digital lifecycle relationship: condition, inspection, prediction, optimization, expert action and service contract.**

The most defensible value is usually not the generic AI model or robot hardware.

It is the combination of:
- KONČAR equipment/domain IP;
- operational data;
- installed base/customer access;
- engineering interpretation;
- field execution;
- software/data/AI;
- lifecycle accountability.
