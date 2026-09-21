---
benchmark_id: B004
title: Adaptive Robotic Welding, Automated NDT & Smart Heavy Fabrication
status: complete-v1
as_of: 2026-09-21
evidence: high-commercial-core_medium-emerging-ai
tags: [welding, robotics, ndt, computer-vision, heavy-fabrication, high-mix-low-volume, quality, productivity]
---

# B004 — Adaptive Robotic Welding, Automated NDT & Smart Heavy Fabrication

## Scope

Outside-in benchmark of automation technologies relevant to KONČAR's large, custom, welded manufacturing environments, especially:

- KONČAR – Metal Structures (KMK);
- KONČAR – Transformer Tanks (KTK);
- Distribution & Special Transformers (D&ST);
- selected rail/generator structural production.

This benchmark deliberately focuses on **high-mix / low-volume / engineering-to-order heavy fabrication**, not automotive-style mass production.

Technology layers assessed:

1. robotic / cobot welding;
2. offline CAD-based robot programming;
3. seam finding / seam tracking / adaptive welding;
4. weld process data and traceability;
5. automated surface weld inspection / 3D vision;
6. mechanized/robotic volumetric NDT (PAUT/TOFD/UT);
7. large-weldment dimensional inspection / 3D metrology;
8. AI-assisted/adaptive welding.

## Executive conclusion

This is a commercially mature automation category with one important shift:

> robotics is moving from fixed, high-volume cells toward **high-mix, low-volume adaptive fabrication** through CAD/offline programming, sensing, vision and flexible positioning.

For KONČAR, this is not a greenfield concept.

**KONČAR – Metal Structures already has a CLOOS robotic welding station** and publicly reported:
- threefold welding-speed improvement on a repeatable assembly;
- one manual welder previously required ~8 hours for one assembly;
- the robot produced three assemblies in the same period;
- stable quality confirmed by NDT;
- operation in two shifts;
- use on transformer-tank components plus train, tram and generator components.

Therefore the research question is not:
> should KONČAR adopt robotic welding?

It is:
> how much of today's high-mix, custom heavy fabrication can be shifted from manual dependence to CAD-driven/adaptive automation and automated quality control?

That is primarily an **internal capacity/profit opportunity** at first. External commercialization should be considered only if KONČAR develops reusable IP/process expertise beyond its own factories.

## Market layer A — high-mix / low-volume robotic welding

### 1. Miller / IFH Group — tank fabrication

IFH manufactures made-to-order hydraulic and fuel tanks in:
- steel;
- aluminum;
- stainless steel;
- frequent changeovers;
- increasingly large/heavy variants.

Automation architecture:
- six Miller PerformArc robotic cells;
- positioners;
- touch sensing;
- CAD/offline programming via IntelliPath;
- engineering/quality/production/automation joint launch process.

Reported results:
- ~25 larger tank models moved from manual to robot cells;
- **25–40% throughput increase** on those tanks;
- on-cell programming that could take ~15 hours reduced to ~2–3 hours touch-up after offline preparation;
- some prototype programs reach cell readiness with ~1 hour at the robot rather than days;
- 3–4 manual tank flips replaced on applicable work by automated positioning;
- fewer leak issues reported on automated tank families.

Important lesson:
**offline programming and positioning—not the robot arm alone—make high-mix tank automation viable.**

Source:
- https://www.millerwelds.com/en-us/case-studies/how-ifh-group-increased-throughput-with-robotic-welding-automation

### 2. Verbotics / TRT — one-offs and short runs

TRT produces road-transport/construction assemblies with high mix and low volume.

Constraint:
traditional robot teach programming was too slow for their mix.

Verbotics Weld:
- generates robot programs from digital models;
- automatic sensing verifies weld placement;
- supports simulation/collision checking.

Reported results:
- ~4 hours offline programming → ~36 hours robot welding;
- ~10:1 robot-running-to-programming ratio;
- ~100–350 m welding per 12-hour shift depending on complexity;
- two new programs/week;
- designed to make one-off parts practical for robotic welding.

Source:
- https://verbotics.com/news/2022-08-02-trt-case-study/
- https://verbotics.com/

