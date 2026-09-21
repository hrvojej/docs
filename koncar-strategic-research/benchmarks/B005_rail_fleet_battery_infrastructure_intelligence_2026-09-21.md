---
benchmark_id: B005
title: Rail Fleet, Battery & Infrastructure Intelligence
status: complete-v1
as_of: 2026-09-21
evidence: high-commercial
tags: [rail, predictive-maintenance, battery, charging, fleet, measurement-train, infrastructure, digital-services]
---

# B005 — Rail Fleet, Battery & Infrastructure Intelligence

## Scope

Outside-in benchmark of commercial rail digitalization relevant to KONČAR's current rail position:

1. rolling-stock condition monitoring / predictive maintenance;
2. maintenance workflow and lifecycle contracts;
3. traction-battery condition monitoring / performance guarantees;
4. fleet energy and charging coordination;
5. trainborne infrastructure measurement / inspection;
6. data platforms connecting vehicle, infrastructure and maintenance.

The analysis distinguishes:
- capabilities KONČAR can plausibly own end-to-end;
- areas where KONČAR currently supplies the vehicle but a specialist partner owns measurement technology.

## Executive conclusion

Rail OEMs increasingly monetize a lifecycle stack:

**vehicle → telemetry → predictive analytics → maintenance planning/work orders → depot/service operation → long-term availability contract**

For battery rail, this expands to:

**battery SOH/SOC → route/duty-cycle model → charging infrastructure → energy scheduling → performance warranty → lifecycle replacement/service**

This is a mature commercial category.

KONČAR has unusually strong adjacency:
- its own EMU/DEMU/BMU/BEMU/EDMU platforms;
- current battery trains in commercial service;
- 1 MW charging infrastructure;
- six charging stations in the initial green-rail program;
- a 2026 contract for six additional BEMUs plus a hybrid PV + storage charging station;
- a publicly announced **centralized platform under development for system-wide coordination**;
- long-term fleet maintenance capability;
- GPS/fleet-management functions already present in low-floor train product material;
- Digital/NEOS analytics/data capability.

This supports a concrete O005 opportunity around **fleet/battery/charging intelligence and long-term lifecycle service**.

The separate measurement-train opportunity is more constrained: KONČAR designed/built/certified the special vehicle, while **MERMEC installed its proprietary measurement systems**. Infrastructure analytics/data rights therefore cannot be assumed to belong to KONČAR.

## Market layer A — rolling-stock predictive maintenance

### Alstom HealthHub

HealthHub is a cloud-based predictive/condition-based maintenance platform covering:
- rolling stock;
- track;
- catenary;
- signalling.

Commercial scale:
- implemented in **100+ projects**;
- 18,000+ cars across 100+ fleets reported in current digital-services material;
- 15+ fleet support centres across 14 countries.

Functions:
- real-time asset health;
- algorithms/data science;
- predictive maintenance;
- maintenance planning;
- integration to Maintenance Management System;
- automatic work-order generation;
- non-Alstom asset support.

Alstom reports benefits up to:
- 20% material-cost reduction;
- 30% downtime reduction;
- 50% recurring-fault reduction.

These are vendor-reported outcomes and should not be treated as universal guarantees.

Commercial model:
HealthHub is often embedded into broader service/maintenance contracts.

Current example:
- GWR Class 175 eight-year service contract uses HealthHub;
- >200 train parameters transmitted every 30 seconds for real-time monitoring.

Sources:
- https://www.alstom.com/stories/future-services-digital-healthhub
- https://www.alstom.com/solutions/services/digital-railway-solutions-unlock-higher-asset-availability-reliability-and-performance
- https://www.alstom.com/press-releases-news/2025/8/alstom-signs-eight-year-services-contract-uk-support-gwr-class-175-fleet-reintroduction

### Siemens Mobility — Railigent X

Railigent X offers:
- Data-as-a-Service;
- Insights-as-a-Service;
- Software-as-a-Service;
- real-time vehicle data APIs;
- predictive maintenance;
- fleet monitoring;
- lifecycle/service integration.

Public Siemens performance positioning includes up to:
- 15% maintenance-cost reduction;
- 40% lower delay costs;
- improved reliability/availability.

Again these are vendor claims, not generic expected results.

