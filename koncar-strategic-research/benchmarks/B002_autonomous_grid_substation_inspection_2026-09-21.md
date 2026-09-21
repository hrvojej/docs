---
benchmark_id: B002
title: Autonomous Grid & Substation Inspection
status: complete-v1
as_of: 2026-09-21
evidence: high-commercial-category
tags: [drones, robotics, substations, transmission, inspection, computer-vision, thermal, bvlos, remote-operations]
---

# B002 — Autonomous Grid & Substation Inspection

## Scope

Outside-in benchmark of commercially deployed inspection systems for:
- substations;
- transmission and distribution assets;
- energized electrical equipment;
- remote/critical grid facilities.

Two distinct commercial subcategories are assessed:
1. **autonomous/docked aerial inspection** — drone-in-a-box, remote operations, BVLOS;
2. **autonomous ground inspection robots** — routine rounds inside substations/plants where flight is undesirable.

A third category — managed drone inspection + asset-data software — is included because it is commercially mature and relevant to KONČAR/Dalekovod.

## Executive conclusion

This is a **repeatable commercial market**, not merely an R&D robotics topic.

Utilities are deploying autonomous/remote inspection to:
- reduce truck rolls and personnel exposure;
- inspect energized assets more frequently;
- accelerate outage/storm response;
- standardize visual/thermal inspection;
- create persistent asset-condition history;
- feed maintenance/work-order decisions.

The commercial product is increasingly not the drone or robot itself. The value chain is:

**robot/drone + dock → repeatable sensor capture → remote operations → AI/thermal analysis → asset history/digital twin → defect prioritization → work order → field intervention**

For KONČAR, the most important finding is that **Dalekovod already uses drones, optical, thermal and laser cameras for condition analysis and maintenance documentation**. Therefore, the opportunity is not “learn to fly drones”.

The likely strategic gap is **persistent autonomy + inspection intelligence + workflow integration + recurring service**.

## Commercial subcategory A — docked drone / remote operations

### Product architecture

Typical stack:
- ruggedized drone;
- RGB zoom camera;
- radiometric thermal imaging;
- optional LiDAR / other sensors;
- weatherproof charging dock;
- remote fleet operations;
- pre-programmed/repeatable missions;
- cloud upload;
- AI/computer-vision analysis;
- asset mapping / geospatial layer;
- integration into maintenance systems.

### Why utilities buy it

Core jobs-to-be-done:
- scheduled visual/thermal inspection without dispatching a crew;
- event-triggered remote inspection after alarms/faults;
- storm/wildfire/emergency response;
- inspection near energized equipment;
- higher inspection frequency;
- standardized, repeatable views;
- data history for condition-based maintenance.

## Vendor benchmark

### 1. Skydio

**Commercial position:** autonomous drones + dock + Remote Ops + inspection workflows.

Capabilities publicly demonstrated:
- remote browser-based flight;
- visual and thermal inspection;
- autonomous return to dock;
- energized substation inspection;
- circuit/powerline patrol;
- AI/computer-vision workflow integrations.

#### AEP
American Electric Power used a drone after a 345 kV bus/static-line event. The inspection identified the initial failure and another static line near failure. Skydio's case study reports approximately **USD 8 million** saved across repairs, outage and additional labour.

AEP is now using docked autonomous drones for programmatic infrastructure inspections and BVLOS response.

#### Southern California Edison
SCE is reported by Skydio as operating **100+ drones**, with additional docked systems, across:
- transmission;
- distribution;
- substations;
- high-fire-risk areas.

#### Arkansas Valley Electric Cooperative
AVECC:
- 36 substations;
- traditional substation inspections required ~6–7 people;
- Skydio workflow reduced inspection time by **>50%**;
- autonomous scanning reduced required people/pilot interaction.

#### 2026 remote-ops demonstration
Skydio publicly demonstrated remote inspection of a live utility environment from **2,090 miles away**, including:
- substation;
- active distribution circuit;
- energized conductors;
- visual/thermal switching;
- automatic return to dock.