### 3. Path Robotics — very large tank automation

Path Robotics publicly shows a dual-arm autonomous generator-tank welding cell rated for:
- parts up to **55,000 lb**;
- **60 ft** long;
- **15 ft** wide.

The vendor explicitly positions this class as historically difficult to automate because of:
- part size;
- fit-up;
- part-to-part variation;
- expensive fixturing.

The cell demonstrates that physically large tank-like structures are no longer automatically outside the automation envelope.

Source:
- https://www.path-robotics.com/videos/generator-tank-welding-cell-factory-acceptance-test

### 4. KUKA / fabricated steel structures

KUKA case material for structural fabrication shows flexible robotic cells using:
- articulated robot;
- linear axis;
- rotary positioners;
- Fronius welding equipment;
- multiple frame/component variants.

Reported case improvements of 200–300% production efficiency should be treated as vendor/customer-case evidence, not generic guaranteed ROI.

## Market layer B — seam sensing and adaptive welding

Traditional robot programs assume repeatable geometry. Heavy fabricated assemblies violate that assumption through:
- fit-up variation;
- tack position;
- thermal distortion;
- joint tolerances;
- large-part positioning.

Commercial solutions address this with:

### SERVO-ROBOT
3D laser-vision systems support:
- seam finding;
- real-time seam tracking;
- adaptive robot path correction;
- pre/post weld measurement;
- weld inspection;
- 3D mapping.

Examples:
- QUICK-SCAN;
- i-CUBE-T;
- POWER-TRAC;
- DIGI-LAS.

Sources:
- https://servo-robot.com/
- https://servo-robot.com/arc-seam-finding/
- https://servo-robot.com/laser-seam-tracking/

### Novarc / NovAI

NovAI combines:
- weld-pool video;
- welding parameters;
- computer vision;
- operator-guided control;
- AI-driven adaptive welding.

Current public positioning spans:
- Capture: traceability/video/parameters;
- Control: operator-in-loop adjustment;
- Autonomy: automatic adaptation to seam position, tacks, root opening and fit-up variation.

This is an important **emerging layer**, but vendor claims of AI autonomy should not be treated as equivalent to broad production maturity across all heavy-fabrication geometries.

Sources:
- https://www.novarctech.com/products/novai/
- https://www.novarctech.com/products/novai/novai-capture/
- https://www.novarctech.com/products/novai/novai-autonomy/

## Market layer C — automated visual / geometric weld inspection

### SERVO-ROBOT weld inspection

Commercial 3D laser vision can:
- map weld bead geometry;
- measure joint/weld features;
- detect geometric defects;
- compare to tolerances;
- generate GO/NO-GO;
- create digital/paperless inspection records.

Products include:
- ARC-SCAN;
- LAS-SCAN;
- WiKi-SCAN.

This is not a replacement for volumetric NDT where codes require it, but it can:
- automate high-frequency surface/geometric inspection;
- support process capability analysis;
- reduce redundant manual gauging;
- improve traceability.

Sources:
- https://servo-robot.com/arc-weld-inspection/
- https://servo-robot.com/laser-weld-inspection/
- https://servo-robot.com/wiki-scan-a-revolution-in-weld-quality-management/

## Market layer D — automated / mechanized volumetric NDT

### Eddyfi — PAUT / TOFD

For large welds such as wind-tower/monopile structures, Eddyfi offers mechanized:
- phased-array ultrasonic testing (PAUT);
- TOFD;
- encoded scanning;
- permanent digital records.

Use case characteristics:
- welds up to ~35 m;
- wall thicknesses up to ~130 mm in cited monopile application;
- code-compliant full volumetric examination;
- mechanized scanner carrying multiple probes.

Important market logic:
encoded UT can replace disruptive radiography in applicable code contexts, reducing:
- radiation exclusion constraints;
- manufacturing disruption;
- inspection time.

Eddyfi NAV2 and related systems can scan:
- circumferential;
- longitudinal;
- flat/curved welds;
and can be interfaced to a robot/integrator.

