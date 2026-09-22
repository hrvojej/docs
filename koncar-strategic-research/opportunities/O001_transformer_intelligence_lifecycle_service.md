---
opportunity_id: O001
title: Monitoring transformatora kao stručna pretplatnička usluga
as_of: 2026-09-22
status: completed-public-research
recommendation: expand-existing-offer-not-new-platform
basis: public-primary-sources-and-explicit-scenarios
actual_profit_verified: false
---

# O001 — Završna procjena: monitoring transformatora kao usluga

[Glavni indeks](../MASTER_INDEX.md) · [Šest zadataka](../validation/TASK_BOARD.md) · [Raniji benchmark B001](../benchmarks/B001_transformer_asset_intelligence_2026-09-21.md)

## 1. Zaključak

**Preporuka: DA ograničenom komercijalnom proširenju postojećeg TMS-a i dijagnostičkog servisa; NE novoj velikoj AI platformi, novom hardveru ili akviziciji za ovu priliku.**

KONČAR ima dokumentiranu tehničku osnovu, a vanjski dobavljači pokazuju da se monitoring i stručna interpretacija prodaju zajedno. Smislen početni proizvod je godišnja usluga za kritične transformatore koji već imaju monitoring: pregled trendova, stručna obrada upozorenja, periodični izvještaj i preporuka održavanja. [S01–S06]

Procjena je da to može biti profitabilno proširenje postojeće djelatnosti. Javni izvori ne dokazuju da KONČAR upravo taj paket još nema niti objavljuju njegovu stvarnu maržu. Zato preporuka vrijedi i ako je proizvod već razvijen: **prodati i standardizirati postojeće, a razvijati samo nužni dodatak.**

Ovaj istraživački zadatak je dovršen. Nema čekanja na korisnikove dokumente, interne intervjue ili dodatne research podzadatke. Poslovni scenariji ispod nisu ostvareni rezultati, a opis probne isporuke nije tvrdnja da je pilot izveden.

## 2. Što ponuditi i kome

**Radni naziv: KONČAR Transformer Care.** To je predloženi naziv paketa, ne potvrđeni postojeći KONČAR brand.

Početni paket:
- objedinjeni pregled stanja odabranih transformatora na postojećim podacima;
- stručna obrada važnih promjena i alarma tijekom ugovorenog radnog vremena;
- tromjesečni izvještaj s prioritetima i preporukom daljnjih mjerenja ili održavanja;
- evidencija preporuke, odgovora kupca i ishoda intervencije.

Kontinuirano prikupljanje podataka nije isto što i neograničena dostupnost stručnjaka 24/7. Prvi paket ne uključuje osiguranje od kvara, jamstvo raspoloživosti ni daljinsko upravljanje transformatorom. Terenska mjerenja, dodatni ekspertni sati, hardver i instalacija naplaćuju se zasebno.

**Prvi ciljani segment, kao moja preporuka:** postojeći korisnici TMS-a i kupci kritičnih srednjih/energetskih transformatora koji nemaju dovoljno vlastitog dijagnostičkog kapaciteta. Posebno su zanimljivi industrijski pogoni i vlasnici obnovljivih portfelja. Ne ciljati automatski svaku malu distribucijsku jedinicu: godišnja stručna usluga mora biti razmjerna vrijednosti odluke i posljedici zastoja.

Korisnik usluge bio bi voditelj održavanja ili upravljanja imovinom; poslovni razlog kupnje je manje nepotrebnih odlazaka i ispitivanja te bolja odluka što popravljati i kada. To je predložena segmentacija, ne popis kupaca koji su obećali naručiti.

## 3. Dokaz da tržište postoji — i što on ne dokazuje