Sources:
- https://www.skydio.com/customer-stories/american-electric-power-company-aep
- https://www.skydio.com/customer-stories/sce-scales-drone-inspections-to-transform-grid-safety
- https://www.skydio.com/customer-stories/arkansas-valley-electric-co-op-substation
- https://live.skydio.com/public/videos/2090-miles-away-real-assets-real-time-inspection-live-from-dtech-2026-03-06
- https://www.skydio.com/solutions/asset-inspection/faq

### 2. Percepto

**Commercial position:** industrial drone-in-a-box + Percepto AIM cloud software + AI inspection + remote operations.

Architecture:
- Percepto Air;
- weatherproof charging Base;
- RGB + radiometric thermal;
- autonomous mission cycle;
- cloud data upload;
- AI anomaly/change/thermal analysis;
- fleet operations;
- remote control center.

Percepto states one remote operation can manage up to 30 drones under its US regulatory framework.

#### Florida Power & Light (FPL)
In 2022 Percepto announced:
- initial deployment of **13 autonomous drones**;
- planned expansion to hundreds;
- statewide monitoring of substations and distribution grid;
- described at the time as the world's largest commercial autonomous drone deployment.

FPL has used the system both for routine infrastructure inspection and post-storm response.

#### Siemens Energy
Percepto case study:
- automated plant inspections;
- autonomous on-site drone;
- AI/deep-learning analysis after missions;
- automated fault detection;
- shutdown monitoring;
- Siemens Energy reported scaling the technology worldwide.

#### EGAT
Percepto states the Electricity Generating Authority of Thailand can remotely inspect:
- substations;
- transformers;
- floating fences;
- solar floaters
from Bangkok.

Sources:
- https://percepto.co/electric-utilities/
- https://percepto.co/percepto-unveils-worlds-largest-autonomous-commercial-drone-deployment-at-leading-us-electric-utility/
- https://percepto.co/siemens-energy-case-study/
- https://percepto.co/remote-operations/
- https://percepto.co/drone-in-a-box/

## Commercial subcategory B — autonomous ground robots

### 3. ANYbotics / ANYmal

ANYmal is a rugged autonomous quadruped inspection robot with:
- 360° LiDAR;
- six depth cameras;
- optical teleoperation cameras;
- Wi‑Fi / 4G/LTE;
- ~90–120 minute mission range;
- dock/charger;
- edge compute.

Inspection modalities include:
- visual;
- thermal;
- acoustic;
- frequency;
- gas.

#### RTE — France
French TSO RTE evaluated ANYmal for:
- offshore substations;
- urban substations;
- HVDC substations.

ANYmal performed scheduled autonomous inspections and captured:
- thermal;
- visual;
- acoustic;
- frequency data.

ANYbotics reports automated diagnostics and early irregularity detection.

Strategic significance:
Ground robots fit environments where:
- flight is unsafe/undesirable;
- indoor/outdoor mixed terrain exists;
- repeatable close-range gauge/thermal/acoustic inspection is needed;
- permanent autonomous rounds have value.

Sources:
- https://www.anybotics.com/industries/robotic-inspections-for-power-utilities/
- https://www.anybotics.com/news/anymal-autodiagnostics-high-voltage-transmission-rte/
- https://www.anybotics.com/robotics/anymal/

## Commercial subcategory C — managed inspection + visual asset management

### 4. Cyberhawk

Cyberhawk combines:
- professional drone inspection;
- industry-qualified inspection engineers;
- iHawk visual asset-management SaaS;
- defect/work-order workflows.

#### SSEN Transmission
Cyberhawk reports inspection/data management across:
- **>11,500 transmission towers**;
- **~150 substations**;
- North of Scotland transmission network.

iHawk:
- stores UAV and field inspection data;
- supports asset/defect history;
- creates maintenance/work orders;
- gives office and field staff a common asset view;
- has supported multi-million-pound investment decisions.

