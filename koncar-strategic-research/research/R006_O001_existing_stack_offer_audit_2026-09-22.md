---
research_id: R006
task_id: O001-A
title: O001 — provjera postojećeg sklopa i komercijalne ponude
as_of: 2026-09-22
status: complete-desk-review
internal_system_access: none
customer_interviews: none
commercial_validation: not-validated
---

# R006 — O001-A: postojeći TMS sklop, ponuda i granice teze

[Glavni indeks](../MASTER_INDEX.md) · [Task board](../validation/TASK_BOARD.md) · [Izvori i lokatori S01–S14](../sources/R006_evidence_register.md) · [O001](../opportunities/O001_transformer_intelligence_lifecycle_service.md)

## Odluka i rezultat

Treba provjeriti može li O001 stvoriti dodatnu naplativu vrijednost povrh postojećeg TMS-a i servisa. **Rezultat: REFRAME / nastaviti validaciju, ne investicijski GO.**

Raniji O001 već je prepoznao postojeći TMS i nije predlagao njegovu ponovnu izgradnju. Ovaj pregled potvrđuje taj baseline; novi doprinos je strože razdvajanje nepoznatih od dokazanih gapova, funkcijsko-teritorijalna provjera i sužavanje pretpostavki o povezivanju, prihodima i certifikaciji.

Fleet APM, stalni ekspertni servis i SLA nisu dokazano odsutni. Označeni su **U — nepoznato**, ne automatski G2. Konačni ishod može biti proširenje/prodaja postojeće ponude, mali tehnički dodatak ili odbacivanje nove poslovne teze.

O001-A završen je kao javna provjera. Stvarna interna arhitektura, ugovori, slobodni timski kapacitet i ekonomika nisu verificirani. Nije obavljen razgovor s kupcem, spajanje na sustav, SQL upit ili pilot.

## Metoda i granice dokaza

Otvorene su službene stranice Instituta, Digitala, D&ST-a, NEOS-a i dvije konkurentske ponude. Opći uvjeti F7220en-3 pregledani su u tekstu i na slikama obje PDF stranice. Točni izvori i ograničenja dohvaćanja su u evidence registru.

DOCUMENTED znači da proizvođač funkciju javno opisuje, ne da smo neovisno izmjerili performanse ili potvrdili svaku instalaciju. HISTORICAL ograničava referencu na njezino razdoblje. U znači nepoznato. Prijedlozi testova nisu tvrdnje o postojećoj implementaciji. Pregled nije iscrpan audit svih mogućih prodajnih i internih materijala.

## 1. Što se može ponovno potvrditi

**TMS [S01].** Opisana je modularna platforma za nove i postojeće transformatore različitih proizvođača, modeli stanja, povijest, alarmi, izvještaji i udaljeni pristup. KonFID koristi ARM/FPGA i proširive I/O module; naveden je tekst/Excel izvoz. To podupire nastavak na postojećem proizvodu. Brza lokalna akvizicija nije sama po sebi dokaz kontinuiranog streaminga u cloud.

**iPDCore [S02].** Dokumentirani su obrada parcijalnih izbijanja, ML grupiranje i klasifikacija PRPD uzoraka. To je specifična dijagnostička funkcija. Stranica ne daje stopu lažnih alarma po asset-mjesecu ni validaciju predviđanja svih vrsta kvarova i preostalog životnog vijeka.

**PROZA [S03].** Odvojena SCADA ponuda na HAT platformi podržava lokalni i Docker/cloud deployment. Objavljen je certifikacijski navod za IEC 62351 i opis procedura povezanih s IEC 62443. Nije pregledan odgovarajući certifikat s verzijom/opsegom; nije potvrđen TMS konektor, multi-tenancy ni end-to-end certifikacija nove ponude.

**Usluge i suradnici [S05, S07–S09, S14].** Institut razdvaja vlastite proizvode, R&D i dijagnostičko-ispitne usluge. D&ST ima postprodaju/teren, NEOS podatkovne i data-science kompetencije. To ne dokazuje konkretno zaduženje u O001, P&L vlasnika ili raspoloživ tim.