Commercial examples:
- Northrail: up to 50 Vectron locomotives with 8-year full-service, option to 16 years, using Railigent X fleet monitoring.
- TX Logistik: 40 Vectrons, ~EUR 300m order, 15-year full-service, Railigent X predictive maintenance.
- 2026 North Westphalia: **61 battery Mireo Plus B trains + full-service contract up to 30 years**, using Railigent X O&M concept with near-100% availability target.

Sources:
- https://developer.siemens.com/railigent-x/overview.html
- https://developer.siemens.com/railigent-x/Streaming-Data-REST-API/StreamingAPI.html
- https://press.siemens.com/global/en/pressrelease/northrail-expands-fleet-50-new-vectron-locomotives
- https://press.siemens.com/global/en/pressrelease/siemens-mobility-receives-large-order-tx-logistik-ag
- https://press.siemens.com/global/en/pressrelease/siemens-secures-long-term-service-contract-61-battery-powered-trains-westphalia

### Hitachi Rail — HMAX

HMAX integrates:
- train data;
- signalling;
- infrastructure;
- third-party systems;
- digital twins;
- predictive maintenance;
- automatic maintenance work orders;
- edge AI.

Current scale:
- HMAX train solutions fitted to **2,000+ trains / 200,000 systems**.

Important strategic direction:
Hitachi is explicitly moving toward **“every train a measurement train”**:
- trainborne sensors inspect rolling stock and track/wayside infrastructure;
- edge AI filters data;
- regular passenger fleets supplement dedicated yellow/measurement trains.

Sources:
- https://www.hitachirail.com/products-and-solutions/digital-asset-management/
- https://www.hitachirail.com/products-and-solutions/digital-asset-management/hmax-for-trains/
- https://www.hitachirail.com/blog/hmax-for-rail-hitachi-rail-at-innotrans-2026/

### Railnova — OEM-neutral specialist

Railnova demonstrates an independent digital-services business:
- 3,500+ connected rail assets;
- ~420,000 km monitored daily;
- OEM/protocol/age-neutral;
- data sovereignty;
- telemetry + diagnostics + maintenance workflows;
- RailGenius predictive-maintenance software.

This matters because operators may buy digital fleet intelligence independently of the vehicle OEM.

Sources:
- https://www.railnova.eu/en
- https://www.railnova.eu/en/solutions
- https://www.railnova.eu/en/products/railgenius

## Market layer B — traction battery intelligence and performance service

### ABB

ABB commercial traction battery services provide:
- remote condition monitoring;
- fleet overview;
- health/performance analysis;
- proactive fault detection;
- service response;
- **performance warranty**;
- lifecycle service and SLA.

ABB explicitly frames digital monitoring as enabling performance guarantees across the battery lifecycle.

Sources:
- https://www.abb.com/global/en/areas/motion/traction-services/traction-digital-solutions
- https://www.abb.com/global/en/areas/motion/traction/traction-battery/pro
- https://www.abb.com/global/en/areas/motion/traction-services/traction-lifecycle-services

### Siemens battery-train service model

The 2026 Westphalia Mireo Plus B deal demonstrates the commercial endpoint:
- battery-electric fleet;
- digital O&M;
- maintenance responsibility;
- availability commitment;
- contract up to 30 years.

This is strategically more important than simply selling battery telemetry software.

## Market layer C — energy / charging optimization

Battery rolling stock introduces a system problem rather than just a vehicle problem:

Inputs:
- timetable/duty cycle;
- route electrification;
- state of charge;
- state of health;
- ambient conditions;
- passenger/load;
- charging-point availability;
- grid connection limits;
- electricity price;
- stationary storage/PV;
- service reserve.

Outputs:
- when/where/how much to charge;
- which vehicle serves which duty;
- battery stress/lifetime tradeoff;
- grid peak management;
- vehicle readiness.

Analogous commercial rail energy optimization exists in products such as Wabtec's energy-management systems, where route/operating conditions are used to optimize propulsion/energy decisions.

Wabtec battery-locomotive projects also use energy-management software to decide discharge/recharge timing.

Sources:
- https://www.wabteccorp.com/digital-intelligence/energy-management
- https://www.wabteccorp.com/digital-intelligence/energy-management/trip-optimizer
- https://www.wabteccorp.com/newsroom/press-releases/rio-tinto-orders-wabtec-flxdrive-battery-locomotives-to-reduce-emissions

