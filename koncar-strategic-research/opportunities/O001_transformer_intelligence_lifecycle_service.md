---
opportunity_id: O001
title: KONČAR Transformer Intelligence & Lifecycle Service
status: reframed-awaiting-internal-evidence
as_of: 2026-09-22
benchmark: B001
latest_validation: R006
public_capability: documented
integrated_architecture: unverified
commercial_validation: not-yet-E5
---

# O001 — Transformer Intelligence & Lifecycle Service

[Master](../MASTER_INDEX.md) · [B001](../benchmarks/B001_transformer_asset_intelligence_2026-09-21.md) · [R006: aktualna provjera](../research/R006_O001_existing_stack_offer_audit_2026-09-22.md) · [Task board](../validation/TASK_BOARD.md)

## Aktualna teza

Provjeriti postoji li profitabilan dodatak ili mogućnost skaliranja **postojeće** TMS/dijagnostičko-servisne ponude. Ranija teza već je polazila od postojećeg TMS-a; nova provjera pooštrava što je dokazani nedostatak, a što samo nepoznato.

Konačni proizvod može biti proširenje postojeće usluge, veći attach/renewal ili manji integracijski dodatak. Ne pretpostavljati potrebu za novom platformom, poduzećem ili akvizicijom.

## Što se zna, uz granicu dokaza

TMS/KonFID i iPDCore dokumentirani su proizvodi s lokalnom obradom i dijagnostikom. PROZA i NEOS predstavljaju moguće susjedne kompetencije, ne dokaz već izvedenog end-to-end sklopa. Detaljni primarni izvori, hardverski opis, prava i temporalne napomene nalaze se u R006 i njegovu evidence registru.

Ranija oznaka E4 značila je desktop procjenu tehničke povezanosti, ne potvrdu internog tima, slobodnog kapaciteta, integrirane arhitekture ili profita. Komercijalni E5 nije dostignut.

## Nepoznato nije potvrđeni gap

| Tema | Aktualni status | Što treba dokazati |
|---|---|---|
| Fleet APM / zajednički portal | U | Aktualni demo, funkcije/SKU, kupci i deploymenti |
| Stalni ekspertni monitoring / 24/7 / SLA | U | Stvarni service catalogue, ugovori, staffing i cijena |
| TMS → centralni sustav / CMMS | U | API/schema, poruke, konfiguracije i reference |
| Data/ML prava između kupaca | U | Ugovorni opseg i odobrena uporaba |
| iPDCore dostupnost po tržištu | Dokumentirana napomena za određenu tehniku | Funkcijsko-teritorijalna matrica; nije blanket zabrana proizvoda |
| Ponavljajući prihod / doprinos | U | Aktivni ugovori i izravni troškovi |
| End-to-end product/P&L owner | U | Potvrđena interna odgovornost; nije dokazano da vlasnik ne postoji |

## Mogući plaćeni ishodi — hipoteze

Manje ekspertnih sati po vjerodostojnom nalazu; brži prijelaz iz alarma u održavanje; manje nepotrebnog terena; kvalitetnije određivanje prioriteta flote; lakši onboarding postojećih monitora. Kupac treba potvrditi dodatnu vrijednost nasuprot svojem postojećem APM-u i servisu. Ne koristiti generički remote monitoring/SLA kao navodno jedinstvenu prednost.

Potencijalni segmenti za O001-C: kritični transformatori utility/industrijskih/obnovljivih portfelja. To nije konačan izbor kupaca. Ne množiti sve D&ST godišnje isporuke cijenom high-end monitoring usluge.

## Mogući doprinosi Grupe — nisu imenovanja

Institut je početni sugovornik za TMS, dijagnostiku i vlastite usluge; D&ST za OEM/postprodajni kanal. Digital/NEOS uključiti nakon provjere stvarne integracije i potreba. HELB/ostali terenski timovi samo uz potvrđen isporučni model. KPT podatke/IP ne pretpostavljati dostupnima bez provjere prava i governancea.

## Kako tezu oboriti

- Isti opseg već postoji i nema nezadovoljene potrebe: odbaciti novi proizvod; razmotriti komercijalno skaliranje postojećeg.
- Kupac ne plaća dodatni ishod ili integracija košta više od koristi: odbaciti/suziti segment.
- Prava onemogućuju odabranu funkciju, podatke ili tržište: promijeniti konfiguraciju/segment ili HOLD.
- Ekspertno vrijeme, lažni alarmi i SLA trošak ponište maržu: ne uvoditi obećani paket.
- Pilot ne nadmaši postojeći TMS/stručni workflow: nema opravdanja za razvoj samo radi AI-a.

## Taskovi i odluke

| Task | Status / izlaz |
|---|---|
| O001-A | COMPLETE_DESK — R006; baseline potvrđen i teza sužena |
| O001-B | WAITING_EVIDENCE — [šest internih dokaznih cjelina](../validation/O001_B_evidence_request.md) |
| O001-C | READY za javni komercijalni pregled; stvarni buyer dokaz još nedostaje |
| O001-D | DEPENDENT — inkrementalna ekonomika nakon B/C |
| O001-E | DEPENDENT — dizajn pa izveden pilot/odluka |

R006 ne potvrđuje ranije povijesne installed-base brojke za financijski model. Nijedan intervju ili pilot nije proveden. U ovoj fazi nema odobrenja razvoja, akvizicije, zapošljavanja 24/7 centra ili investicijske preporuke.

## Evidencija promjene

2026-09-22: APM/SLA/integracijski nedostaci promijenjeni iz pretpostavljenih build gapova u U; dodana funkcijsko-teritorijalna provjera, razdvojene certifikacije i aktivna installed base od povijesnih isporuka. Stara razrada ostaje u Git povijesti; R006 je aktualni dokazni baseline.