| Javni primjer | Što je dokumentirano | Poslovna pouka |
|---|---|---|
| Hitachi TXpert Services | Udaljena dijagnostika, proizvođački neovisan sustav i mogućnost dugoročnih servisnih paketa [S04] | Kupac može kupovati stručnu uslugu, ne samo senzor |
| Reinhausen | Odvojeni monitoring i servisni ugovori te njihova kombinacija; navodi strategije od 3–5 godina [S05] | Ponudu treba jasno ograničiti i odvojiti od skupljih garancija |
| Neoen / Camlin, objava 9. 6. 2026. | Nakon višeregionalnog pilota ugovoren je globalni program s centralnom analitikom i ekspertnim centrom [S06] | Postoji potražnja vlasnika obnovljivih portfelja; objava nije dokaz da je cijela flota već opremljena |
| KAMO / Vaisala, objava 3. 7. 2025. | U konkretnom slučaju praćenja 84 MVA transformatora smanjeno je uzorkovanje i izbjegnuta daljnja ispitivanja; kupac procjenjuje uštede u desecima tisuća USD [S07] | Naplativa vrijednost može biti bolja dijagnostička odluka, ne samo spriječen katastrofalan kvar |
| Tata Steel / Hitachi | Opisan je početni plan za pet kritičnih transformatora i potreba za preventivnim održavanjem [S08] | Industrijski pogon je relevantan tip kupca; plan implementacije nije izmjeren rezultat |

Ovo su izvori proizvođača/dobavljača, ponegdje s izjavom kupca. Dokazuju ponudu, ugovore ili opisane slučajeve; nisu neovisni audit ušteda niti dokaz spremnosti hrvatskog kupca da plati određenu cijenu. Starije opće postotke smanjenja kvarova iz promidžbenih materijala nisam prenio u financijski model.

**Konkurencija je ozbiljna.** Proizvođačka neovisnost, dashboard i AI već postoje drugdje. KONČAR-ova moguća prednost je postojeća oprema i servisni odnos, stručna dijagnostika te manji trošak uključivanja korisnika vlastitog TMS-a — ne tehnološka jedinstvenost koja bi bila unaprijed dokazana.

## 4. Što KONČAR već ima i što bi stvarno trebalo dodati

TMS je dokumentiran za nove i postojeće transformatore različitih proizvođača, s modelima stanja, alarmima, pohranom, izvještajima i udaljenim pristupom. Objavljena arhitektura koristi KonFID; naveden je izvoz u tekst i Excel. To je dovoljna javna osnova za preporuku nadogradnje postojećeg proizvoda, ali nije specifikacija konkretnog korisničkog sustava. [S01]

Institut zasebno navodi vlastita rješenja i dijagnostičko-ispitne usluge. D&ST ima proizvodni, terenski i postprodajni kanal. [S02–S03]

Digitalova PROZA podržava lokalno i cloud postavljanje; NEOS opisuje podatkovnu integraciju i obradu događaja. Te kompetencije mogu pomoći, ali njihov zajednički TMS proizvod i potrebna integracija nisu dokazani ovim izvorima. [S09–S10]

| Sastavnica | Odluka za početak |
|---|---|
| Mjerenje, lokalni alarmi i postojeća dijagnostika | Ponovno koristiti TMS, ne razvijati zamjenu |
| Stručna interpretacija | Predloženi nositelj Institut; nije potvrda slobodnih internih kapaciteta |
| Prodaja i terenske intervencije | Početi postojećim servisnim kanalima, bez obveznog angažiranja cijele Grupe |
| Pregled više uređaja i evidencija preporuka | Upotrijebiti postojeću funkciju ako postoji; inače napraviti mali integracijski dodatak |
| Napredni AI | Dodavati samo za mjerljivo smanjenje ručnog rada ili bolju dijagnostiku |
| Nova platforma, 24/7 centar i vlastiti dodatni senzori | Ne preporučujem ih kao početno ulaganje |

Ne tvrdim da centralni pregled ili SLA interno nedostaju. Njihov javno nepoznat opseg ne smije postati razlog za dupliciranje razvoja.

**Predloženi jednostavan tok, ne snimka postojeće arhitekture:** TMS → odobreni izvoz/veza → evidencija stanja uređaja → stručni nalaz → preporuka kupcu → zasebno ugovorena intervencija. Za početak ne treba nova kontrolna petlja niti centralno slanje svih brzih sirovih valnih oblika.