## Market layer D — infrastructure measurement / inspection

### MERMEC

MERMEC offers a mature rail-infrastructure diagnostic stack:
- dedicated measurement trains;
- track geometry;
- rail profile/corrugation;
- ride quality;
- tunnel/clearance;
- catenary geometry/wear;
- thermal/electrical pantograph interaction;
- machine-vision track inspection;
- ultrasonic rail-flaw testing;
- data-analysis platforms TRACKWARE/RAMSYS.

V-CUBE:
- machine vision;
- detects >50 defect types;
- runs at speed;
- can be installed on diagnostic or revenue trains.

MERMEC also offers contracted inspection/data-analysis services.

Sources:
- https://www.mermecgroup.com/pageview.php?i=15
- https://www.mermecgroup.com/pageview2.php?i=524&sl=1
- https://www.mermecgroup.com/inspect/909/trackware.php
- https://www.mermecgroup.com/

## KONČAR current position

### Vehicle manufacturing / fleet
KONČAR Electric Vehicles:
- nearly 400 employees;
- >80 engineers/master's graduates;
- 55 low-floor EMUs and 5 DEMUs stated on current about page;
- broader current page reports 70 low-floor trains plus tram/locomotive references;
- long-term maintenance of trams, trains and locomotives for domestic and private leasing operators;
- Ministry-approved maintenance provider;
- workshops for repairs/maintenance;
- diagnostics and specialized measurements.

Sources:
- https://koncar.hr/en/kev/about-us
- https://www.koncar.hr/en/koncar-electric-vehicles

### Battery / hybrid train platform
Current development/product portfolio includes:
- BMU;
- BEMU;
- EDMU.

Important current milestones:
- battery train entered commercial service in 2025;
- optimal range ~100 km per charge, tests >200 km;
- 1 MW KONČAR charging stations, cited charge time ~27 minutes;
- six original charging sites;
- 2025 additional contract: 5 EDMU + 4 BEMU + 4 BMU + 2 charging stations, EUR 117.9m;
- July 2026: another **6 BEMU + hybrid Kotoriba charging station**, project value EUR 53.6m;
- Kotoriba station includes PV + energy storage;
- new BEMUs due 2028/early 2029.

Sources:
- https://koncar.hr/en/news/croatias-first-battery-train-officially-launched-service
- https://koncar.hr/en/news/hz-passenger-transport-expands-fleet-13-new-trains
- https://koncar.hr/en/kev/news/contracts-signed-for-6-new-bemus-and-construction-hybrid-charging-station-kotoriba-station

### Centralized platform already under development
In May 2025, KONČAR publicly stated that battery train + charging infrastructure creates predictable energy profiles and that it was **developing a centralized platform to enable system-wide coordination**.

This is direct evidence that O005 is not merely an external idea; some relevant product work is already underway.

Source:
- https://www.koncar.hr/en/kev/news/battery-electric-train-debuts-croatian-rails

### Existing fleet functionality
Current low-floor train product page includes:
- GPS positioning;
- fleet management;
- reduced maintenance-cost positioning.

Source:
- https://koncar.hr/en/kev/low-floor-trains

### Measurement train
KONČAR:
- designed;
- manufactured;
- delivered;
- certified
the measurement-train prototype.

But:
- **MERMEC installed its proprietary measurement systems**;
- end customer is HŽ Infrastructure.

HŽ Infrastructure states its vehicle measures:
- track/catenary video;
- track and catenary geometry;
- rail corrugation;
- ground/embankment radar;
- ultrasonic rail inspection.

The vehicle was reported at ~EUR 13m procurement value.

Sources:
- https://koncar.hr/en/kev/projects/delivery-measurement-train-prototype-mermec
- https://www.hzinfra.hr/na-innotransu-predstavljen-mjerni-vlak-hz-infrastrukture/

## Critical boundary — measurement train

Do not infer that KONČAR owns:
- MERMEC measurement algorithms;
- infrastructure defect models;
- HŽ Infrastructure data;
- track/catenary analytics IP.

