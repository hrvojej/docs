# CURRENT CONTEXT — load this first

**Program:** KONČAR Strategic Technology & New Business Research  
**As-of:** 2026-09-21  
**Status:** foundation + Group/capability baseline + E001–E019 + B001–B005 + O001–O005 candidates

## Objective

Identify realistic new products, services and business models that KONČAR Group could profitably commercialize by intersecting:

**existing KONČAR industrial / engineering / manufacturing / digital / R&D / service assets**

with

**global technologies and business models that are already commercially proven or sufficiently mature for industrial adoption.**

The program is deliberately broader than AI, ROVs or robotics. Those are opportunity families, not the starting assumption.

## Current strategic picture

### 1. Group perimeter
Current corporate material says KONČAR consists of the parent, **16 subsidiaries**, plus **one affiliated/joint-venture company with Siemens Energy**. Reconciliation of Q1 2026 consolidation data with Jul/Aug 2026 status changes yields the current direct-subsidiary baseline in R001.

### 2. 2026 restructuring matters
Capabilities cannot be inferred from legal entities alone:
- KONČAR – Electronics and Informatics (INEM) was reorganized and then merged into KONČAR Inc.;
- its **Power Supply** business unit was separated into KONČAR – Helb before the final merger;
- the **Assembly** business unit was also incorporated into HELB;
- Prosperus Growth NEOS and KREANCA SUSTAVI were merged into KONČAR – Digital;
- KONČAR completed acquisition of the remaining HELB shares and became 100% owner.

Therefore this repository tracks both **legal ownership** and **capability lineage**.

### 3. AI/data capability is already in-house
The Group is not starting from zero:
- **KONČAR – Digital** has documented R&D in AI/ML, edge/cloud analytics, predictive maintenance and AI integration with SCADA-related systems;
- **KONČAR – Electrical Engineering Institute** has proprietary condition-monitoring products and ML-based automatic clustering/classification of partial-discharge faults;
- **NEOS** has an explicit Data Science practice covering advanced analytics, ML and AI, data engineering capabilities, automated time-series forecasting work and the AI Defender R&D project.

Implication: future opportunities should test how these capabilities can be attached to KONČAR domain hardware, installed base and service operations rather than assuming the Group must first acquire generic AI capability.

### 4. Core cross-group assets visible already
- power equipment and installed-base domain knowledge;
- large-scale industrial manufacturing;
- EPC / construction / commissioning;
- field service and lifecycle maintenance;
- electrical-engineering R&D, labs, testing and diagnostics;
- embedded/control/power-electronics lineage;
- software, SCADA, OT/IT, data engineering, analytics and cybersecurity;
- rail/mobility domain;
- hydro and renewable-energy domain;
- international export and project footprint.

### 5. Concrete capability signals found in entity baseline
- Institute: proprietary TMS/MCM/EMCM/iPDCore monitoring and ML-assisted diagnostics; 9 laboratories and broad testing/certification capability.
- Electric Vehicles: BEMU/BMU development, fleet-maintenance capability and a measurement-train reference.
- Metal Structures / Transformer Tanks: large welded-manufacturing footprint, machining, NDT and quality-control environments suitable for automation/CV benchmarking.
- HELB + TELENERG + Dalekovod: field deployment, testing/commissioning, protection/control and infrastructure access.
- former INEM lineage: power electronics, converters, embedded/protection/control capability that must be traced after the 2026 reorganization.
- D&ST / KPT / Generators & Motors / Switchgear / Instrument Transformers: large equipment domains with lifecycle/monitoring adjacency.
- Hydro Turbine / Renewables: direct operating/service environments relevant to autonomous inspection, predictive O&M and remote operations research.

### 6. First outside-in result — transformer intelligence
[B001](benchmarks/B001_transformer_asset_intelligence_2026-09-21.md) establishes transformer asset intelligence/predictive lifecycle services as a mature E3 commercial category.

Key market pattern:
- monitoring hardware is increasingly only the entry layer;
- leading vendors combine sensors/edge + fleet APM + remote experts + multi-year SLA/performance contracts;
- 2026 Siemens Energy–Camlin transaction is a major validation signal for grid monitoring/analytics/asset-digitalization value.

Important KONČAR finding:
- Institute TMS is already vendor-independent, retrofit-capable and internationally deployed;
- it already includes condition models, remote access, reporting and condition-based-maintenance functions;
- Institute reporting cites 780 delivered online monitoring systems in 64 countries and >60,000 MVA monitored by TMS.

Therefore the first identified gap is more likely **productization/servitization** than core monitoring technology.

This produced [O001 — KONČAR Transformer Intelligence & Lifecycle Service](opportunities/O001_transformer_intelligence_lifecycle_service.md), currently market E3 / KONČAR fit E4 / commercial E5 pending.

### 7. Second outside-in result — autonomous grid/substation inspection
[B002](benchmarks/B002_autonomous_grid_substation_inspection_2026-09-21.md) establishes autonomous/remote grid inspection as a mature E3 category.

