# R006 — registar provjerenih izvora

**Datum provjere:** 2026-09-22. **Opseg:** O001-A. [R006](../research/R006_O001_existing_stack_offer_audit_2026-09-22.md) · [Master](../MASTER_INDEX.md)

Status READ označava pregledan sadržaj, ne neovisnu potvrdu svih proizvođačevih tvrdnji. Nedatirana stranica nije dokaz kada je određena funkcija uvedena. Ne kopiramo cijele web-stranice ni zaštićene PDF-ove u javni repo.

| ID | Primarni izvor i status | Lokator / što podupire / ograničenje |
|---|---|---|
| S01 | [Institut: Transformer monitoring system](https://www.koncar-institut.hr/en/transformer-monitoring-system) — READ | Benefits, System architecture, Overvoltage measurement. Funkcije i KonFID; nije as-built kupca niti API specifikacija. |
| S02 | [Institut: iPDCore](https://www.koncar-institut.hr/en/partial-discharge-measurement-and-monitoring-system-ipd-core) — READ | DSync Demodulator Clusters, pripadajuća teritorijalna napomena, Automatic noise suppression and source separation. Specifični ML i ograničenje jedne tehnike; razlog ograničenja nije objavljen. |
| S03 | [Digital: PROZA Station](https://www.koncar.hr/en/digital/digital-soulutions-and-platforms/proza-station) — READ | Cloud deployment; Certified cybersecurity. Lokalno/cloud i opis certifikacije; ne prenosi se na TMS i novi end-to-end proizvod. |
| S04 | [Institut: General Terms and Conditions of Sales, F7220en-3](https://www.koncar-institut.hr/sites/default/files/dokumenti/2025-04/F7220en-3.pdf) — READ + VISUAL | PDF stranice 1–2. Točke 1.4, 3–5, 10, 12.1, 12.3: posebni ugovor, ponuda/cijena, jamstvo, dokumentacija i povjerljivost. Pregledane slike obiju stranica. Nije aktualni kupčev ugovor niti pravno mišljenje. |
| S05 | [Institut: Operations overview](https://www.koncar-institut.hr/en/operations-overview) — READ | Tri djelatnosti i link na uvjete prodaje. Razlikovati proizvod, R&D i dijagnostičke usluge. |
| S06 | [Institut: Ras Laffan C](https://koncar-institut.hr/en/projekt/termoenergetski-projekt-samostalni-vodoenergetski-projekt-ras-laffan-c) — READ / HISTORICAL | Projektni opis i datum 2009.–2010. Isporuka TMS-a, ne potvrda aktivnog servisa u 2026. |
| S07 | [D&ST: društvo, proizvodi i servis](https://www.koncar.hr/en/koncar-distribution-and-special-transformers) — READ | Proizvodni raspon, terenske usluge, SET/DT service and post sales. Ne dokazuje monitoring attach rate ni partnerstvo u O001. |
| S08 | [NEOS: Data Science](https://www.neos.hr/expertise/data-science/) — READ | Data Science odjeljak. Deklarirana kompetencija, ne dokaz isporučenog TMS ML produkta. |
| S09 | [NEOS: Data Engineering](https://www.neos.hr/expertise/data-engineering/) — READ | Data Engineering odjeljak. Adjacent capability; konkretan TMS stack nije potvrđen. |
| S10 | [Institut: Monitoring](https://www.koncar-institut.hr/en/monitoring) — READ | Portfolio i navod 60 zemalja, više kategorija imovine. Ne koristiti kao TMS pretplatničku populaciju. |
| S11 | [Hitachi Energy: TXpert Services](https://www.hitachienergy.com/products-and-solutions/transformers/the-txpert-ecosystem/txpert-services) — READ | Glavni opis remote diagnostics, manufacturer-agnostic ecosystem, packaged/long-term agreements. Dokaz ponude; ne cijene ni dobit klijenta. |
| S12 | [Reinhausen: Performance Contracts and Consulting Transformers](https://www.reinhausen.com/servicedetail/transformer-services/performance-contracts-and-consulting-transformers) — READ | 3–5-year strategy, monitoring/service/AMG/TaaS odjeljci. Dokaz različitih paketa/odgovornosti; nije usporediva ponuda za konkretan KONČAR pilot. |
| S13 | [Institut: About us](https://www.koncar-institut.hr/en/about-us-0) — READ AFTER NAVIGATION | Objavljeni aggregate poslovni podatak za 2025. Ne poistovjećivati s profitom, TMS prometom ili ARR-om. Izravan dohvat jednom je vratio 404; link s naslovnice potom je vratio sadržaj. |
| S14 | [Institut: Research and Development](https://www.koncar-institut.hr/en/research-and-development) — READ | Advanced transformer research: domenska istraživanja/analize. Ne dokazuje raspoloživ tim za novu obvezu. |

## Nedohvaćeni izvori i posljedice

| ID | Izvor | Ishod |
|---|---|---|
| U01 | [Sustainability report 2023 iz B001](https://www.koncar-institut.hr/sites/default/files/dokumenti/2024-10/KEEI-Sustainability-report-2023.pdf) | Web dohvat nije uspio (DisabledError/timeout). Ranije brojke 780/64/>60.000 MVA nisu ponovno potvrđene; isključene iz nove ekonomike. Ne tvrditi da su pogrešne. |
| U02 | [KONČAR Product Catalogue iz B001](https://www.koncar.hr/sites/default/files/dokumenti/mediji/2025-03/KON%C4%8CAR%20-%20Product%20Catalogue_0.pdf) | Ponavljani timeout. Tvrdnja o fleet-wide prognostics ostaje za provjeru na katalogu ili demonstraciji. |

## Audit istraživanja

Otvorene su i službene pregledne stranice Digitala i njegova Energy područja; nisu dovoljan izvor za negativnu tvrdnju 'APM ne postoji'. Pokušaji široke web-pretrage vratili su nerelevantne rezultate pa su isključeni. Lokalni pokušaj arhiviranja javnih dokumenata nije uspio zbog DNS ograničenja; nije nastala potvrđena lokalna kopija tih PDF-ova. Web sadržaj i GitHub pohrana korišteni su kroz raspoložive alate.

R006 nije cjelovit IP/certifikacijski audit niti benchmark svih suparnika. Presudni public nalazi služe da se postave falsifikacijski testovi i ciljani interni zahtjevi.
