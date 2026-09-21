---
benchmark_id: B003
title: Hydropower Underwater Inspection, ROV & Robotic NDT
status: complete-v1
as_of: 2026-09-21
evidence: high-commercial-basic_medium-advanced
tags: [hydro, rov, underwater, penstock, turbine, dam, inspection, ndt, sonar, photogrammetry]
---

# B003 — Hydropower Underwater Inspection, ROV & Robotic NDT

## Scope

Outside-in benchmark of commercial and near-commercial robotic inspection for hydropower assets:

- turbines / runners / draft tubes / spiral casings;
- intakes / trash racks / gates / seals;
- dam walls / outlet structures;
- reservoirs;
- penstocks / tunnels;
- underwater corrosion / geometry / thickness / NDT;
- debris and limited intervention.

The benchmark explicitly distinguishes **mature visual/sonar ROV inspection** from **advanced long-range robotic NDT**, because their technical and commercial maturity differs substantially.

## Executive conclusion

### Mature category
Portable tethered ROV inspection of:
- intakes;
- gates;
- trash racks;
- dam structures;
- turbines / runners;
- draft tubes;
- short accessible penstock sections

is commercially proven.

Value is clear:
- replace or reduce diver entry;
- avoid/shorten dewatering;
- reduce outage time;
- smaller crews;
- faster emergency diagnosis;
- high-resolution visual/sonar evidence;
- inspect places divers cannot safely access.

### Less mature / higher-value category
Long, winding or high-pressure penstocks and quantitative structural inspection remain harder.

Challenges include:
- long tether drag/friction;
- strong flow;
- localization;
- pressure;
- communications;
- navigation in darkness/turbidity;
- reliable wall-thickness/NDT measurements;
- mapping measurements to exact position;
- retrieval/failure risk.

2026 ENGIE/SHEM work explicitly shows this gap remains active R&D.

### Strategic implication for KONČAR
Do **not** begin by designing a generic ROV.

A faster commercial path is:
> hydro-domain inspection + engineering interpretation + partner ROV/crawler + digital condition history + repair/refurbishment follow-through.

Only after recurring inspection demand is proven should KONČAR consider owning specialized robotic tooling for difficult penstock/NDT missions.

## Market segment A — portable ROV visual/sonar inspection

### Typical platform
- small tethered ROV;
- HD/4K camera;
- strong lighting;
- imaging sonar for poor visibility;
- depth/heading;
- optional laser scaling;
- optional manipulator;
- portable surface console.

### Typical applications
- intake screens;
- gates and seals;
- turbine runner/blades;
- draft tubes;
- spiral casings;
- trash racks;
- dam face;
- debris/blockage;
- leak/problem investigation.

### Commercial value
The ROV is often inexpensive relative to:
- commercial dive mobilization;
- lockout/tagout;
- dewatering;
- lost production;
- scaffolding/confined-space access.

## Vendor / deployment evidence

### 1. Deep Trekker

Commercial product family:
- DTG3;
- PIVOT;
- REVOLUTION;
- pipe crawlers.

Hydro packages support:
- HD video;
- sonar;
- inspection of intakes, walls, turbines, gates and submerged structures.

#### Ontario Power Generation — Chats Falls
Deep Trekker case material states:
- runner inspections historically required a **six-person dive team** plus work-protection procedures;
- OPG adapted the work to ROV inspection;
- **two-person crew**;
- no human-diver work protection;
- significant time/cost reduction;
- ROV became the normal approach for runner inspection.

#### Still Creek Dam
Deep Trekker DT340 crawler inspected submerged intake pipes and gates:
- entry at ~90 ft underwater;
- pipe lengths ~490 ft;
- murky conditions;
- visual condition / corrosion / blockage assessment.

#### GENIFAB / hydro customers
Deep Trekker materials describe utility/service contractors buying compact ROVs and performing their own inspections, including inspecting one draft tube while other generating groups remain operating.

Sources:
- https://www.deeptrekker.com/industries/energy/hydroelectric
- https://www.deeptrekker.com/resources/customer-success-story-che-swearengen-and-ontario-power-generation
- https://www.deeptrekker.com/news/dam-inspection
- https://www.deeptrekker.com/news/hydroelectric-rov-inspections

### 2. VideoRay

Hydropower product positioning:
- dam inspections;
- intake visual inspection;
- trash-rack inspection;
- reservoir inspection;
- turbine inspection.

Platforms:
- Mission Specialist Defender;
- Pro 5;
- modular payload/tool integration.

#### U.S. Bureau of Reclamation
The Bureau's Underwater Investigations Dive Team evaluated ROVs to replace human diving when possible and selected VideoRay Pro 4 with multibeam imaging sonar for hydro-dam underwater investigation.

Source:
- https://videoray.com/industries/hydroelectric/
- https://videoray.com/u-s-bureau-of-reclamation/

## Market segment B — inspection service rather than equipment sale

### 3. Engineers With Drones — ESB Ireland

This is useful because it demonstrates a **managed service** business model rather than owner-operated equipment.

