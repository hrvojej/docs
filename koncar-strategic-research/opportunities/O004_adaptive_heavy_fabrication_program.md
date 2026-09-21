---
opportunity_id: O004
title: KONČAR Adaptive Heavy Fabrication & Digital Quality Program
status: candidate-validation-internal-first
as_of: 2026-09-21
market_evidence: E3
koncar_fit_evidence: E4
commercial_validation: internal-roi-pending
benchmark: B004
tags: [manufacturing, welding, robotics, ndt, quality, capacity, productivity, digital-thread]
---

# O004 — KONČAR Adaptive Heavy Fabrication & Digital Quality Program

## Opportunity type

**Internal-first profit/capacity opportunity.**

Unlike O001–O003, the first objective is not to launch an external product.

The objective is to increase:
- effective factory capacity;
- welding throughput;
- scarce-welder leverage;
- quality consistency;
- traceability;
- NDT/inspection efficiency;
- on-time delivery;

in KONČAR's own high-value heavy-fabrication operations.

External commercialization becomes a later option only if reusable KONČAR IP/process technology emerges.

## Thesis

Create a cross-factory adaptive manufacturing program connecting:

**engineering CAD/3D → weld feature extraction → robotability decision → offline robot programming → seam sensing/adaptation → weld process data → automated surface/dimensional inspection → NDT record → quality dossier**

Initial factories:
1. KONČAR – Metal Structures;
2. KONČAR – Transformer Tanks;
3. selected D&ST fabrication operations.

## Why this is credible

### KONČAR proof already exists
KMK published a real internal result:
- CLOOS robotic station;
- one manual assembly ~8 hours;
- robot: three assemblies in same period;
- approximately 3× welding speed;
- consistent quality confirmed by NDT.

This is not a hypothetical automation benefit.

### External high-mix proof exists
- IFH tank fabrication: ~25–40% throughput improvement across ~25 larger tank designs through robotic cells + offline programming.
- Verbotics/TRT: one-off/high-mix assemblies made practical by automatic offline programming; 4h programming → 36h robot welding.
- Path Robotics: autonomous welding demonstrated on generator-tank-scale parts up to 55,000 lb / 60 ft.
- commercial seam tracking and automated inspection technology exists.

## Strategic problem

KONČAR has strong global demand and major factory expansion, but growth is constrained by:
- production capacity;
- qualified specialist labour;
- high quality requirements;
- custom/engineering-to-order product mix.

Adding factory square metres and employees is only one response.

The alternative/complement is:
**increase output per skilled welding/quality-engineering hour.**

## Program modules

### M1 — Part-family / weld Pareto
Create a data model of:
- part family;
- annual quantity;
- weld metres;
- process;
- material/thickness;
- position;
- joint type;
- fit-up variability;
- current manual hours;
- crane/repositioning time;
- inspection requirement;
- rework rate.

Output:
which work should be:
- manual;
- fixed robotic;
- flexible/adaptive robotic;
- mechanized SAW;
- not automated.

### M2 — Offline robot programming
Pilot CAD-based programming on current/new robot cell.

Goal:
reduce teach-pendant/programming downtime and make small-batch work economic.

Candidates:
- Verbotics-type software;
- robot OEM offline tools;
- integrator solution.

### M3 — Seam sensing / adaptive control
Use:
- touch sensing;
- laser seam finding;
- seam tracking;
- fit-up measurement.

Goal:
handle real fabricated-part variation without excessive fixtures/manual touch-up.

### M4 — Weld data traceability
Capture per weld:
- weld ID;
- program/revision;
- current/voltage/wire/feed/travel;
- timestamp/operator/cell;
- video/vision where relevant;
- alarms/deviations;
- NDT result.

This becomes the manufacturing data foundation.

### M5 — Automated geometric inspection
3D laser/vision:
- bead geometry;
- undercut/concavity;
- size;
- fit-up;
- joint mismatch;
- GO/NO-GO;
- permanent inspection record.

This supplements rather than replaces required certified NDT.

### M6 — Automated / mechanized NDT
Where codes and geometry permit:
- PAUT;
- TOFD;
- encoded UT;
- robotic/mechanized scanning.

Targets:
- faster full weld coverage;
- permanent digital records;
- reduce radiography disruption where allowed;
- reduce manual scanner variability.

### M7 — Large-weldment 3D dimensional QA
CAD-linked scanning before:
- trial assembly;
- machining;
- customer acceptance.

Goal:
find distortion/dimensional issues before they become expensive rework.

### M8 — Manufacturing intelligence
Digital/NEOS layer:
- cell OEE;
- arc-on time;
- program/changeover time;
- defect/rework;
- NDT findings;
- robot vs manual economics;
- predictive maintenance;
- cross-factory benchmarking.