## 2. Podatkovni tok — javno poznato i otvorene granice

Ovo nije as-built dijagram kupca:

`mjerenja → KonFID/TMS/iPDCore → lokalna obrada, povijest i prikaz → objavljeni export/izvještaj/udaljeni pristup`

`TMS → [U: interface, ugovor i mrežna granica] → centralni fleet sustav → [U] → ekspertni servis/radni nalog`

| Granica | Javni dokaz | Što O001-B mora donijeti |
|---|---|---|
| Senzor → uređaj | Modularni I/O i IED integracija | Senzor, jedinica, kalibracija, preciznost, protokol i stvarna konfiguracija |
| Signal → feature/rezultat | Opis KonFID/PD obrade | Firmware, filtri, gain, sample rate, trigger, algoritam/model i verzija |
| Obrada → povijest | Pohrana/eventi/export | Schema, tipovi, quality, source/ingest timestamp, timezone, retention, backfill |
| Lokalno → fleet | Remote access nije API specifikacija | Transport/auth, payload/encoding, redoslijed, deduplikacija/retry, mrežne zone |
| Fleet → odluka/nalog | Nije provjereno | Asset ID, severity, ljudska potvrda, CMMS/EAM interface i zatvaranje |
| Više kupaca → ML skup | Nije provjereno | Prava agregiranja/treniranja, izolacija, retention, brisanje i izvedeni modeli |

Ne navoditi Kafka, REST, JSON, PostgreSQL ili određeni cloud kao aktualni stack bez dokaza. Kompetencija u Grupi nije konfiguracija ovog proizvoda. Izvoz može omogućiti read-only replay, ali ne dokazuje production streaming.

## 3. Funkcijsko-teritorijalna napomena koja utječe na izbor tržišta

Uz **DSync Demodulator Clusters** službena iPDCore stranica navodi da ta tehnologija nije dostupna u SAD-u, UK-u, Njemačkoj, Austriji, Švicarskoj, Italiji i Lihtenštajnu [S02].

Opravdani zaključak: prije ponude te konkretne funkcije potrebna je potvrda dopuštenog opsega po zemlji i verziji. Stranica ne objašnjava razlog, eventualni patent/licencu, rok ili trošak. Ne proširivati napomenu na cijeli TMS/iPDCore ili druge clustering metode. Tražiti funkcija × država × verzija × licenca matricu i odobrenu alternativu gdje je potrebna.

Ovo je prioritet za O001-B, ne pravno mišljenje niti zaključak da je cijeli izvozni proizvod zabranjen.

## 4. Komercijalni i installed-base baseline

Opći uvjeti [S04] vežu opseg i cijenu uz ponudu/ugovor, a posebne odredbe imaju prednost. Uređuju jamstvo, dokumentaciju i povjerljivost kupčevih informacija; standardno jamstvo ne pokriva određene štete/izgubljenu dobit zbog zastoja. Nisu stvarni kupčev SLA ni javni godišnji cjenik.

Poslovna implikacija: trebamo reprezentativan ugovor da razlikujemo isporuku uređaja, softversku licencu, servis i jamstvo raspoloživosti. Ne izvoditi pravo treniranja na telemetriji iz odredbe o tehničkoj dokumentaciji. Specifične ugovore mora provjeriti ovlaštena pravna funkcija.

Ras Laffan C je projekt iz **2009.–2010.**, s 12 step-up i četiri inter-bus transformatora [S06]. To potvrđuje povijesnu isporuku, ne aktivne pretplatnike u 2026. Monitoring portfolio navodi 60 država kroz više vrsta opreme [S10], ne TMS subscription inventory.

Raniji navod **780 sustava / 64 države / >60.000 MVA** nije ponovno potvrđen jer izvještaj iz B001 nije uspješno dohvaćen. Ne tvrdimo da su brojke netočne; ne koristimo ih kao ulaz u ARR model. I nakon potvrde povijesne brojke treba filtrirati na TMS, aktivan, kompatibilan, poveziv, pravno dostupan i komercijalno osvojiv uređaj. Broj isporuka nije broj pretplatnika.

