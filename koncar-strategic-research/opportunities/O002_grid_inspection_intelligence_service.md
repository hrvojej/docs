---
opportunity_id: O002
title: KONČAR Grid Inspection Intelligence & Remote Inspection Service
status: candidate-validation
as_of: 2026-09-21
market_evidence: E3
koncar_fit_evidence: E4-candidate
commercial_validation: not-yet-E5
benchmark: B002
tags: [grid, substations, transmission, drones, robotics, computer-vision, inspection, remote-operations, service]
---

# O002 — KONČAR Grid Inspection Intelligence & Remote Inspection Service

## Thesis

Build a **vendor-agnostic grid inspection intelligence and managed service**, using existing KONČAR domain/field/software assets while partnering for robotic capture hardware.

The product should not depend on KONČAR designing a drone or quadruped robot.

Conceptual stack:

**capture platform → standardized inspection mission → visual/thermal/LiDAR data → AI/engineering validation → asset history → defect/risk prioritization → work order → KONČAR field intervention**

Capture platforms may include:
- existing/manual Dalekovod drones;
- docked autonomous drones;
- ground inspection robots;
- fixed cameras/sensors;
- technician mobile capture.

## Why this thesis exists

B002 validates a mature market:
- Skydio: AEP, SCE, AVECC;
- Percepto: FPL, Siemens Energy, EGAT;
- ANYbotics: RTE;
- Cyberhawk: SSEN Transmission;
- Sharper Shape: data/digital-twin inspection layer.

KONČAR also has unusually relevant internal adjacency:
- Dalekovod already uses drones + optical/thermal/laser cameras;
- Digital owns OT/SCADA/data/cyber capability;
- HELB/Dalekovod/TELENERG can execute field remediation;
- Institute brings sensing/diagnostic expertise.

## Customer problem

Today inspection often suffers from:
- manual truck rolls;
- dangerous energized environments;
- inconsistent capture;
- inspection intervals too long to detect developing defects;
- large image volumes not tied cleanly to assets;
- expert bottlenecks;
- weak longitudinal comparison;
- disconnected inspection and maintenance systems.

The product should sell faster, safer, repeatable **decisions**, not imagery.

## Target buyers

Primary:
1. transmission system operators;
2. distribution system operators;
3. owners of large private grids / industrial substations;
4. renewable operators;
5. EPC customers with long-term O&M;
6. ports / rail / industrial critical infrastructure where KONČAR already works.

Potential initial regional buyers to investigate:
- Croatia;
- Slovenia;
- CEE/SEE utility markets where KONČAR/Dalekovod already have customer access.

No buyer has yet been validated for willingness-to-pay.

## Product structure

### Tier 1 — Inspection-as-a-Service
Use existing/manual drones and current sensors.

Deliver:
- standardized visual/thermal/LiDAR capture;
- asset-linked findings;
- severity classification;
- engineering validation;
- digital report;
- recommended actions.

Goal:
establish workflow and data model before autonomy.

### Tier 2 — Grid Inspection Intelligence
Central software layer:
- asset registry/map;
- inspection history;
- side-by-side/time-series comparison;
- thermal/visual anomaly support;
- defect taxonomy;
- risk/severity;
- work-order integration;
- API integration with SCADA/GIS/EAM.

Commercial model:
annual software/service subscription + inspection activity.

### Tier 3 — Remote Autonomous Site
For selected substations:
- partner drone-in-a-box;
- scheduled and event-triggered missions;
- remote operation center;
- automated upload;
- repeatable camera poses;
- alarm-driven dispatch.

Commercial model:
multi-year managed service / hardware lease + recurring software/service fee.

### Tier 4 — Multi-Robot / Sensor Orchestration
Optional later:
- ground robot for indoor/flight-constrained areas;
- fixed cameras;
- other sensors;
- drone fleet.

The key principle is one asset/workflow layer independent of capture hardware.

## Internal capability map

| Layer | Candidate KONČAR owner |
|---|---|
| Grid asset domain / defect taxonomy | Dalekovod + TELENERG + Institute |
| Existing aerial capture | Dalekovod-Projekt |
| Visual/thermal engineering validation | Dalekovod + Institute |
| Asset data/platform | Digital + NEOS |
| SCADA/OT/cyber integration | Digital |
| GIS / project geometry | Dalekovod-Projekt + Digital |
| AI/CV pipelines | NEOS/Digital + partner initially |
| Field remediation | Dalekovod + HELB + TELENERG |
| Customer/channel | Dalekovod + Group sales |
| Autonomous drone/robot hardware | partner |
| BVLOS operations/regulatory | build operational capability + specialist partner initially |

## Gap classification

### G0 — Native
- power-grid infrastructure domain;
- substation/line engineering;
- field inspection and maintenance;
- existing drone use;
- optical/thermal/laser data capture;
- condition analysis;
- SCADA/OT;
- service/commissioning.

### G1 — Adjacent
- centralized asset data model;
- GIS integration;
- workflow/work-order system;
- customer portal;
- cybersecurity layer;
- AI/data engineering.

