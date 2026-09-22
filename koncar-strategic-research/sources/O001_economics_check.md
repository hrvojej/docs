# O001 — kontrola scenarijskog izračuna

Datum: 2026-09-22. [O001 izvještaj](../opportunities/O001_transformer_intelligence_lifecycle_service.md) · [Master](../MASTER_INDEX.md).

**Ovo je kontrola matematike, ne potvrda tržišnih cijena ili financija KONČAR-a.** Nema internih podataka, SQL upita, ponude dobavljača ni provedene prodaje.

## Puni ulazi

P = 3.000 EUR po uređaju/godini; stručni rad 12 sati × 75 EUR = 900; podaci/hosting 150; korisnička podrška 250; varijabilna rezerva 200. Ukupni V = 1.500 EUR po uređaju/godini. F = 75.000 EUR godišnjih fiksnih programskih troškova. K = 50.000 EUR početnog izdatka. Sve su to izričite pretpostavke autora.

Prihod = N × P. Varijabilni trošak = N × V. Godišnji doprinos = N × (P − V) − F. Prva puna godina nakon početnog izdatka = N × (P − V) − F − K.

## Puni rezultati osnovnih scenarija

| N | Prihod | Varijabilni trošak | F | Doprinos | K | Prva godina nakon K |
|---:|---:|---:|---:|---:|---:|---:|
| 30 | 90.000 | 45.000 | 75.000 | −30.000 | 50.000 | −80.000 |
| 50 | 150.000 | 75.000 | 75.000 | 0 | 50.000 | −50.000 |
| 100 | 300.000 | 150.000 | 75.000 | 75.000 | 50.000 | 25.000 |
| 200 | 600.000 | 300.000 | 75.000 | 225.000 | 50.000 | 175.000 |

Operativno pokriće = 75.000 / 1.500 = **50** punogodišnjih uređaja. Pokriće uključujući početni izdatak = 125.000 / 1.500 = 83,333…; najmanji cijeli broj uređaja je **84**. To nije prognoza prodaje.

## Puni rezultati osjetljivosti

| Slučaj | P | V | Doprinos pri N=100 | N za operativno pokriće |
|---|---:|---:|---:|---:|
| Niža cijena | 2.000 | 1.500 | −25.000 | 150 |
| Viši varijabilni trošak | 3.000 | 2.250 | 0 | 100 |
| 36 ekspertnih sati umjesto 12 | 3.000 | 3.300 | −105.000 | Nema pozitivnog pokrića povećanjem volumena |

Za zadnji red: 36 × 75 + 150 + 250 + 200 = 3.300 EUR.

## Što je provjereno

Izračun je izvršen neovisnom Python provjerom. Za svaki osnovni red uspoređene su formule `prihod − svi godišnji troškovi` i `N × jedinični doprinos − F`, te rezultat prve godine i sve osjetljivosti. Svi aritmetički testovi prošli su; izvorni puni rezultati spremljeni su u `calculation_results.json`, a detaljni debug trag u `debug.txt` tijekom ove sesije. Ovaj MD čuva sve materijalne ulaze i rezultate za buduće chatove, neovisno o lokalnom runtimeu.

## Granice

Izračun je za punu godinu naplate, na već opremljenim i dostupnim uređajima. Ne uključuje PDV, porez na dobit, financiranje, dodatnu korporativnu alokaciju, nove senzore ni teren. Novi hardver, složeni onboarding i teren moraju imati zasebnu cijenu i trošak. Programski rad postojećih stručnjaka nije besplatan. Rast F iznad prikazanog opsega, postupno ugovaranje i gubitak kupaca mogu pogoršati rezultat.
