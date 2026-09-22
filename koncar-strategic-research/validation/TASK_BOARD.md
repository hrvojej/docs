# Task board — validacija O001–O006

**Ažurirano:** 2026-09-22. **32 zadatka:** 1 COMPLETE_DESK, 6 READY, 6 WAITING_EVIDENCE, 19 DEPENDENT.

[MASTER_INDEX](../MASTER_INDEX.md) · [R005: metodologija i gateovi](../research/R005_validation_program_2026-09-22.md) · [R006: prvi rezultat](../research/R006_O001_existing_stack_offer_audit_2026-09-22.md)

Svaki red je zaseban task za zasebnu sesiju. A = javna provjera, B = interni dokaz, C = kupac/cijena, D = ekonomika, E = pilot i odluka. E ima odvojene izlaze DESIGN i RESULT; nije završen samo zato što postoji dizajn. Uloge su predloženi davatelji dokaza, ne dodijeljeni zaposlenici. READY za C znači da može krenuti javni dio, ne da su intervjui provedeni.

Konvencija budućih izlaza: `validation/results/<TASK_ID>.md`; za E još `<TASK_ID>_pilot_results.md`. To su planirane putanje, ne postojeće datoteke. Svaki izrađeni rezultat dobiva stvarnu poveznicu. O001-A je izrađen kao R006. U svakom rezultatu moraju biti izvori, potvrđeno/osporeo/nepoznato, odluka i sljedeći korak prema R005.

## O001 — Transformer intelligence i lifecycle usluga

| ID / status | Zadatak i potreban dokaz | Izlaz / kriterij zaustavljanja | Ovisnost |
|---|---|---|---|
| O001-A / COMPLETE_DESK | Ponovno provjeriti TMS, KonFID, iPDCore, PROZA, objavljene usluge i konkurentsko pakiranje; kontrolirati dupliciranje postojeće ponude | [R006](../research/R006_O001_existing_stack_offer_audit_2026-09-22.md). Potvrđen postojeći TMS; nepoznati APM/SLA gapovi vraćeni na U, dodatna usluga ostaje hipoteza | B001, O001 |
| O001-B / WAITING_EVIDENCE | Institut: aktualna arhitektura, API/export uzorci, licence, aktivni uređaji, postojeći APM/SLA, prodaja i troškovi; D&ST postprodaja; Digital gdje već sudjeluje | Dokazan deployment i ownership; [zahtjev](O001_B_evidence_request.md). STOP za novu platformu ako isti SKU već postoji; teritorijalna prava razriješiti prije izbora izvoznog paketa | A; ovlašten interni pristup |
| O001-C / READY | Vlasnici kritičnih transformatora: tenderi/ponude, kupci i odbijeni poslovi; odvojiti kupnju monitora od ekspertne usluge | Sadašnji trošak, budžet, incumbent, prihvatljiva cijena i odbijanja. Suziti/odbaciti ako nema dodatnog plaćenog ishoda | A; stvarni buyer dokazi za završetak |
| O001-D / DEPENDENT | Doprinos po uređaju/kupcu; aktivni i pravno dostupni uređaji; integracija, ekspertni sati, false alerts, podrška, teren | Break-even, downside i cash/payback; usporediti proširenje postojećeg s novim proizvodom. STOP ako realna cijena ne pokriva isporuku | B + C |
| O001-E / DEPENDENT | Read-only replay pa ograničena flota; usporedba s postojećim TMS alarmima i ekspertom; ugovoreni opseg, podaci, pragovi i sigurnost | DESIGN pa stvarni RESULT. Mali uzorak ne dokazuje spriječene katastrofalne kvarove; GO samo uz radni tok, mjerljivu vrijednost i kupčev prihvat | B + D |

## O002 — Grid inspection intelligence