### G2 — Buildable
- standardized defect ontology;
- inspection history / change detection;
- operator center;
- computer-vision validation workflow;
- remote mission operations SOPs;
- recurring inspection SLA;
- asset-level KPI and ROI dashboards.

### G3 — Partner
- drone-in-a-box;
- low-level autonomous navigation;
- ground robot;
- advanced payloads where needed;
- initial production-grade CV foundation models;
- BVLOS regulatory expertise.

### G4 — Acquire
No acquisition needed for pilot or first product.

Potential future acquisition only if autonomy/robotics becomes a common strategic platform across:
- grids;
- hydro;
- renewables;
- factories;
- rail;
and KONČAR wants to own core robotics IP.

### G5 — Structural / regulatory
BVLOS is regulated under EASA specific-category/SORA pathways. This raises operating complexity but is not currently a structural blocker.

## Why KONČAR should not build the robot first

The external benchmark shows:
- strong mature robot/drone suppliers already exist;
- drone hardware commoditizes faster than grid-domain data/workflow;
- Croatian inspection providers already sell basic drone services.

KONČAR's defensible assets are more likely:
- grid engineering;
- customer access;
- defect interpretation;
- inspection history;
- OT integration;
- field response;
- lifecycle service.

Owning low-level flight/legged locomotion would add R&D burden before customer value is proven.

## Candidate pilot sequence

### Pilot A — workflow/data pilot
Use existing Dalekovod drones.

Scope hypothesis:
- 1–2 substations;
- selected overhead-line/tower segment;
- RGB + thermal, LiDAR where useful;
- define repeatable asset shot list;
- create digital asset/defect history;
- compare manual report vs integrated workflow.

Goal:
validate data model and maintenance workflow with almost no robotics CAPEX.

### Pilot B — docked autonomous substation
After Pilot A:
- one partner drone-in-a-box;
- one controlled/willing substation;
- scheduled mission;
- event-triggered remote launch;
- visual + thermal;
- remote operations;
- work-order integration.

### Pilot C — ground robot only if justified
Test a partner quadruped only where:
- indoor/outdoor terrain;
- gauge/acoustic/gas close-range inspection;
- flight restrictions;
- hazardous routine rounds
create clear incremental ROI.

## Business model hypotheses

Potential revenue:
1. project inspection fee;
2. annual site/fleet inspection contract;
3. SaaS/asset-intelligence fee;
4. managed remote-operations fee;
5. dock/robot lease or pass-through;
6. field maintenance/remediation;
7. multi-year O&M/SLA.

Best recurring model hypothesis:
**managed inspection + asset intelligence + field intervention**, not hardware resale.

No pricing/margin is yet validated.

## Competitive differentiation hypotheses

1. **end-to-end grid domain** — inspection through remediation;
2. **vendor-agnostic capture** — customer not locked to one robot;
3. **OT-native integration** — SCADA/cyber and operational workflows;
4. **existing EPC/service footprint** — Dalekovod/HELB/TELENERG;
5. **engineering validation** — not black-box CV alone;
6. **cross-asset expansion** — later hydro/renewables/rail/manufacturing.

These remain hypotheses until buyer validation.

## Regulatory architecture

For aerial autonomy in Europe:
- VLOS pilots can start quickly under applicable operating rules;
- true BVLOS typically requires specific-category authorization or applicable predefined framework;
- SORA 2.5 is central to current EASA risk assessment.

Regulatory operations should be designed as part of the product, not added after deployment.

## Evidence state

- Market: **E3** repeatable category.
- KONČAR fit: **E4 candidate** because domain, existing drone use, software and field-service assets are verified and a low-CAPEX pilot path exists.
- Commercial E5: not reached.

## Validation gates

### Internal
- document current Dalekovod drone fleet/operators/workflows;
- identify software used for photogrammetry/GIS;
- determine whether current imagery is asset-linked and longitudinal;
- map Digital GIS/EAM/SCADA integration;
- assess production CV capability.

### Customer
- interview TSO/DSO/O&M buyers;
- current inspection frequency and cost;
- defect classes;
- truck-roll cost;
- outage/safety value;
- BVLOS appetite;
- procurement model.

### Partner
Shortlist:
- EU-supported drone-in-box/autonomy vendors;
- ground robot vendor if needed;
- sensor/payload vendors;
- regulatory/BVLOS partner.

### Economics
- inspection cost per site/tower/km;
- operator hours;
- dock CAPEX/lease;
- regulatory overhead;
- cloud/CV costs;
- remote operator span;
- avoided truck rolls;
- incremental maintenance/remediation revenue.

## Linked evidence

- [B002](../benchmarks/B002_autonomous_grid_substation_inspection_2026-09-21.md)
- [E002 Digital](../entities/E002_koncar_digital.md)
- [E005 HELB](../entities/E005_helb.md)
- [E006 Dalekovod](../entities/E006_dalekovod.md)
- [E017 TELENERG](../entities/E017_telenerg_engineering.md)
- [E001 Institute](../entities/E001_electrical_engineering_institute.md)

## Next action

Run O002-V1 validation:
1. current Dalekovod drone capability audit;
2. TSO/DSO buyer economics;
3. EU partner + BVLOS path;
4. inspection workflow prototype;
5. select first pilot assets.