## 5. Poslovni model i realna granica zaključivanja o profitu

U pregledanim službenim ponudama nisam našao usporediv javni godišnji cjenik ovog kompletnog paketa. Šira pretraga cijena i tendera nije dala dovoljno pouzdan usporediv iznos. **Niže navedeni iznosi su moje scenarijske pretpostavke, a ne tržišni cjenik, ponuda dobavljača ili financije KONČAR-a.**

Model računa samo novi godišnji servis na već opremljenim i dostupnim transformatorima. Ne pribraja maržu od prodaje opreme, remonta ili ugradnje. To sprječava da se pretpostavljeni budući remont upotrijebi za uljepšavanje isplativosti usluge.

### Pretpostavke modela

| Ulaz | Pretpostavka i značenje |
|---|---|
| Godišnja naknada | 3.000 EUR po uređaju; cijena za scenarij, ne potvrđena spremnost kupca |
| Ekspertni rad | Prosječno 12 sati godišnje po uređaju × 75 EUR ukupnog/opportunitetnog troška sata = 900 EUR |
| Podaci i hosting | 150 EUR po uređaju godišnje |
| Korisnička podrška i izvještajni rad | 250 EUR po uređaju godišnje, odvojeno od stručne dijagnostike |
| Varijabilna rezerva | 200 EUR po uređaju godišnje za manje dodatne troškove isporuke/prodaje |
| Ukupni varijabilni trošak | 1.500 EUR po uređaju godišnje |
| Godišnji fiksni trošak programa | 75.000 EUR: pretpostavljeno 30.000 održavanje/inženjerska podrška proizvoda, 20.000 koordinacija/prodaja, 15.000 sigurnost/kvaliteta i 10.000 zajednički sustavi |
| Jednokratna priprema | 50.000 EUR za ograničeno pakiranje/integraciju; scenarij i predložena početna granica, ne izvođačka procjena |

I postojeći zaposlenici imaju trošak; ne računam njihov rad kao besplatan. Dvanaest sati je proračunski prosjek, ne dokazana operativna potreba. Složen uređaj ili intenzivna obrada mora imati drugačiji paket ili dodatno plaćene sate.

### Rezultat pri punoj godini naplate

| Plaćeni uređaji tijekom cijele godine | Godišnji prihod | Varijabilni trošak | Fiksni trošak | Doprinos nakon programskih troškova | Nakon jednokratnih 50.000 EUR u prvoj godini |
|---:|---:|---:|---:|---:|---:|
| 30 | 90.000 | 45.000 | 75.000 | −30.000 | −80.000 |
| 50 | 150.000 | 75.000 | 75.000 | 0 | −50.000 |
| 100 | 300.000 | 150.000 | 75.000 | 75.000 | 25.000 |
| 200 | 600.000 | 300.000 | 75.000 | 225.000 | 175.000 |

Sve brojke u EUR. Formula: `doprinos = N × (cijena − varijabilni trošak) − fiksni trošak`.

Točka operativnog pokrića je **50 uređaja**. Uz uključen početni izdatak, za nenegativan iznos u prvoj punoj godini treba najmanje **84 uređaja**. Broj kupaca/uređaja ovdje je test veličine poslovanja, ne prognoza prodaje ni tvrdnja o aktivnoj TMS bazi. Dolasci tijekom godine daju manje naplate od prikazane pune godine.

Ovo nije neto dobit Grupe: porez, financiranje i eventualna dodatna korporativna alokacija nisu uključeni. Terenski rad, novi senzori i zahtjevna prilagodba pojedinog kupca također nisu u godišnjem paketu; morali bi se naplatiti odvojeno uz pripadajući trošak. Fiksni trošak ne treba nekritički zadržati istim za mnogo veći broj uređaja ili država.

### Kako se dobit lako izgubi