Ukupan poslovni podatak Instituta [S13] nije TMS prihod, profit ili ARR. Za O001 trebaju segmentni ugovori, stavke prihoda/troška i sati isporuke, ne samo financijska veličina društva.

## 5. Konkurentski kontrolni test

Hitachi nudi manufacturer-agnostic TXpert usluge, remote procjenu i dugoročne pakete [S11]. Reinhausen javno prikazuje monitoring/service kombinacije i višegodišnje SLA modele [S12]. Nisu pribavljene usporedive komercijalne ponude.

Iz toga slijedi da remote monitoring, vendor-neutral integracija i SLA sami nisu jedinstvena diferencijacija. O001 treba dokazati bolji ukupni trošak, stručnu odluku, integraciju, servisni odziv ili pokrivenost za točno određenog kupca. Postojeći APM kupca dio je alternative, ne prazan prostor.

## 6. Matrica falsifikacije

| Testirana tvrdnja / kontrolni scenarij | Ishod | Posljedica |
|---|---|---|
| Izgraditi osnovni monitoring ponovno | Nema opravdanja: TMS je dokumentiran | Potvrđuje se raniji smjer nadogradnje, ne greenfield monitor |
| Povijest, izvještaji i remote access novi su opseg | Funkcije su već opisane | Ne predstavljati postojeće funkcije kao inovaciju |
| Fleet APM ne postoji | U | Demo i katalog isporučenih funkcija prije razvoja |
| 24/7 servis i ponavljajući ugovori ne postoje | U | Provjeriti ugovore, obnovu, service catalogue i staffing |
| PROZA certifikat automatski pokriva novi TMS sklop | Nepotkrijepljeno | Certifikat po komponenti, verziji i deploymentu |
| Sve iPDCore funkcije slobodno su dostupne svugdje | Za navedenu tehniku postoji teritorijalna napomena | Provjera dopuštenog opsega prije izbora tržišta |
| Povijesna installed base neposredno daje ARR | Nepotkrijepljeno | Aktivni uređaji, pristup, ugovor i spremnost platiti |
| Dobar tehnički fit znači profit | U | Kupac, inkrementalna ekonomika i izveden pilot |

## 7. Revidirana teza i najkraći sljedeći dokaz

**Provjeriti može li se profitabilno proširiti postojeća TMS/dijagnostičko-servisna ponuda za odabrani segment.** Mogući rezultat je veći attach/renewal ili bolji onboarding postojeće ponude, ne nužno nova platforma, organizacija ili razvoj AI-a.

[O001-B paket](../validation/O001_B_evidence_request.md) traži arhitekturu/verzije, reprezentativni podatkovni uzorak, prava, anonimiziranu ponudu/ugovor, aktivni inventory i isporučne troškove. Interni prilozi ne idu u public repo.

Prvi tehnički korak nakon dobivanja prava: read-only replay i usporedba s originalnim TMS prikazom. Mjeriti onboarding, ekspertno vrijeme i lažna upozorenja prije obećavanja cijene ili 24/7 centra. To nije dokaz spriječenih budućih kvarova.

Ishodi nakon B/C:

1. Ista ponuda već postoji: zaključiti da novi razvoj nije potreban; testirati skaliranje/prodaju/obnovu.
2. Kupac plaća mali nedostajući dodatak: razviti samo taj delta-opseg, uz postojeću platformu i odobrena prava.
3. Nema budžeta, prava ili pozitivne ekonomike: REJECT/HOLD.

Za sada je opravdano nastaviti dokazivanje, ne odobriti ulaganje. B002–B006 i njihove interne tvrdnje nisu ovim taskom revalidirane. R006 ima prednost pred starijim O001 gap pretpostavkama; ostale prilike imaju vlastite A taskove.