Public 2026 case material describes an ongoing underwater ROV inspection programme covering most ESB hydroelectric sites in Ireland.

Assets inspected:
- inlet/outlet screens;
- turbines;
- spiral casings;
- gates;
- sealing surfaces;
- scour drains;
- weirs;
- valves.

Reported operating model:
- site manager calls when a routine/specific issue arises;
- inspection drawings reviewed before deployment;
- micro ROV deployed;
- high-resolution condition evidence delivered;
- many jobs completed in a day;
- no diver / no dewatering for suitable tasks.

#### Golden Falls
2026 project:
- 2 m penstock diameter;
- ~17 m max depth;
- penstock, expansion joint, screens, gates, spiral casing;
- zero diver entry;
- inspection identified silt/vegetation and supported maintenance decisions.

Sources:
- https://www.engineerswithdrones.ie/case-studies/esb-hydroelectric-dam-rov-inspections.php
- https://www.engineerswithdrones.ie/case-studies/penstock-inspection-rov.php

## Market segment C — high-fidelity 3D / sonar / photogrammetry

### 4. Ashtead Technology + Voyis

Hydroelectric dam inlet-tower case:
- compact ROV;
- Voyis Discovery stereo camera;
- turbid water;
- high-resolution structural data;
- 3D photogrammetric model;
- dimensional assessment;
- degradation/wear/surface damage;
- baseline for future comparison.

This demonstrates a value shift from “video” to **measurable digital condition baseline**.

Source:
- https://www.ashtead-technology.com/case-study/hydroelectric-dam-inspection/

## Market segment D — robotic crawlers and NDT

### 5. Eddyfi / Inuktun VersaTrax

Capability:
- robotic crawlers;
- remote visual inspection;
- ultrasonic thickness;
- eddy-current techniques;
- laser / sensor integration;
- long-distance penetration.

Hydro/penstock references:
- visual structural assessment of hydroelectric plant pipelines;
- >300 m continuous downhill inspection;
- >1 km traversal completed over two days;
- inspection of weld seams, rivets, corrosion, pitting and deformation.

Eddyfi also demonstrates robotic deployment of UT thickness measurement and integrated RVI/NDT.

Sources:
- https://blog.eddyfi.com/en/how-the-versatrax-goes-the-distance-for-internal-pipeline-inspection
- https://blog.eddyfi.com/en/leveraging-robotics-for-remotely-operated-ut-thickness-measurement
- https://robotics.eddyfi.com/versatrax-ndt-series
- https://www.eddyfi.com/en/industry/municipal-water-sewer-inspection

## Boundary of current maturity — ENGIE/SHEM

ENGIE Research & Innovation published an especially useful 2026 account because it documents **failure/limitations**, not only success.

### 2023 underwater ROV trial
Goal:
- 800 mm penstock;
- target ~400 m penetration;
- optical + acoustic camera.

Problems:
- pressure limits exceeded;
- acoustic camera added limited value;
- umbilical friction in winding penstock prevented long-distance progression.

The robot did not meet the target.

### 2025 aerial robot
SHEM / Laborelec / OMS tested a robot inside a dewatered ~1 m riveted penstock:
- high-resolution camera;
- laser profilometer;
- deformation/corrosion geometry.

### 2026 next step
Planned:
- contactless EMAT ultrasonic thickness;
- robotic arm;
- integration with robot;
- real-site testing;
- stated ambition to commercialize a benchmark solution.

Source:
- https://innovation.engie.com/en/news/news/research-and-innovation/inside-penstocks-how-robotics-is-transforming-hydropower-infrastructure-inspection/30520

## Commercial maturity matrix

| Use case | Maturity |
|---|---|
| Intake/trash-rack visual inspection | E3 mature |
| Gates/seals/dam face visual inspection | E3 mature |
| Turbine/runner/draft tube inspection | E3 mature |
| Emergency problem diagnosis | E3 mature |
| Imaging sonar in turbid water | E3 mature |
| 3D photogrammetric structural baseline | E2/E3 |
| Simple manipulator/debris tasks | E2/E3 |
| Long penstock visual crawler | E2/E3 depending geometry |
| Long flooded winding penstock ROV | E1/E2, site-dependent |
| Full quantitative robotic UT/corrosion mapping | E2 specialized |
| Fully autonomous long-range underwater inspection | E1/E2 |
| Contactless robotic EMAT hydro inspection | E1 / active development |

## Economics / customer value evidence

### Avoided dewatering / outage
ROV value is frequently dominated by avoiding production loss and complex access, not the ROV equipment cost.

Historical hydropower examples demonstrate that shortening multi-day dewatering/outage to hours can repay equipment quickly, but these older cases should be validated for modern plant economics before a business case.

### Smaller inspection crew
OPG example: six-person dive-team workflow → two-person ROV crew.

### Inspection without shutdown/dewatering
ESB/Golden Falls cases show suitable visual inspections can be completed without divers or full dewatering.

### Faster maintenance decision
ROV/3D evidence supports decision:
- clean or not;
- repair or monitor;
- authorize drain-down or defer;
- target diver/NDT work only where needed.