- Pri cijeni **2.000 EUR**, uz ostale iste pretpostavke, 100 uređaja daje **−25.000 EUR** godišnje; operativno pokriće raste na 150 uređaja.
- Pri cijeni 3.000 EUR i varijabilnom trošku **2.250 EUR**, 100 uređaja samo pokriva godišnje programske troškove.
- Uz **36 umjesto 12 ekspertnih sati**, varijabilni trošak raste na 3.300 EUR. Usluga tada gubi po uređaju već prije fiksnih troškova; veći volumen ne rješava problem.

**Zaključak ekonomike:** moguć je koristan servisni posao, ali nije automatski visokomarginalni SaaS. Najvažniji su naplativa vrijednost, ekspertni sati i standardizirano uključivanje korisnika. Izračuni su provjereni zasebnim aritmetičkim testovima; [potpuni kontrolni rezultati](../sources/O001_economics_check.md).

## 6. Gdje AI ima smisla

iPDCore već dokumentira ML grupiranje i klasifikaciju uzoraka parcijalnih izbijanja. To je domenska sposobnost, ne dokaz pouzdanog predviđanja svih kvarova. [S11]

Moj prijedlog dodatnog AI opsega je usko vezan uz ekonomiku: pomoći pri grupiranju ponovljenih upozorenja, usporedbi s ranijim nalazima i nacrtu izvještaja uz provjerljive podatke. Stručnjak odobrava nalaz. Ne prodavati generički chatbot kao zaštitu transformatora i ne koristiti generirani tekst kao samostalan sigurnosni signal.

Ako AI ne smanjuje ukupno vrijeme stručne obrade ili broj nepotrebnih intervencija, nema razloga uvoditi ga u ovaj paket.

## 7. Prava, sigurnost i granice — sažeto

Za početni paket preporučujem odvojene podatke svakog kupca, samo odobren pristup za njegovu uslugu, bez pretpostavke da se tuđi podaci smiju koristiti za zajedničko treniranje. Ne vezati početak za KPT podatke ili IP niti obećavati priključivanje svih konkurentskih uređaja bez provjere kompatibilnosti.

Važna javna napomena: iPDCore stranica uz **Demodulator cluster technology** navodi nedostupnost u SAD-u, UK-u, Njemačkoj, Austriji, Švicarskoj, Italiji i Lihtenštajnu. To nije opća zabrana TMS-a. Preporuka je početni paket ne temeljiti na toj specifičnoj funkciji za ta tržišta. Razlog ograničenja nije objašnjen na stranici. [S11]

PROZA-ini javni certifikacijski navodi ne prenose se automatski na svaku novu integraciju. Preporučeni početak ostaje read-only, dok postojeći lokalni alarmi, zaštita i odgovornost operatora ostaju aktivni. [S09]

## 8. Preporučeni ulazak — poslovna odluka, ne novi research zadaci

Predlažem jednu ograničenu probnu isporuku na 5–10 već nadziranih transformatora jednog kupca, približno 12 tjedana. Broj, trajanje i pragovi su prijedlog, ne potvrđeni plan KONČAR-a. Ne kupovati novu opremu za dokazivanje same usluge.

Isporuka treba pokazati: razumljiv kvartalni nalaz, evidenciju korisne odluke te utrošak rada i dodatnog povezivanja. Kao početni kriterij predlažem barem 30% manje ručnog vremena za usporediv izvještaj bez smanjenja njegove stručne kvalitete, ili drugi dokumentirani operativni dobitak koji kupcu opravdava naknadu. Zahtijevati dodatni plaćeni opseg ili obnovu usluge za komercijalno širenje; besplatno zadovoljstvo samo po sebi nije dokaz cijene.

Mali uzorak ne dokazuje smanjenje katastrofalnih kvarova. Njegova svrha je provjera standardizirane usluge, korisnosti nalaza i opsega rada. Ukupnu početnu pripremu ograničio bih na scenarijskih 50.000 EUR. Ako se bez većeg novog sustava ne može isporučiti, ne širiti ulaganje automatski.

Odbacio bih zaseban novi proizvod ako kupac već dobiva isti ishod iz TMS-a/servisa bez nezadovoljene potrebe. Odbacio bih fiksni jeftini paket ako ekspertni rad redovito prelazi njegovu ekonomiku. U tim slučajevima i dalje može imati smisla prodaja postojeće opreme ili naplata pojedinačne ekspertize.