Sources:
- https://www.eddyfi.com/en/appnote/mechanized-paut-and-tofd-inspection-techniques-for-monopile-and-wind-tower-welds
- https://www.eddyfi.com/en/preview/products/202/2/en/product/automated-inspection-solutions
- Eddyfi automated weld-inspection brochure / NAV2 materials.

### IRELEC / Testia
Robotic UT has also been engineered for high-consequence components such as ITER first-wall panel welds, demonstrating robot-positioned NDT in demanding low-volume/high-value manufacturing.

Source:
- https://www.irelec-alcen.com/case-study/robot-ut-alsymex/

## Market layer E — large-weldment dimensional inspection

### Creaform / Xtreme Manufacturing

Large/heavy weldment inspection case:
- manual dimensional inspection was slow;
- defects sometimes reached assembly and caused rework/delay;
- handheld large-volume 3D scanning used CAD-linked inspection;
- inspection files correlate measured geometry directly to design intent.

This is relevant to KONČAR because large custom welded structures often require both:
- weld quality;
- global dimensional conformance after welding/distortion.

Source:
- https://www.creaform3d.com/en/resources/blog/how-xtreme-manufacturing-improved-quality-and-inspection-efficiency-using-the-handyscan-3d-max-series

## KONČAR current capability baseline

### KONČAR – Metal Structures

Current official facts:
- advanced large welded components for energy, transport and industry;
- transformer tanks historically ~70% of production capacity;
- >400 employees;
- >EUR 31m annual revenue;
- ~71.8% export share;
- ~4.75m kg annual output;
- two major production sites;
- certified welding coordinators/welders and NDT inspectors;
- large cranes, machining, cutting, blasting and corrosion protection;
- rail components under EN 15085 CL1;
- nuclear-grade/high-quality welded structures.

Existing automation:
- automatic submerged-arc-welding portal;
- CLOOS robotic welding station;
- published 3× welding-speed result on applicable repeatable work.

Sources:
- https://koncar.hr/en/kmk/about-us
- https://www.koncar.hr/en/kmk/manufacturing-capacities
- https://koncar.hr/en/kmk/quality-and-certifications
- https://koncar.hr/en/kmk/news/investments-welding-technology
- https://koncar.hr/hr/kmk/komponente-tracnickih-vozila

### KONČAR – Transformer Tanks (KTK)

Current official facts:
- custom transformer tanks exceeding 100 t;
- steel + stainless + aluminum + copper;
- MAG/MIG/TIG/EPP welding;
- VT/PT/MT/UT and leak/pressure testing;
- 3D model/drawing-driven production;
- trial assembly and dimensional checks;
- continuous Quality Control + Technical Office oversight;
- new state-of-the-art factory opened Jan 2026;
- global OEM customers including Siemens Energy, Hitachi Energy, GE Grid Solutions, Royal SMIT, Kolektor Etra and Hyosung.

Pre-opening planning material cited >400 future employees and ~160 custom tanks/year; these figures should be revalidated against operating ramp rather than assumed as current production.

Sources:
- https://www.koncar.hr/en/ktk/transformer-tanks
- https://koncar.hr/en/news/croatia-gains-new-production-center-for-global-energy-transformer-market
- KONČAR 2025 investment notice for KTK capacity plan.

### D&ST
Distribution-transformer manufacturing already uses automated:
- core cutting lines;
- winding machines;
and high-throughput production.

The B004 focus for D&ST is more likely targeted weld/inspection/dimensional automation rather than generic factory automation.

## Maturity assessment

| Technology | Commercial maturity |
|---|---|
| Fixed robotic welding for repeat parts | E3+ mature |
| Offline CAD programming for high-mix | E3 mature |
| Touch/laser seam finding/tracking | E3 mature |
| Adaptive heavy-fabrication welding | E2/E3, increasingly commercial |
| Weld data capture / traceability | E3 |
| 3D laser geometric weld inspection | E3 |
| Mechanized PAUT/TOFD weld NDT | E3 for suitable geometries/codes |
| Large-weldment 3D dimensional QA | E3 |
| AI closed-loop autonomous welding | E2/E3 emerging |
| Fully lights-out one-off heavy fabrication | E1/E2 depending complexity |

