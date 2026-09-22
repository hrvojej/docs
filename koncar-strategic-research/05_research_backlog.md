# Research backlog — aktualna faza

**Ažurirano:** 2026-09-22. [MASTER_INDEX](MASTER_INDEX.md) · [TASK_BOARD](validation/TASK_BOARD.md)

## Izvršavanje: jedan izvor istine

Detaljni statusi svih 32 validacijskih zadataka vode se u TASK_BOARD-u, ne u paralelnim checkbox listama. [R005](research/R005_validation_program_2026-09-22.md) određuje metode, ulaze, izlaze i kriterije odluke.

Prvi zadatak O001-A je završen kao javna provjera kroz [R006](research/R006_O001_existing_stack_offer_audit_2026-09-22.md). Preostaje 31 task. O001-B čeka ovlaštene interne dokaze; O001-C i ostali A taskovi mogu nastaviti javni dio.

## Preostali rad po cjelinama

| Cjelina | Što je napravljeno | Što ostaje |
|---|---|---|
| Struktura Grupe | R001 prvi perimeter | Pravna usklađenja indirektnih entiteta, promjena i ownershipa; ne proglašavati ga iscrpnim registry auditom |
| Kompetencije | R002–R003, E001–E019 | Aktualni timovi, IP, proizvodi, reference, slobodni kapacitet, data rights i financijski segmenti |
| Vanjski benchmark | B001–B006 i R004 prva sinteza | Revalidirati presudne tvrdnje u A taskovima; razlikovati vendor izjavu od nezavisnog dokaza |
| As-is arhitekture/ponuda | O001-A javni baseline | Svih šest B taskova: stvarne verzije, tokovi, serializacija, ugovori i isporuka |
| Kupci/cijene | Definiran okvir | Svih šest C taskova; O004 ima internog ekonomskog kupca |
| Ekonomika | Definirane formule i testovi | Svih šest D taskova; stvarni ulazi ili eksplicitni break-even scenariji, bez lažne bazne profitabilnosti |
| Piloti | Definirani tipovi dokaza | Svih šest E taskova: DESIGN pa stvarni RESULT; ne poistovjećivati plan i izvršenje |
| Zajednička platforma | Hipoteza iz R004 | X01 tek nakon stvarnih B arhitektura, minimalni dijeljeni opseg |
| Investicijski zaključak | Nije donesen | X02: GO/REFRAME/HOLD/REJECT uključujući opciju ne ulagati |

## Neposredni red rada

1. O001-B: pribaviti [minimalni paket internih dokaza](validation/O001_B_evidence_request.md) u privatnom prostoru.
2. O001-C: javni komercijalni pregled kao idući izvršivi desk task; aktualne ponude/tenderi i buyer segmentacija, bez izmišljanja intervjua.
3. O002-A–O006-A neovisno nastaviti revalidacije.
4. B/C → D → E po prilici; X01 i X02 po ovisnostima iz boarda.

Nisu zakazana automatska izvršavanja. Svaki task može se pokrenuti u zasebnoj sesiji pozivanjem njegovog ID-a. Trenutačno nijedna teza nije dobila E5 ni budžet za razvoj.