## 9. Završna ocjena

**Tržište postoji. Tehnička povezanost s KONČAR-om je snažna. Profitabilnost je moguća, ali ovisi o opsegu usluge i naplativoj bazi.** Najrazumniji oblik je servisni dodatak postojećem proizvodu, predvođen Institutom uz odgovarajući prodajni kanal; ne velika višedruštvena platforma prije prvih prihoda.

Pouzdanost zaključka je visoka za postojanje dokumentiranih proizvoda i vanjske ponude, srednja za predloženi način ulaska, a niska za stvarnu cijenu, dostupne kapacitete i ostvarenu dobit. Te nepoznanice su ograničenje procjene, ne razlog da se ovaj javni research ostavi nedovršen.

**O001 je završen kao procjena iz javnih izvora. Sljedeći od ukupno šest zadataka je O002.**

## Izvori

Svi pregledani 22. 9. 2026.; nedatirane stranice prikazuju javno dostupnu ponudu, ne točan datum uvođenja funkcije.

- **S01:** [KONČAR Institut — Transformer monitoring system](https://www.koncar-institut.hr/en/transformer-monitoring-system). Funkcije i System architecture; ne interni as-built/API.
- **S02:** [Institut — Operations overview](https://www.koncar-institut.hr/en/operations-overview). Razvoj, vlastita rješenja i dijagnostičko-ispitne usluge.
- **S03:** [KONČAR D&ST](https://www.koncar.hr/en/koncar-distribution-and-special-transformers). Proizvodi, terenske usluge i postprodaja; broj godišnjih isporuka nije pretplatnička baza.
- **S04:** [Hitachi Energy — TXpert Services](https://www.hitachienergy.com/products-and-solutions/transformers/the-txpert-ecosystem/txpert-services). Paketi i dugoročni ugovori; bez usporedivog javnog cjenika.
- **S05:** [Reinhausen — Performance Contracts](https://www.reinhausen.com/servicedetail/transformer-services/performance-contracts-and-consulting-transformers). Monitoring, servis, kombinirani paketi i zasebne garancije.
- **S06:** [Camlin — ugovor s Neoenom](https://camlingroup.com/neoen-appoints-camlin-energy-to-deliver-global-high-voltage-transformer-monitoring-across-renewable-portfolio/). Objava 9. 6. 2026.; pilot, ugovor i plan širenja, ne potvrda dovršenog globalnog rollouta.
- **S07:** [Vaisala — KAMO slučaj](https://www.vaisala.com/en/case/how-one-electric-co-op-reduced-operations-and-maintenance-costs-versatile-dga-monitoring). Objava 3. 7. 2025.; događaji 2022.–2024.; opis dobavljača s procjenom kupčeve uštede.
- **S08:** [Hitachi — Tata Steel](https://www.hitachienergy.com/news-and-events/customer-stories/intelligent-transformers-from-hitachi-abb-power-grids-to-bolster-tata-steel-operations). Customer problem i početni deployment plan; opće postotke ušteda nisam koristio u modelu.
- **S09:** [KONČAR — PROZA Station](https://www.koncar.hr/en/digital/digital-soulutions-and-platforms/proza-station). Deployment i sigurnosni opis, ne dokaz nove TMS integracije.
- **S10:** [NEOS — Data Engineering](https://www.neos.hr/expertise/data-engineering/). Podatkovna integracija i streamovi; ne potvrda isporučenog TMS rješenja.
- **S11:** [Institut — iPDCore](https://www.koncar-institut.hr/en/partial-discharge-measurement-and-monitoring-system-ipd-core). ML grupiranje/klasifikacija i teritorijalna napomena uz Demodulator cluster technology.

Raniji detaljni tehnički pregled ostaje u [R006](../research/R006_O001_existing_stack_offer_audit_2026-09-22.md). Ovaj dokument zamjenjuje prethodni status O001 koji je čekao interne podatke i njegove A–E podzadatke.
