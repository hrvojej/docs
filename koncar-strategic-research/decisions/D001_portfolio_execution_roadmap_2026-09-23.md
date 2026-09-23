---
decision_id: D001
title: KONČAR Opportunity Portfolio — Execution Roadmap
as_of: 2026-09-23
status: recommended-execution-framework
inputs: [O001, O002, O003, O004, O005, O006]
basis: public-research-and-explicit-scenarios
budget_approved: false
pilots_executed: false
---

# D001 — KONČAR Opportunity Portfolio: Execution Roadmap

[MASTER_INDEX](../MASTER_INDEX.md) · [CURRENT_CONTEXT](../CURRENT_CONTEXT.md) · [O006 završna usporedba](../opportunities/O006_renewable_bess_intelligence_optimization_service.md#usporedba)

## 1. Svrha

Prevesti dovršeni research O001–O006 u praktičan portfolio rada.

Ovo nije odobren budžet, interni plan KONČAR-a niti tvrdnja da su resursi raspoloživi. To je preporučeni slijed izvedbe temeljen na javno potvrđenim kompetencijama, komercijalnim primjerima i scenarijskoj ekonomici iz O001–O006.

## 2. Portfolio logika

Šest prilika ne treba voditi kao šest jednakih novih projekata.

Najkorisnije ih je rasporediti u četiri različita tipa rada:

### A — Komercijalizirati postojeću osnovu
**O001 — Transformer monitoring + stručni servis**

Cilj: više ponavljajućeg prihoda iz već postojećeg TMS/dijagnostičkog proizvoda.

Ne graditi novi monitoring sustav. Standardizirati stručni paket, definirati komercijalni opseg i prodavati uz postojeće kupce/retrofit.

### B — Povećati internu produktivnost
**O004 — Adaptivno zavarivanje i digitalna kvaliteta**

Cilj: osloboditi stvarno usko grlo i povećati prihvaćenu/isporučenu proizvodnju.

Ne automatizirati tvornicu kao tehnološki program. Raditi jednu ćeliju / 2–3 obitelji proizvoda / jasno mjerljiv ukupni takt.

### C — Graditi vlastite strateške proizvode
**O005 — Rail/tram digital, ADAS, autonomni depo**
**O006 — Renewable/BESS intelligence + optimization**

To su dva područja gdje postoji smislen razlog za vlastiti KONČAR software/control/domain IP:
- O005 zbog vlastitih vozila, održavanja, SafeTram razvojnog traga i baterijskih vlakova/punionica;
- O006 zbog EMS/SCADA/KONBAT/renewables reference i tržišne integracije.

Ne razvijati generičku platformu. Razvijati ponovljive domenske proizvode.

### D — Prodavati kao partnerski servis
**O002 — Grid inspection**
**O003 — Hydro/ROV inspection**

Cilj: dodatni prihod i jači lifecycle odnos s kupcem.

KONČAR treba zadržati domenski nalaz, odnos s kupcem i sanaciju; generički drone/ROV/robot hardware u početku partnerirati.

## 3. Preporučeni red rada

### Faza 1 — 0–90 dana: dokazati brzi učinak

#### 1. O001 — paketirati postojeći TMS servis
**Nositelj:** Institut + D&ST; Digital samo gdje je konkretno potreban.

Minimalni rezultat:
- jedan standardni opis paketa;
- što je uključeno / nije uključeno;
- način izvještavanja;
- godišnja cijena po uređaju ili floti;
- 3–5 postojećih kupaca kojima se može ponuditi proširenje.

Research planning envelope: O001 scenarij koristio je 50.000 EUR početne pripreme. To nije odobren budžet.

**Decision gate:** ne razvijati novu platformu ako se isti ishod može prodati kroz postojeći TMS i stručni workflow.

#### 2. O004 — audit jedne robotske ćelije / procesa
**Nositelj:** KMK ili KTK manufacturing + kvaliteta; vendor/integrator po potrebi.

Minimalni rezultat:
- jedna odabrana ćelija;
- 2–3 part familyja;
- ukupni takt prije/poslije;
- programiranje, pozicioniranje, čekanje kvalitete i dorade;
- vrijednost stvarno dodatno isporučivog outputa.

Research planning envelope: 120.000 EUR ciljane nadogradnje u srednjem scenariju.

**Decision gate:** ne investirati ako nema najmanje približno 700 neto oslobođenih sati/god. ili ekvivalentne stvarne uštede koja podržava željeni povrat u scenariju.

### Faza 2 — 3–9 mjeseci: pokrenuti dva razvojna proizvoda

#### 3. O005 — Tram/rail digital + safety
**Nositelj:** Electric Vehicles + Institute; Digital/NEOS za data/backend; FER kao mogući istraživački partner, ne Group owner.

Prvi proizvodni smjer:
1. fleet/maintenance intelligence;
2. tram ADAS / anti-collision / event recording;
3. autonomni depot tek uz konkretnog operatora.

Ne početi s punim driverless tramvajem za javne ulice.

Planning envelopes iz research scenarija:
- digital service adaptation ~100.000 EUR;
- series-specific ADAS adaptation/test ~300.000 EUR;
- autonomni depot je zaseban projekt kupca/operatora, ne mali feature.

**Decision gate:** vlastiti razvoj ima smisla samo ako funkcija može biti ponovljiva kroz više vozila/serija/kupaca, ne jedna demonstracija.

#### 4. O006 — Renewable/BESS portfolio intelligence
**Nositelj:** Digital + Renewable Energy Sources + aktualni vlasnik KONBAT/EMS capabilityja; NEOS za data/forecasting.

Prvi proizvod:
- multi-site performance/lost-production view;
- expert recommendations;
- BESS optimization only as incremental layer over existing EMS;
- market participation via partner where licenses/market access are needed.

Research planning envelope: 150.000 EUR početne productization/integration pripreme u scenariju.

**Decision gate:** ne razvijati universal AI dashboard; tražiti dovoljno velike lokacije/portfelje gdje 1–2% performance improvement ili BESS optimization stvara kupcu mjerljivu neto korist.

### Faza 3 — paralelno, samo uz narudžbu: O002/O003

#### O002 — Grid Inspection Care
**Nositelj:** Dalekovod + relevantni servis/engineering; Digital za evidence/history kada treba.

Model:
- mobilna inspekcija;
- standardni stručni nalaz;
- partner drone/robot;
- dock/BVLOS samo gdje je učestalost dovoljno visoka.

Research scenario: 30.000 EUR početne pripreme.

#### O003 — Hydro Inspection Care
**Nositelj:** Hydro Turbine / hydro service + specijalizirani ROV partner.

Model:
- partner podvodna operacija;
- KONČAR hidro-inženjerska interpretacija;
- bez vlastitog generičkog ROV razvoja u prvoj fazi.

Research scenario: 15.000 EUR početne pripreme.

## 4. Preporučeni organizacijski model

Ne osnivati šest novih timova.

### Product Council / portfolio owner
Jedna mala centralna koordinacija treba pratiti:
- business owner;
- product owner;
- technology owner;
- customer/channel;
- revenue or internal ROI;
- partner dependency;
- sigurnosne/data/IP granice.

### Domain product ownership

| Smjer | Business owner kandidat | Tehnički nositelji |
|---|---|---|
| O001 | Institut / D&ST | Institut + Digital gdje treba |
| O002 | Dalekovod | Dalekovod + Digital + partner |
| O003 | Hydro Turbine | Hydro + partner + Institute po potrebi |
| O004 | KMK/KTK operations | Manufacturing engineering + quality + integrator |
| O005 | Electric Vehicles | KEV + Institute + Digital/NEOS |
| O006 | Digital / Renewables | Digital + Renewables + KONBAT lineage + NEOS |

To su istraživački prijedlozi vlasništva, ne stvarne interne odluke.

## 5. Što zajednički graditi — a što ne

### Dijeliti kao platform primitives
- asset identity;
- time-series ingestion;
- alarm/event model;
- evidence/images;
- work-order link;
- identity/access/audit;
- reporting;
- model deployment/observability gdje je potreban.

### Ne centralizirati prerano
- rail safety control;
- transformer physics models;
- BESS control loops;
- welding robot control;
- ROV/drone navigation;
- domain-specific certification.

Pravilo: zajednički sloj graditi tek kada ga najmanje dva stvarna proizvoda trebaju u produkciji.

## 6. Resursna disciplina

Prema javnom researchu, vrijednost se najčešće gubi kada se:
- generički AI proglasi proizvodom;
- kupi robot prije jasnog procesa;
- scenarijska ušteda prikaže kao ostvareni profit;
- duplicira postojeći KONČAR ili vendor proizvod;
- partner hardver zamijeni za strateški IP;
- domain safety i business analytics spoje bez jasne granice.

Za svaku novu funkciju tražiti jedan od ova tri razloga:
1. kupac dodatno plaća;
2. tvornica stvarno isporučuje više;
3. lifecycle trošak ili rizik se dokazivo smanjuje.

Ako nema nijednog, razvoj ne ide dalje.

## 7. Portfolio milestoneovi

### M0 — Research complete
O001–O006 dovršeni iz javnih izvora. DONE.

### M1 — Commercial packaging
O001, O002, O003 imaju standardni scope/cjenovni okvir i named buyer segment.

### M2 — Internal productivity proof
O004 ima jednu stvarnu cell/process before-after metriku.

### M3 — Product MVP
O005 i O006 imaju svaka po jedan narrow production-grade use case, bez monolitne platforme.

### M4 — Repeatability
Najmanje dva različita kupca/asset seta koriste isti proizvodni core bez bespoke rekonstrukcije.

### M5 — Scale decision
Tek tada odlučiti:
- zasebna business line;
- veći software/AI tim;
- acquisition;
- vlastita robotics/autonomy platforma;
- 24/7 operations center.

## 8. Konačna preporuka

Ako KONČAR želi maksimalno smanjiti rizik i istodobno graditi buduće sposobnosti:

1. **monetizirati postojeći TMS servis (O001);**
2. **povećati proizvodni kapacitet kroz ciljanu automatizaciju (O004);**
3. **uložiti razvoj u tram/rail safety + fleet intelligence (O005);**
4. **uložiti razvoj u renewable/BESS intelligence (O006);**
5. **grid i hydro robotics koristiti kao servisne kanale uz partner hardver (O002/O003).**

To nije rang prinosa nego preporučeni portfolio red prema kombinaciji:
- postojećeg KONČAR capabilityja;
- vremenu do prve vrijednosti;
- potrebi za novim IP-em;
- partner ovisnosti;
- ponovljivosti;
- recurring/lifecycle potencijalu.

## 9. Što je sljedeći smisleni artefakt

Ako se ovaj portfolio stvarno želi pretvoriti u program, sljedeći artefakt treba biti **jedan-page investment/project brief za O005 i O006**, te **commercial packaging brief za O001**.

Ne treba ponovno otvarati široki research.
