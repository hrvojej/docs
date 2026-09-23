# O006 — provjerena scenarijska ekonomika

**23. 9. 2026.** [O006](../opportunities/O006_renewable_bess_intelligence_optimization_service.md) · [Glavni indeks](../MASTER_INDEX.md)

Svi ulazi su eksplicitne pretpostavke, EUR bez PDV-a. Nema aktualnog cjenika, internih troškova, stvarnog backtesta ili ostvarenog profita. A prikazuje pružatelja usluge, B i C kupca. Ne zbrajati ih. Izvori za tržišni/tehnički kontekst su u O006; ovaj dokument provjerava aritmetiku.

## A. Pružatelj portfolio-performance usluge

P = 18.000/lokacija/god.; C = 48 h × 100 + 1.200 podaci/licence + 2.000 podrška = 8.000; F = 120.000/god.; početni I = 150.000.

F nije drugi obračun istih 48 stručnih sati po lokaciji. I je ograničena nadogradnja postojeće osnove, ne novi industrijski EMS/trgovačka platforma. Oprema, posebni priključci i nova terenska ekipa nisu besplatno uključeni. Troškovi uvođenja koji premašuju standardni opseg mijenjaju model; dodatni onboarding prihod nije dodan.

`R = N × P`

`B = N × (P − C) − F`

`B_first = B − I`

| N | R | NC | F | B | I | B_first | Ekspertni sati |
|---:|---:|---:|---:|---:|---:|---:|---:|
| 10 | 180.000 | 80.000 | 120.000 | −20.000 | 150.000 | −170.000 | 480 |
| 20 | 360.000 | 160.000 | 120.000 | 80.000 | 150.000 | −70.000 | 960 |
| 40 | 720.000 | 320.000 | 120.000 | 280.000 | 150.000 | 130.000 | 1.920 |

Točka nule godišnje: F/(P−C) = 12, pozitivno od 13. Prva godina: (F+I)/(P−C) = 27, pozitivno od 28. Provjerene susjedne cijele vrijednosti 11/12/13 i 26/27/28. Ako P≤C, rast broja lokacija ne daje pozitivan doprinos pod ovim troškovima.

| Osjetljivost | N | P | C | F | I | B | B_first |
|---|---:|---:|---:|---:|---:|---:|---:|
| Niža cijena | 20 | 12.000 | 8.000 | 120.000 | 150.000 | −40.000 | −190.000 |
| C +50% | 20 | 18.000 | 12.000 | 120.000 | 150.000 | 0 | −150.000 |
| Veća početna izgradnja | 40 | 18.000 | 8.000 | 120.000 | 500.000 | 280.000 | −220.000 |
| Prosječno samo 10 lokacija prve godine | 10 | 18.000 | 8.000 | 120.000 | 150.000 | −20.000 | −170.000 |

Punogodišnji N nije broj ugovora na kraju godine. Nema prognoze osvojivog tržišta, dvostrukog brojanja sadašnjeg servisa, neto dobiti, poreza/financiranja/radnog kapitala ili nepoznate dodatne režije.

## B. Kupac: dodatno vraćena solarna proizvodnja

20 MWp × 1.300 MWh/MWp/god. = 26.000 MWh. Neto granična vrijednost = 70 EUR/MWh. Godišnja naknada = 18.000; dodatna provedba korekcije = 5.000. Sve scenarij, ne cijena električne energije ili izmjerena proizvodnost.

`gross = 26.000 × stvarni_povrat_proizvodnje × 70`

`net = gross − 23.000`

| Stvarni povrat | MWh | Gross | Net |
|---:|---:|---:|---:|
| 0,5% | 130 | 9.100 | −13.900 |
| 1% | 260 | 18.200 | −4.800 |
| 2% | 520 | 36.400 | 13.400 |

Pokriće `23.000 / (26.000 × 70) = 0,0126373626`, odnosno **1,263736%**. To je dodatak povrh postojećeg održavanja i ograničenja, ne udio samo prepoznatih problema.

Za 5 MWp i isti 1%: 5 × 1.300 × 0,01 × 70 = 4.550 gross; nakon iste naknade i korekcije net = **−18.450**. Skupi ekspertni paket nije primjeren svakoj maloj lokaciji. Prihod mora biti isporučiv/naplativ; curtailment, cijene i ugovori mogu ga smanjiti. Dodatne uštede rada nisu dodane.