Commercial evidence includes:
- AEP / Skydio: emergency substation inspection case with ~USD 8m reported savings and move toward docked autonomous inspection;
- SCE: >100 drones with docked systems scaling across grid assets;
- FPL / Percepto: statewide autonomous drone-in-a-box rollout;
- RTE / ANYbotics: autonomous ground-robot inspections in high-voltage environments;
- SSEN / Cyberhawk: inspection/asset-data workflow across >11,500 towers and ~150 substations.

Important KONČAR finding:
**Dalekovod-Projekt already uses drones, optical, thermal and laser cameras for maintenance documentation and condition analysis of operating power facilities.**

Therefore the likely gap is not basic drone capture. It is:
- persistent autonomy/docks;
- BVLOS operating capability;
- grid-specific CV/defect workflow;
- longitudinal asset history;
- SCADA/GIS/EAM/work-order integration;
- recurring managed service.

This produced [O002](opportunities/O002_grid_inspection_intelligence_service.md). Initial strategy: own the grid-domain intelligence/service layer and partner for drone/robot hardware.

### 8. Third outside-in result — hydro / underwater inspection
[B003](benchmarks/B003_hydro_underwater_inspection_2026-09-21.md) separates two maturity levels:

**Commercially mature:** ROV visual/sonar inspection of intakes, gates, trash racks, turbines/runners, draft tubes and submerged dam structures.

Evidence:
- Ontario Power Generation moved runner inspection from a six-person diver workflow to a two-person ROV crew;
- ESB Ireland has an ongoing ROV programme across most hydro sites;
- VideoRay/US Bureau of Reclamation and multiple contractor cases show repeatable operational use.

**Less mature / higher technical difficulty:** long flooded penstocks, reliable localization and quantitative robotic NDT. ENGIE/SHEM publicly documented a 2023 ROV trial that failed its ~400 m objective because of pressure/tether constraints; robotic EMAT work continued in 2026.

KONČAR implication:
Hydro Turbine already has diagnostic measurements, commissioning, maintenance and refurbishment capability. The first commercial move should therefore be **partner ROV + KONČAR hydro engineering + lifecycle repair path**, not proprietary ROV development.

This produced [O003](opportunities/O003_hydro_underwater_inspection_lifecycle_service.md). Proprietary underwater robotics remains an R&D option only if recurring customer jobs expose a high-value unsolved problem.

### 9. Fourth outside-in result — adaptive heavy fabrication
[B004](benchmarks/B004_adaptive_welding_automated_ndt_smart_fabrication_2026-09-21.md) shows that high-mix/low-volume heavy fabrication can now be automated much further through offline CAD programming, seam sensing, adaptive vision, digital weld traceability and mechanized NDT.

KONČAR-specific proof is unusually strong:
- KMK already has a CLOOS robotic welding cell and published an approximately **3× welding-speed improvement** on an applicable repeatable assembly, with NDT-confirmed consistency;
- KTK's new factory produces very large custom transformer tanks from 3D models and already operates under demanding VT/PT/MT/UT quality workflows.

External benchmarks show:
- IFH: 25–40% higher throughput on ~25 larger tank models after robotic/offline-programming expansion;
- Verbotics/TRT: one-off/high-mix parts made economically robotizable via CAD-based programming;
- commercial adaptive seam vision, automated geometric inspection, PAUT/TOFD and large-weldment 3D QA are available.

This produced [O004](opportunities/O004_adaptive_heavy_fabrication_program.md), an **internal-first** opportunity: release bottleneck capacity and scarce skilled labour before considering external commercialization.

### 10. Fifth outside-in result — rail fleet / battery / charging intelligence
[B005](benchmarks/B005_rail_fleet_battery_infrastructure_intelligence_2026-09-21.md) confirms a mature rail-digital lifecycle market: OEMs combine telemetry, predictive maintenance and digital workflows with multi-year/full-lifecycle service contracts.

Key market evidence:
- Alstom HealthHub: 100+ projects and 18k+ cars monitored;
- Hitachi HMAX: 2,000+ trains / 200,000 systems;
- Siemens Railigent X: long-term predictive-maintenance contracts, including a 2026 battery-train deal for 61 Mireo Plus B units with service up to 30 years;
- ABB traction batteries: remote condition monitoring + performance warranty + SLA.

KONČAR-specific evidence is strong and current:
- BEMU/BMU/EDMU portfolio;
- battery trains and charging stations in operation/contracts;
- 2026 contract for 6 additional BEMUs and hybrid Kotoriba charging station with PV + storage;
- existing long-term rolling-stock maintenance;
- KONČAR has publicly stated it is already **developing a centralized platform for system-wide coordination** of battery-rail operations/charging.

This produced [O005](opportunities/O005_rail_fleet_battery_intelligence_service.md): vehicle health + battery SOH/RUL + charging orchestration + predictive maintenance + lifecycle SLA.