| ID / status | Zadatak i potreban dokaz | Izlaz / kriterij zaustavljanja | Ovisnost |
|---|---|---|---|
| O002-A / READY | Revalidirati Dalekovodove usluge i benchmark slučajeve; razdvojiti manual drone, dock, ground robot i stvarnu BVLOS operaciju | Mapa tržišta po podkategoriji; pilot nije rollout, vendor ušteda nije KONČAR ROI | B002, O002 |
| O002-B / WAITING_EVIDENCE | Dalekovod-Projekt: flota, operateri, odobrenja, RGB/termalni/LiDAR formati, GIS, defect workflow, prava; Digital/servis: stvarne integracije | Tok snimka→asset→stručni nalaz→nalog; STOP za autonomiju bez sigurne/odobrive operacije ili prava pohrane | A + interni dokazi |
| O002-C / DEPENDENT | TSO/DSO: trošak po lokaciji/km/stupu, izlazaka, učestalost, ručni pregled, izvještaj, usporedive cijene | Dodatna vrijednost ponovljivosti/workflowa; zadržati manual capture ako dock/BVLOS ne donosi neto korist | A |
| O002-D / DEPENDENT | Manual/docked/fixed-sensor model; mobilizacija, vrijeme bez leta, dozvole, operator-to-fleet ratio, AI pregled i intervencije | Profit i prag iskorištenosti po tipu lokacije; STOP za CAPEX uz premalo misija ili preskupu ljudsku kontrolu | B + C |
| O002-E / DEPENDENT | Postojeće snimke i autorizirane rute; geolokacija nalaza, pokrivenost, vrijeme pregleda i valjanost naloga; tek zatim autonomija | DESIGN/RESULT s baselineom; odbaciti nedokazanu automatsku detekciju ili preusmjeriti na asistirani proces | B + D |

## O003 — Hydro underwater inspekcije

| ID / status | Zadatak i potreban dokaz | Izlaz / kriterij zaustavljanja | Ovisnost |
|---|---|---|---|
| O003-A / READY | Revalidirati ROV reference i neuspjele misije; odvojiti kratku vizualnu inspekciju, sonar, mjerni 3D i penstock NDT | Zrelost po zadatku, ne jedan status za sve ROV primjene | B003, O003 |
| O003-B / WAITING_EVIDENCE | Hydro/GIM: podizvođači, godišnji poslovi, geometrije, tlak/protok/vidljivost, izolacije, operatori, recovery plan, izvještaji i prava | Potvrđena misijska ovojnica i stručni potpis; STOP bez sigurnog pristupa ili potrebne dijagnostičke kvalitete | A + interni dokazi |
| O003-C / DEPENDENT | Kupci/partneri: diver/ROV/dewatering alternative, stvarni zastoj i gubitak proizvodnje, periodicitet, cijena stručnog izvještaja | Razdvojiti naplativi pregled i hipotetski remont; STOP ako video bez kvantitativnog mjerenja ne rješava problem | A |
| O003-D / DEPENDENT | Najam/podizvođač/kupnja; operatori, put, sezonalnost, neuspjele misije i rizik gubitka opreme | Prag broja poslova i doprinos; preferirati najam ako kupnja nema opravdanu iskorištenost | B + C |
| O003-E / DEPENDENT | Dostupna niskorizična inspekcija s referentnim nalazom; ne dugi tlačni cjevovod kao prvi test | DESIGN/RESULT: pokrivenost, lokacija/mjerljivost defekta, izbjegnuti stvarni trošak i stručni prihvat; STOP za neprihvatljiv retrieval rizik | B + D |

## O004 — Interna adaptivna proizvodnja i kvaliteta

| ID / status | Zadatak i potreban dokaz | Izlaz / kriterij zaustavljanja | Ovisnost |
|---|---|---|---|
| O004-A / READY | Revalidirati KMK/CLOOS i vanjske high-mix slučajeve; razlikovati arc-on brzinu, takt, smjenu i cijelu tvornicu | Usporediv dokaz po obitelji dijelova; ne prenositi 3× brzinu sklopa na 3× tvorničkog kapaciteta | B004, O004 |
| O004-B / WAITING_EVIDENCE | KMK/KTK: weld-hour Pareto, OEE, programiranje, fixture/crane vrijeme, ERP/MES/CAD/PLM, NDT, dorade, kvalifikacije i JV prava | Stvarni bottleneck i tok CAD→weld→NDT→prihvat; STOP za novi robot ako zavarivanje nije ograničenje ili postojeća ćelija nije iskorištena | A + proizvodni podaci |
| O004-C / DEPENDENT | Interni kupac: pogon, kvaliteta i prodaja; backlog, stvarna potražnja, partner ponude i prihvat promjene procesa | Dokaz da dodatni izlaz može biti prodan/isporučen ili stvarna ušteda dorade; ne zamišljeni ARR | A + pogon/prodaja |
| O004-D / DEPENDENT | Offline programiranje, senzori, integracija, ćelija, NDT, održavanje; doprinos dodatne količine i trošak zastoja | ROI/NPV s odobrenom stopom i bez dvostrukog brojanja sati; STOP ako dorade/odobrenja ponište korist | B + C |
| O004-E / DEPENDENT | Kontrolirana usporedba 2–3 obitelji, s kvalifikacijom procesa i potpisom kvalitete | DESIGN/RESULT: ukupni takt, first-pass yield, NDT i dorade, ne samo brzina luka. GO samo za validirane obitelji | B + D |