## C. Kupac: BESS arbitraža i inkrementalni optimizer

Postojeći sustav 1 MW; isporučivo 2 MWh/ciklus × 250 ciklusa = 500 MWh na AC izlazu godišnje. Pretpostavljena ukupna učinkovitost 0,88: punjenje `500/0,88 = 568,181818 MWh`. Degradacija 25 EUR/isporučeni MWh, ostale varijabilne naknade 5. Dodatni optimizer = 10.000/god. Nema baterijskog CAPEX-a ni prihoda rezerve snage.

`arbitrage_net_before_optimizer = Qout × sell − (Qout/eta) × buy − Qout × (degradation + fees)`

`incremental_after_optimizer = enhanced − baseline − optimizer_fee`

| Varijanta | Buy | Sell | Prodaja EUR | Trošak kupnje | Degradacija | Ostale var. naknade | Net prije optimizatora |
|---|---:|---:|---:|---:|---:|---:|---:|
| Jednostavni EMS | 55 | 100 | 50.000 | 31.250 | 12.500 | 2.500 | 3.750 |
| Bolji raspored | 40 | 110 | 55.000 | 22.727,272727 | 12.500 | 2.500 | 17.272,727273 |
| Slabiji raspored | 40 | 90 | 45.000 | 22.727,272727 | 12.500 | 2.500 | 7.272,727273 |

Bolji raspored: dodatno prije naknade 13.522,727273; nakon 10.000 = **3.522,727273**.

Slabiji raspored prema istoj referenci: 7.272,727273−3.750−10.000 = **−6.477,272727**.

Naknada od 20% boljeg neto poboljšanja prije naknade iznosila bi samo 2.704,545455/god., prije troškova pružatelja. To je alternativa fiksnoj naknadi, ne dodatak; pokazuje potrebu za odgovarajućim razmjerom lokacije/portfelja.

Ovo nije optimizacijski algoritam ili validirani backtest. Buy/sell su pretpostavljeni ostvareni ponderirani prosjeci; nema tvrdnje da se mogu predvidjeti. Podrazumijevaju se isti SOC na početku/kraju, jednak opseg dostupnosti i ista operativna/ugovorna ograničenja. Različiti ciklusi zahtijevaju različitu degradaciju. PV punjenje ima oportunitetni trošak. Rezerva snage i arbitraža ne smiju dvostruko koristiti iste resurse.

## D. Završna usporedba — način tumačenja

O001–O003 i digitalni dio O005 prikazuju scenarijski doprinos pružatelja; O004 internu vrijednost dodatne isporuke; O005 depo i B/C ovog dokumenta korist kupcu. Početni troškovi, timovi i volumeni nisu jednaki. Nema zbrajanja u navodni profit Grupe niti rangiranja prema najvećem nominalnom iznosu. Izračuni O001–O005 ostaju u njihovim računskim prilozima; ovdje nisu ponovno proglašeni tržišnim podacima.

## Kontrola izvršavanja

**65/65 automatskih provjera uspješno.** Uključeni zbrojevi, dvije neovisne formulacije doprinosa, Decimal/Fraction identiteti, granice pozitivnog rezultata, pad cijene, rast troška, nula lokacija, negativni ulazi, PV prag i energetska bilanca s gubicima. Skripta je izvršena dvaput; izlazni rezultati su identični bajt po bajt.

Lokalno u `/mnt/data/koncar_o006/`: `check_economics.txt` (izvor kao tekst), `O006_economics_results.txt` (svi ulazi/izlazi/testovi), `O006_economics_results_run1.txt`, `O006_debug_log.txt`, `O006_debug_run1.txt`, `O006_run_stdout.txt`, `O006_run_stderr.txt`, `O006_repeat_stdout.txt`, `O006_repeat_stderr.txt`, `O006_final_test_summary.txt`. To su putanje ove sesije, ne trajni web URL-ovi; kanonski trajni poslovni rezultati sačuvani su u ovom MD-u.

Opcionalni lokalni dohvat javnog GitHub sadržaja nije uspio zbog DNS-a. Povezani GitHub alat korišten je za čitanje i pohranu; matematika ne koristi mrežu. Nisu izvršeni SQL upiti, interni pristupi, intervjui, kontrole stvarne baterije ili pilot.