## KONČAR gap analysis

| Layer | KONČAR evidence | Gap |
|---|---|---|
| Welding engineering / IWE/EWE competence | strong | G0 |
| Manual high-quality fabrication | strong | G0 |
| NDT competence | strong | G0 |
| Automatic SAW | existing | G0 |
| Fixed robotic welding | existing CLOOS | G0 |
| CAD/3D engineering models | explicit KTK | G0 |
| Offline programming at scale | not evidenced | G1/G2 |
| Automatic seam finding/tracking | not evidenced | G2/partner |
| Adaptive vision welding | not evidenced | G2/G3 |
| Weld-parameter/data traceability platform | unclear | G1/G2 |
| Automated geometric weld inspection | not evidenced | G2/G3 |
| Mechanized PAUT/TOFD in production flow | not evidenced | G2/G3 |
| Automated 3D dimensional inspection | not evidenced | G2/G3 |
| Closed-loop AI weld adaptation | not evidenced | G3 / pilot |
| Cross-factory data/analytics layer | Digital/NEOS adjacent | G1 |
| Product-selection analytics: manual vs robot | likely process know-how, digital decision support not evidenced | G1/G2 |

## Strategic implication

This is different from O001–O003 because the first profit pool may be **internal operating leverage**, not an external service.

KONČAR faces strong transformer/global equipment demand and has publicly disclosed a very large capacity-expansion investment cycle. Skilled specialist labour and factory capacity are strategic constraints.

For this environment, a 10–30% improvement in effective welding/inspection throughput in selected bottlenecks may be economically more valuable and less commercially risky than launching a brand-new external product.

This benchmark therefore supports an **internal-first O004**.

## What KONČAR should not do first

- Do not buy robots without analysing part families and programming economics.
- Do not assume every custom structure should be automated.
- Do not lead with generic “AI for welding”.
- Do not attempt to replace certified welding/NDT engineering judgment where standards require qualified personnel.
- Do not build proprietary robot arms, scanners or NDT instruments before proving a gap.
- Do not centralize automation so rigidly that factory-specific welding qualifications/customer rules are lost.

## High-value pattern

A likely scalable architecture is:

**3D/CAD model → automatic weld extraction → manufacturability/robotability decision → offline path/program → seam sensing/adaptive correction → welding → geometric inspection → NDT where required → digital quality record**

The differentiating Group asset would be the **digital thread and process know-how across multiple high-quality fabrication plants**, not the robot hardware.

## Evidence level

- high-mix robotic welding: E3 commercial;
- automated geometric inspection: E3;
- mechanized PAUT/TOFD: E3;
- adaptive/AI welding: E2–E3;
- KONČAR fit for internal deployment: E4 because relevant plants, welding competence and prior robot results exist.

## Open questions

1. How many current welding hours/year exist in KMK and KTK by process and part family?
2. Which weld families account for the top 20% of labour/bottleneck time?
3. Current robot utilization/OEE of the CLOOS station?
4. Why were other assemblies not migrated to robotic welding?
5. Is programming/fixturing the limiting factor?
6. Which CAD/PLM/MES systems are used?
7. Are weld IDs and parameters traceable digitally today?
8. What percentage of welds require VT/PT/MT/UT/RT?
9. Is PAUT/TOFD already used via subcontractors or internally?
10. Where does NDT create cycle-time bottlenecks?
11. What is rework/scrap/leak-test failure cost?
12. How much value is tied to large-part repositioning/crane time?
13. Can KTK's new factory support robotic cells/digital data without major retrofit?
14. What customer approvals are needed after process automation changes?
15. Is Siemens Energy JV governance/IP relevant to KTK automation data?

## Next validation

Create O004 as an internal-first capacity and quality program:
- part-family Pareto;
- robotability assessment;
- CLOOS utilization audit;
- CAD/offline-programming pilot;
- adaptive seam sensing pilot;
- automated NDT/3D QA pilot;
- first unit/throughput economics;
- external commercialization only after internal repeatability is proven.