## KONČAR capability fit

### KONČAR – Hydro Turbine
Verified:
- design/manufacturing;
- erection supervision;
- commissioning;
- performance testing;
- diagnostic measurements;
- maintenance;
- refurbishment;
- after-sales lifecycle support worldwide.

This provides:
- direct hydro-domain expertise;
- customer relationships;
- inspection interpretation;
- a natural path from finding → repair/refurbishment.

Source:
- https://www.koncar.hr/en/koncar-hydro-turbines

### KONČAR – Generators and Motors
Hydro-generator lifecycle:
- inspection;
- preventive/planned maintenance;
- overhaul;
- diagnostics;
- condition evaluation;
- remaining-life assessments.

Source:
- https://www.koncar.hr/en/gim/hydro-generators-1

### Institute
Adjacent capability:
- diagnostics;
- materials/electrical/mechanical testing;
- NDT / condition assessment;
- sensor/monitoring engineering.

### Digital / NEOS
Adjacent:
- inspection-data platform;
- asset history;
- computer vision / data engineering;
- digital-twin integration;
- remote expert workflow.

### HELB
Adjacent:
- field engineering/commissioning/service organization.

## Gap analysis

| Layer | KONČAR evidence | Gap |
|---|---|---|
| Hydro turbine engineering | strong | G0 |
| Hydro lifecycle/service customer access | strong | G0 |
| Diagnostic interpretation | strong | G0 |
| Mechanical/electrical refurbishment | strong | G0 |
| Field project execution | strong | G0 |
| Inspection data platform | adjacent | G1 |
| CV/AI defect support | adjacent / production depth unclear | G1/G2 |
| ROV platform | no evidence | G3 partner |
| ROV pilots/tether operations | no evidence | G2/G3 |
| Imaging sonar | no evidence | G3 |
| Underwater photogrammetry | no evidence | G2/G3 |
| Underwater UT/NDT robotic tooling | no evidence | G3 |
| Long-penstock localization/navigation | no evidence | G3 / R&D |
| Manipulator/intervention tooling | no evidence | G3 |
| Commercial diving integration/safety procedures | unclear | G2/G3 |
| Standardized underwater inspection service SKU | no evidence | G2 |
| Longitudinal condition model | Digital/Institute adjacency | G1/G2 |

## Build / partner / acquire implication

### Partner first
For initial commercial service:
- ROV hardware;
- sonar;
- underwater imaging/photogrammetry;
- NDT crawler;
- specialist underwater operator/training.

### Build / own
KONČAR should own:
- hydro inspection procedure;
- defect taxonomy;
- engineering interpretation;
- asset model/history;
- comparison over time;
- repair/refurbishment recommendation;
- integration with lifecycle service;
- customer relationship.

### Selective R&D later
Only after volume/need is validated:
- specialized hydro payload;
- tether management;
- localization;
- automated turbine/penstock mapping;
- AI defect segmentation;
- dedicated robotic NDT.

### Acquisition
No acquisition needed for MVP.

Potential future acquisition becomes rational only if underwater/inspection robotics proves reusable across:
- hydro;
- ports/marine;
- offshore renewable;
- industrial water;
- dam infrastructure
at sufficient revenue scale.

## Strategic inference

A generic “KONČAR ROV” is unlikely to be the best starting product.

A more defensible first position is:

> **KONČAR hydro inspection and lifecycle service using partner robotic platforms, where the deliverable is an engineering condition decision and repair path, not raw video.**

The first commercial wedge can be narrow:
- turbine/runner;
- intake/gates;
- draft tube/spiral casing;
- dam structures.

Advanced penstock NDT can be a second-stage R&D/product opportunity.

## Evidence level

- Basic hydro ROV visual inspection: **E3 repeatable market**.
- Advanced long-range/robotic NDT: **E1–E2 depending use case**.
- KONČAR fit for managed hydro inspection: **E4 candidate** via Hydro Turbine + GIM + Institute + Digital + service footprint.

## Open questions

1. What underwater inspection does KONČAR Hydro Turbine currently subcontract?
2. Which customer outages/refurbishments already require diver/ROV work?
3. Does KONČAR have inspection procedures for cavitation/erosion under water?
4. Can existing hydro clients provide a pilot?
5. What is the cost of diver inspection vs dewatering vs ROV across representative KONČAR projects?
6. What percentage of jobs need sonar due to turbidity?
7. Is dimensional/3D measurement commercially valued or is video enough?
8. How often is UT wall thickness needed?
9. Which penstock geometries are highest-value and technically feasible?
10. Does KONČAR want to sell equipment, inspection service, or lifecycle contract?
11. What certifications/safety procedures are required in target countries?
12. Could the same team serve dams, ports, shipyards or offshore wind to increase utilization?

## Next validation

Create O003 and validate:
- current KONČAR hydro inspection/subcontracting workflow;
- pilot asset/customer;
- partner ROV/NDT platform;
- diver/outage cost baseline;
- service price and utilization;
- advanced penstock R&D only after commercial service validation.