## O005 — Rail fleet/battery/charging

| ID / status | Zadatak i potreban dokaz | Izlaz / kriterij zaustavljanja | Ovisnost |
|---|---|---|---|
| O005-A / READY | Potvrditi status centralne platforme: razvoj, pilot, ugovor ili produkcija; revalidirati benchmark vremenske scopeove | Postojeće funkcije i ograničenja; MERMEC i vozilo nisu isti IP | B005, O005 |
| O005-B / WAITING_EVIDENCE | KEV/Digital: TCMS/BMS/punionice, signalni katalog, timestep, SOC/SOH definicije, firmware, licence, servis i sigurnosna granica | Read-only tok train→charger→platform→maintenance; STOP za model bez potrebnih BMS signala/licenci | A + interni dokazi |
| O005-C / DEPENDENT | Operator/leasing: kašnjenja, raspoloživost, servisni trošak, baterijsko jamstvo, tarife i nedostatna napunjenost | Plaćeni dodatak povrh maintenance ugovora; odvojiti SOC prikaz od naplative optimizacije | A |
| O005-D / DEPENDENT | Cijena po vozilu/punionici, integracija, baterijsko trošenje, energija, SLA i vozni red | Simple-rule baseline protiv optimizacije; STOP ako trošenje/operativni rizik nadmašuju uštedu | B + C |
| O005-E / DEPENDENT | Replay i shadow-mode na odobrenim podacima; nema neodobrenog upravljanja vlakom | DESIGN/RESULT: spremnost vozila, energija, peak, izvedivost voznog reda i battery-health validacija | B + D |

## O006 — Renewable/BESS portfolio

| ID / status | Zadatak i potreban dokaz | Izlaz / kriterij zaustavljanja | Ovisnost |
|---|---|---|---|
| O006-A / READY | Potvrditi KONBAT, EMS, Vis/Pometeno i kontrolni centar; odvojiti lokalni kontroler, portfolio APM i merchant bidding | Proizvod/verzija/status; kontrolni centar nije automatski portfolio optimizer | B006, O006 |
| O006-B / WAITING_EVIDENCE | Aktualni KONBAT vlasnik; SCADA/historian/BMS/PCS/CMS, maintenance, licence, podaci i sigurnosne granice | Stvarna arhitektura i prava po lokaciji; STOP za pooling bez dopuštenja OEM-a/operatora | A + interni dokazi |
| O006-C / DEPENDENT | IPP/utility: lost production, curtailment, balancing, servis, APM cijene, lokalna tržišna ograničenja | Problem/cijena po tehnologiji i zemlji; zasebna provjera prije market bidding ponude | A |
| O006-D / DEPENDENT | Integracija/platforma/pregledi/baterijsko trošenje; dispatch backtest bez budućih informacija | Neto vrijednost nasuprot jednostavnom EMS-u; STOP ako uplift nestaje nakon trošenja, naknada i ograničenja | B + C |
| O006-E / DEPENDENT | Ovlašteni povijesni podaci pa shadow-mode na lokaciji; prognoza, nalozi i dispatch | DESIGN/RESULT: neto vrijednost i pouzdanost uz iste granice; bez autonomnog upravljanja prije odobrenja | B + D |

## Zajednički zaključni zadaci

| ID / status | Zadatak i potreban dokaz | Izlaz / kriterij zaustavljanja | Ovisnost |
|---|---|---|---|
| X01 / DEPENDENT | Stvarne B arhitekture, dijeljeni podatkovni ugovori, timovi, ulaganja, kanali i kanibalizacija | Minimalni zajednički interface/platform opseg; ne graditi monolit bez dva dokazana consumer-proizvoda i vlasnika | Najmanje dva relevantna B |
| X02 / DEPENDENT | Investicijski memorandum za šest prilika i opciju ne ulagati; odvojiti interne uštede od vanjskog rasta | GO/REFRAME/HOLD/REJECT s dokazima, budžetom, rizicima i odgovornim donositeljem. Manjak dokaza nije GO | E-result ili obrazložena ranija eliminacija; X01 gdje relevantan |

## Nastavak u novom chatu

Učitati CURRENT_CONTEXT, R005, ovaj board i relevantni O###. Za O001 dodatno R006 i O001_B_evidence_request. Navesti TASK_ID. Sačuvati rezultat, izvore, ažurirati red i O###, master i sesiju. Ne zaključivati iz memorije ako postoje noviji podaci u repozitoriju.