Current evidence shows KONČAR's role as special-vehicle designer/manufacturer/certifier, with MERMEC owning/installing measurement systems.

Therefore infrastructure-intelligence productization requires:
- a MERMEC partnership;
- new in-house sensing/software development;
- or another partner/rights arrangement.

## KONČAR gap analysis — fleet/battery opportunity

| Layer | KONČAR evidence | Gap |
|---|---|---|
| Rolling-stock OEM | strong | G0 |
| Battery/BEMU vehicle integration | strong/current | G0 |
| Charging-station hardware | strong/current | G0 |
| Hybrid PV+BESS charging project | contracted | G0/G1 |
| Maintenance organization | existing | G0 |
| GPS/fleet management | product evidence | G0/G1 |
| Central coordination platform | explicitly under development | G1 active |
| Vehicle telemetry ingestion | likely but architecture not public | G1 |
| Battery SOH/SOC analytics | BMS exists implicitly, fleet analytics not evidenced | G1/G2 |
| Battery RUL / performance warranty analytics | not evidenced | G2 |
| Predictive maintenance across vehicle subsystems | not evidenced as product platform | G2 |
| Automatic maintenance work orders | not evidenced | G2 |
| Digital depot workflow | not evidenced | G2 |
| Charging optimization across timetable/grid/PV/BESS | central platform adjacency, exact optimization unclear | G1/G2 |
| Data platform / ML | Digital + NEOS | G1 |
| Long-term availability/performance contract | maintenance contracts exist; outcome model not evidenced | G1/G2 |
| Third-party fleet retrofit | modernization/service capability exists | G1/G2 |
| Track/catenary measurement algorithms | MERMEC-owned in current measurement train | G3/partner |

## Strategic inference

The strongest rail opportunity is not a generic “rail AI platform”.

It is a tightly integrated extension of KONČAR's battery/fleet business:

> **KONČAR Rail Fleet & Battery Intelligence: vehicle health + battery health + charging orchestration + maintenance workflow + long-term lifecycle service.**

This can start on KONČAR-owned/new vehicle platforms where data access is controllable.

It can later extend to:
- legacy KONČAR fleets;
- third-party fleets through retrofit/modernization;
- infrastructure sensing only where data/IP partnerships are clear.

## Competitive differentiation hypotheses

1. **Vehicle + charger + grid capability** in one Group.
2. **Battery train deployed locally**, giving a real development/reference fleet.
3. **Long-term maintenance organization** already exists.
4. **Digital/NEOS** can provide scalable data/analytics.
5. **Power electronics/control lineage** from former INEM.
6. Potential to integrate PV/BESS/grid constraints into charging orchestration.

These must be validated against customer willingness to pay and software maturity.

## Evidence level

- rail predictive/lifecycle digital service: E3 mature;
- traction battery monitoring/service: E3;
- rail energy optimization: E3 adjacent, battery-passenger-train orchestration narrower but commercially credible;
- KONČAR fit: E4 because vehicles, charging, maintenance and central-platform development are current;
- infrastructure measurement analytics fit: only E2/G3 due MERMEC dependency.

## Open questions

1. What telemetry is available from KONČAR EMU/BEMU/EDMU in production?
2. What is the architecture/status of the centralized coordination platform?
3. Which KONČAR company/team owns it?
4. Battery vendor/BMS supplier and data-access rights?
5. Is SOH/RUL calculated today?
6. Are charger, train and timetable data already integrated?
7. Does the platform optimize charging or only coordinate/monitor?
8. How are PV+BESS at Kotoriba dispatched?
9. What maintenance-management system does KEV use?
10. Can alerts automatically create work orders?
11. Can KONČAR offer battery performance/availability guarantees?
12. What current maintenance contract ARR/service margin exists?
13. Can legacy/third-party rolling stock be retrofitted without expensive homologation?
14. What MERMEC/HŽ data can KONČAR legally/technically access from the measurement train?
15. Could a passenger KONČAR fleet later act as infrastructure sensor carrier, Hitachi-style?

## Next validation

Create O005 and map:
- centralized-platform architecture;
- battery/BMS data rights;
- charging/PV/BESS optimization;
- fleet maintenance workflow;
- digital service packaging;
- pilot on current HŽPP battery fleet;
- long-term SLA/performance-contract economics.