## Candidate internal owners

| Layer | KONČAR owner |
|---|---|
| Welding process / qualifications | KMK + KTK + D&ST |
| Manufacturing engineering | respective plants |
| NDT / quality | KMK + KTK + Institute where relevant |
| Robot cell | plant + automation integrator |
| CAD/PLM integration | plant engineering + Digital |
| Data platform | Digital + NEOS |
| AI/analytics | NEOS + Digital |
| Business case / rollout | KONČAR Group operations + plant management |

## Gap classification

### G0 native
- welding expertise;
- certified personnel;
- NDT;
- CAD/3D designs;
- robotic welding experience;
- automatic SAW;
- large-part handling;
- quality systems.

### G1 adjacent
- manufacturing data platform;
- cross-cell analytics;
- digital traceability;
- predictive equipment analytics.

### G2 build/integrate
- CAD-to-robot workflow at scale;
- part robotability classifier;
- standardized weld-data model;
- automated quality record;
- integration with MES/ERP/PLM.

### G3 partner
- robot/positioner hardware;
- seam-vision sensors;
- offline programming software;
- PAUT/TOFD scanner;
- 3D metrology hardware;
- initial application engineering.

### G4 acquire
No acquisition justified at this stage.

### G5 blockers
Potential:
- customer procedure qualification / approval after welding-process changes;
- standards/traceability requirements;
- KTK JV data/governance;
- low utilization if part-family selection is poor.

## Pilot A — highest confidence

### Existing CLOOS cell utilization expansion
Before buying anything:
1. measure current arc-on/OEE;
2. map all parts currently run;
3. identify rejected candidate parts and reason;
4. quantify programming/fixturing/changeover bottleneck;
5. introduce offline programming on 2–3 high-labour short-run families;
6. compare manual vs robot total cost.

This leverages sunk capital and gives fastest evidence.

## Pilot B — KTK adaptive welding cell

Choose one tank subassembly family with:
- meaningful annual volume;
- substantial weld hours;
- manageable access;
- fit-up variation;
- expensive manual repositioning.

Test:
- offline CAD programming;
- positioner;
- seam sensing;
- digital process capture.

Do not start with the largest/most unique whole tank.

## Pilot C — digital QA/NDT

For a weld family with substantial inspection time:
- 3D surface inspection and/or mechanized PAUT/TOFD;
- compare inspection cycle time;
- defect detection;
- repeatability;
- digital traceability;
- customer/code acceptance.

## Economics model

Required inputs:
- welder fully loaded hourly cost;
- robot/cell/operator cost;
- programming hours;
- fixturing;
- arc-on time;
- reposition/crane time;
- NDT hours;
- rework/leak failures;
- throughput constraint value;
- contribution margin of additional units delivered;
- capex + maintenance.

### Important rule
ROI should be calculated on **additional contribution margin / bottleneck capacity released**, not only labour savings.

If a transformer-tank factory is demand constrained by welding capacity, releasing one bottleneck hour may be worth far more than one labour hour.

## External commercialization path — optional

Do not make this the initial objective.

Possible later products if internal deployment creates defensible knowledge:
- transformer-tank automation methodology;
- weld digital-thread software/templates;
- AI-assisted welding/quality models;
- engineering/integration services.

But generic robot integration is already a competitive industrial-automation market. KONČAR should only sell externally if it has unique domain IP.

## Evidence state

- Market technology: E3.
- KONČAR capability fit: E4.
- Internal ROI: not validated.
- External business opportunity: E0/E1 until internal repeatability and buyer demand are proven.

## Validation gates

1. actual welding-hour Pareto from KMK/KTK;
2. CLOOS OEE/utilization;
3. programming/fixture/changeover data;
4. KTK line layout and bottleneck map;
5. NDT cycle-time/rework data;
6. standards/customer-approval constraints;
7. pilot vendor quotations;
8. first internal ROI model.

## Linked evidence

- [B004](../benchmarks/B004_adaptive_welding_automated_ndt_smart_fabrication_2026-09-21.md)
- [E015 Metal Structures](../entities/E015_metal_structures.md)
- [E016 Transformer Tanks](../entities/E016_transformer_tanks.md)
- [E007 D&ST](../entities/E007_distribution_special_transformers.md)
- [E001 Institute](../entities/E001_electrical_engineering_institute.md)
- [E002 Digital](../entities/E002_koncar_digital.md)
- [E003 NEOS](../entities/E003_neos_capability_lineage.md)

## Next action

Request/derive the manufacturing Pareto and build the first **factory bottleneck + ROI model** before recommending new capex.