This is important because it shows commercial value can be captured without owning a unique drone platform.

Sources:
- https://thecyberhawk.com/case-studies/example-case-study
- https://thecyberhawk.com/news/ssen-combine-new-standard
- https://thecyberhawk.com/asset-inspections
- https://thecyberhawk.com/aviate-ebook

### 5. Sharper Shape

Sharper Shape's utility inspection model combines:
- LiDAR;
- RGB;
- IR;
- hyperspectral sensing;
- aerial inspection;
- predictive asset management;
- vegetation analytics;
- a “Living Digital Twin”.

This demonstrates another defensible layer: converting recurring inspection captures into a long-lived geospatial/asset model rather than isolated reports.

Source:
- https://sharpershape.com/applications/

## Regulation — Europe

### BVLOS is not ordinary “open category”
Under current EASA rules, BVLOS generally moves a drone operation outside the normal low-risk open category and into the **specific category** unless an applicable predefined/standard scenario covers the operation.

EASA's current SORA framework requires:
- operational risk assessment;
- ground/air risk evaluation;
- mitigations;
- operational procedures;
- personnel/training requirements;
- technical requirements;
- operational authorization by the competent national authority when required.

As of the June 2026 Easy Access Rules, SORA 2.5 is the current adopted risk-assessment framework.

Implication:
**BVLOS regulatory operations are a real capability layer**, not a paperwork afterthought.

Sources:
- https://www.easa.europa.eu/en/domains/drones-air-mobility/operating-drone/specific-category-civil-drones/specific-operations-risk-assessment-sora
- https://www.easa.europa.eu/en/document-library/easy-access-rules/online-publications/easy-access-rules-unmanned-aircraft-systems

## Local / Croatian commercial baseline

Simple drone inspection is already commercially available in Croatia.

Examples include providers offering:
- visual/thermal powerline inspection;
- substation/infrastructure inspection;
- RGB/thermal/multispectral/LiDAR capture;
- AI-assisted analysis;
- technical reports.

Examples:
- AeroScout;
- Darna;
- TEKUM;
- other regional drone-service companies.

Therefore “drone inspection as such” is **not a differentiated KONČAR strategy**.

Potential differentiation must move up the stack:
- persistent autonomy;
- grid-specific inspection taxonomy;
- repeatable baseline comparison;
- multi-sensor fusion;
- asset graph/history;
- AI-assisted defect recognition;
- SCADA/EAM/GIS integration;
- work-order generation;
- field remediation through KONČAR service entities.

## KONČAR current capability evidence

### Dalekovod / Dalekovod-Projekt
Official Dalekovod material states its engineers use:
- drones;
- optical cameras;
- thermal cameras;
- laser cameras;
for:
- design/project documentation;
- maintenance documentation;
- **condition analysis of operational power facilities**.

This is direct evidence of an existing internal aerial-data/inspection-adjacent capability.

Source:
- https://www.dalekovod.hr/en/design

### Dalekovod OSO
Testing/lab capability includes:
- visual inspection;
- dimensional inspection;
- materials/mechanical/electrical tests;
- magnetic/penetrant methods;
- vibration measurement;
- transmission-line and substation equipment testing.

Source:
- https://www.dalekovod-oso.hr/en/laboratory-testing.aspx

### KONČAR Digital
Relevant adjacent assets:
- SCADA / critical-infrastructure software;
- OT/IT integration;
- cybersecurity;
- AI/ML/data platform capability;
- remote/central control workflow capability.

### HELB
Relevant adjacent assets:
- field installation;
- MV/HV testing;
- commissioning;
- maintenance;
- international deployment.

### TELENERG
Relevant adjacent assets:
- protection/control;
- automation;
- communications;
- substation commissioning.

### Institute
Relevant adjacent assets:
- sensing;
- diagnostics;
- thermal/electrical condition interpretation;
- embedded/monitoring;
- ML diagnostics.

## Gap analysis — market expectation vs KONČAR