Important boundary: the measurement train does not automatically give KONČAR infrastructure-measurement IP. MERMEC installed proprietary measurement systems, so data/algorithm rights must be validated separately.

### 11. Strategic constraint to keep in mind
2026 corporate reporting points to **production capacity and availability of qualified specialist personnel** as important growth constraints. New opportunities should therefore be evaluated not only on revenue potential but also on whether they:
- increase lifecycle/software/service revenue;
- leverage installed base and existing channels;
- create high value without proportionally consuming scarce factory capacity;
- or justify capacity investment through strong margin/export potential.

## Current research artifacts

### Cross-cutting research
- **R001** — [Current Group Structure & Ownership](research/R001_current_group_structure_2026-09-21.md)
- **R002** — [In-house AI, Data & Advanced Analytics](research/R002_inhouse_ai_data_capabilities_2026-09-21.md)
- **R003** — [Cross-Group Capability Atlas](research/R003_capability_atlas_baseline_2026-09-21.md)

### Entity/capability dossiers
- **E001–E019 baseline v1** exist for all current direct subsidiaries, KPT affiliate and key capability-lineage nodes.
- Browse: [entities/README.md](entities/README.md)

### External benchmarks
- **B001** — [Transformer Asset Intelligence & Predictive Lifecycle Services](benchmarks/B001_transformer_asset_intelligence_2026-09-21.md)
- **B002** — [Autonomous Grid & Substation Inspection](benchmarks/B002_autonomous_grid_substation_inspection_2026-09-21.md)
- **B003** — [Hydropower Underwater Inspection, ROV & Robotic NDT](benchmarks/B003_hydro_underwater_inspection_2026-09-21.md)
- **B004** — [Adaptive Robotic Welding, Automated NDT & Smart Heavy Fabrication](benchmarks/B004_adaptive_welding_automated_ndt_smart_fabrication_2026-09-21.md)
- **B005** — [Rail Fleet, Battery & Infrastructure Intelligence](benchmarks/B005_rail_fleet_battery_infrastructure_intelligence_2026-09-21.md)

### Opportunity candidates
- **O001** — [KONČAR Transformer Intelligence & Lifecycle Service](opportunities/O001_transformer_intelligence_lifecycle_service.md)
- **O002** — [KONČAR Grid Inspection Intelligence & Remote Inspection Service](opportunities/O002_grid_inspection_intelligence_service.md)
- **O003** — [KONČAR Hydro Underwater Inspection & Lifecycle Service](opportunities/O003_hydro_underwater_inspection_lifecycle_service.md)
- **O004** — [KONČAR Adaptive Heavy Fabrication & Digital Quality Program](opportunities/O004_adaptive_heavy_fabrication_program.md)
- **O005** — [KONČAR Rail Fleet & Battery Intelligence Lifecycle Service](opportunities/O005_rail_fleet_battery_intelligence_service.md)

### Complete registry
- [MASTER_INDEX.md](MASTER_INDEX.md)

## What is NOT yet concluded

- No product opportunity has yet been declared commercially attractive.
- No ROV/robotics thesis is privileged over other opportunities.
- No market-size or margin claim is considered validated yet.
- Detailed current ownership of some indirect subsidiaries after the summer-2026 mergers still requires registry-level reconciliation.
- E001–E019 are **baseline dossiers**, not exhaustive deep dives: team size, IP/patents, installed-base data, exact software stacks, customer references, economics and current internal organization still need deeper validation where relevant.
- B001–B005 are complete; renewable O&M/BESS benchmark remains pending.
- O001–O005 are candidate theses/programs, not validated business cases/ROI cases. Customer willingness-to-pay, pricing, internal ownership, service economics and pilot assets still require validation.

## Next research sequence

1. Deepen the highest-leverage E### dossiers with patents, projects, deployed products, customers, team/stack and installed-base evidence.
2. Resolve the remaining indirect-ownership/legal-lineage questions in R001.
3. Continue **B### outside-in commercial benchmarks**:
   - ✅ B001 equipment intelligence / predictive lifecycle service;
   - ✅ B002 autonomous grid/substation inspection;
   - ✅ B003 hydro / underwater inspection and maintenance;
   - ✅ B004 industrial CV / robotic NDT / smart manufacturing;
   - ✅ B005 rail/battery/fleet/measurement intelligence;
   - next: renewable O&M / inspection / forecasting / BESS optimization.
4. Validate O001–O003 commercially, O004 through factory bottleneck/OEE/ROI data, and O005 by deep-diving the centralized coordination platform/BMS/data rights.
5. Generate further O### theses only where market evidence and internal capability intersect.
6. Perform stack-level gap analysis + build/partner/acquire.
7. Validate economics and pilot paths.

## Repository protocol

Every new research output must be registered in [MASTER_INDEX.md](MASTER_INDEX.md).  
If a result changes the strategic picture, this file must also be updated.  
Each material research/chat session gets an S### capsule so a future chat can reconstruct why the current state looks the way it does.