| Layer | KONČAR evidence | Gap |
|---|---|---|
| Utility/substation/transmission domain | strong | G0 |
| Field inspection/service engineers | strong | G0 |
| Existing drone use | Dalekovod-Projekt explicit | G0 |
| Optical/thermal/laser capture | explicit | G0 |
| Power-facility condition analysis | explicit | G0 |
| SCADA/OT integration | Digital | G0/G1 |
| Field remediation/commissioning | HELB/Dalekovod/TELENERG | G0 |
| Repeatable automated mission planning | not evidenced | G2/G3 |
| Docked drone / drone-in-box hardware | not evidenced | G3 partner |
| BVLOS operating capability | not evidenced | G2/G3 |
| Utility-specific computer vision models | not evidenced at production scale | G2/G3 |
| Remote fleet operations center | adjacent, not evidenced for drones | G2 |
| Inspection data lake / asset graph | Digital/NEOS adjacent | G1/G2 |
| GIS/EAM/work-order integration | likely adjacent, exact products unclear | G1/G2 |
| Autonomous ground robot hardware | not evidenced | G3 partner |
| Ground-robot autonomy stack | not evidenced | G3 partner |
| Longitudinal digital twin / change detection | adjacency exists, product not evidenced | G2 |
| Managed inspection SLA | field services exist; standardized digital inspection SLA unclear | G1/G2 |

## Build / partner / acquire implication

### Build / own
KONČAR should seek ownership of:
- grid inspection ontology / defect taxonomy;
- inspection-data model;
- asset history;
- workflow/work-order integration;
- domain validation;
- customer-facing inspection intelligence;
- service/SLA;
- Digital/SCADA integration.

### Partner
For v1, partner rather than build:
- drone hardware;
- drone docks;
- low-level flight autonomy;
- ground robot hardware;
- potentially baseline CV models;
- regulatory operating tooling.

### Acquire
No acquisition is required to test the business thesis.

Acquisition only becomes relevant if:
- autonomous robotics becomes a strategic core across several Group verticals;
- partner economics/IP access becomes limiting;
- KONČAR wants its own robotics/autonomy platform rather than a domain solution.

## Strategic inference

The likely attractive position for KONČAR is **not**:
> build a better drone.

It is:
> become the grid-domain inspection intelligence and service layer that can use whichever robotic capture platform best fits the asset.

This means the same platform/workflow could accept:
- handheld technician images;
- manually flown drones;
- docked autonomous drones;
- ground robots;
- fixed thermal/visual cameras;
- other sensors.

That platform/service thesis becomes O002.

## Evidence level

**Market:** E3 — repeatable commercial category with multiple vendors and scaled utility deployments.

**KONČAR fit:** E4 candidate — concrete domain, drone, field-service, OT/software and diagnostic capabilities exist, and a pilot path is plausible; autonomy/CV/BVLOS gaps are clear and partnerable.

## Open questions

1. How extensively does Dalekovod currently use drones operationally vs for project/design documentation?
2. Is there an internal UAS team, fleet and licensed operators?
3. What photogrammetry/GIS platform does Dalekovod-Projekt use?
4. Is inspection imagery stored longitudinally per asset today?
5. Is there an existing defect taxonomy/work-order workflow?
6. Does Digital already integrate GIS/EAM with PROZA or related platforms?
7. Is computer vision used on inspection imagery today?
8. Can HOPS/HEP or another utility provide a pilot fleet/site?
9. What BVLOS operational approvals would a Croatian pilot require?
10. Which drone-in-a-box vendors provide viable EU/Croatia regulatory/support coverage?
11. Does a ground robot add enough value in typical European substations versus docked aerial + fixed sensors?
12. What is current inspection cost per substation / tower / km and crew-hours?

## Next validation

Proceed with O002:
- split aerial vs ground-robot economics;
- map Dalekovod's current drone workflow in detail;
- identify partner hardware shortlist;
- quantify regulatory path;
- identify a utility/substation pilot;
- model service pricing and customer ROI.
