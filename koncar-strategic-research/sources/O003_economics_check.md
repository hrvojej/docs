# O003 — provjera scenarijske ekonomike

**Datum: 22. 9. 2026.** [O003 završni izvještaj](../opportunities/O003_hydro_underwater_inspection_lifecycle_service.md) · [Master](../MASTER_INDEX.md)

Sve novčane pretpostavke su u EUR bez PDV-a. Nisu KONČAR-ovi stvarni troškovi, ponude dobavljača ili prognoza prodaje. Javni izvori za kontekst i razliku osnovnog ROV-a od cjelovite usluge nalaze se u O003, S01–S13. Ovaj prilog provjerava aritmetiku, ne tržišnu spremnost na plaćanje.

## A. Partnerska hidro-inspekcijska usluga

### Ulazi i obuhvat

Jedna kampanja = priprema, jedan planirani terenski dan na omeđenoj dostupnoj lokaciji i izvještaj. Tri puna dana hidro-inženjera po kampanji. Partnerov paket modelira potrebnu ROV opremu i dvije operativne uloge u dogovorenom dnevnom opsegu; ovo nije propisani minimum ekipe.

| Ulaz | Pretpostavka |
|---|---:|
| Cijena P | 6.500 |
| Partnerov ROV/operativni paket | 2.200 |
| Hidro-inženjer: 3 × 450 | 1.350 |
| Put i mobilizacija izvan partnerova paketa | 450 |
| Podaci/manja misijska rezerva | 200 |
| Varijabilni trošak C | **4.200** |
| Godišnji fiksni trošak F | 40.000 |
| Početna priprema I | 15.000 |

F pokriva prodaju, koordinaciju, opću kvalitetu, osiguranje/podršku; ne naplaćuje još jednom iste inženjerske dane iz C. Početna priprema nije razvoj velike softverske platforme. Troškovi su puni resursni troškovi u okviru postojeće organizacije, a ne pretpostavka besplatnih zaposlenika.

### Formule

`C = 2.200 + 3 × 450 + 450 + 200 = 4.200`

`doprinos_po_kampanji = P − C = 2.300`

`prihod = N × P`

`godišnji_rezultat = N × (P − C) − F`

`prva_godina_nakon_pripreme = godišnji_rezultat − I`

`operativno_pokriće = ceil(F / (P − C)) = ceil(40.000 / 2.300) = 18`

`prva_godina_pokriće = ceil((F + I) / (P − C)) = ceil(55.000 / 2.300) = 24`

Ako je P ≤ C, veći volumen ne popravlja negativni doprinos i ovakva formula za konačan prag nema smisla.

### Potpuni izlazi

| N | Prihod | Varijabilni trošak | F | Godišnji rezultat | Nakon I | Inženjerski dani |
|---:|---:|---:|---:|---:|---:|---:|
| 10 | 65.000 | 42.000 | 40.000 | −17.000 | −32.000 | 30 |
| 20 | 130.000 | 84.000 | 40.000 | 6.000 | −9.000 | 60 |
| 40 | 260.000 | 168.000 | 40.000 | 52.000 | 37.000 | 120 |
| 60 | 390.000 | 252.000 | 40.000 | 98.000 | 83.000 | 180 |

Provjera granice: 17 kampanja daje −900 godišnje, 18 daje +1.400. U prvoj godini 23 daju −2.100, 24 daju +200 nakon pripreme.

### Osjetljivost pri 40 kampanja

| Scenarij | P | C | Godišnji rezultat | Nakon I |
|---|---:|---:|---:|---:|
| Osnovni | 6.500 | 4.200 | 52.000 | 37.000 |
| Niža prodajna cijena | 5.000 | 4.200 | **−8.000** | −23.000 |
| C viši za 25% | 6.500 | 5.250 | **10.000** | −5.000 |

Ovo nije neto dobit ni model novčanog toka po mjesecima. Nisu uključeni porezi, financiranje, radni kapital, nepoznata dodatna korporativna režija ili neosigurana velika šteta. Nema dodanih hipotetskih prihoda od remonta, drugih tržišta ili spriječenih kvarova. Već postojeću prodaju ne brojiti ponovno kao inkrementalni prihod.

## B. Najam nasuprot kupnji — samo oprema

**Ne uspoređuje se s punim partnerovim operativnim paketom iz A.** Posada, kvalifikacije, misijska kvaliteta i zajednički troškovi moraju biti isti. Različite troškove obuke, transporta, osoblja, dozvola ili rizika treba dodati prije konkretne odluke. Ovaj model nije dodatni prihod ili dobit uz A.

| Ulaz | Pretpostavka |
|---|---:|
| Kupljeni konfigurirani sustav K | 45.000 |
| Vijek L | 5 godina |
| Rezidualna vrijednost | 0 |
| Godišnja amortizacija K/L | 9.000 |
| Godišnji servis/osiguranje, novčani trošak M | 6.000 |
| Varijabilna uporaba/trošenje po kampanji V | 200 |
| Najam po kalendarskom danu r | 600 |
| Naplativi dani najma po kampanji d | 3 |

45.000 EUR nije preračunata cijena osnovnog BlueROV2. 600 EUR nije verificirana najamnina. Oboje je pretpostavka za funkcionalno usporediv sustav.

`rent(N) = r × d × N = 1.800N`

`own_annual(N) = K/L + M + VN = 15.000 + 200N`

`own_first_year_cash(N) = K + M + VN = 51.000 + 200N`

| N | Trošak najma | Godišnji trošak vlasništva s amortizacijom | Prvi godišnji novčani izdatak vlasništva | Godišnja prednost vlasništva |
|---:|---:|---:|---:|---:|
| 5 | 9.000 | 16.000 | 52.000 | −7.000 |
| 10 | 18.000 | 17.000 | 53.000 | 1.000 |
| 20 | 36.000 | 19.000 | 55.000 | 17.000 |
| 40 | 72.000 | 23.000 | 59.000 | 49.000 |

Godišnja prednost počinje od `ceil(15.000/1.600) = 10` kampanja. Prvi godišnji novčani izdatak niži je od najma od `ceil(51.000/1.600) = 32` kampanje.

Trogodišnji nediskontirani cash model uz konstantan N godišnje i bez prodaje opreme na kraju: `K + 3M + 3VN` nasuprot `3rdN`. Prag je `ceil(63.000/4.800) = 14 kampanja godišnje`. Nije NPV model; ne uključuje financiranje, razlike u kvarovima niti korisnički zahtjev za određenim rokom povrata.

### Zašto broj kalendarskih dana mijenja odluku

Ako je d = 1, najam iznosi 600N. Razlika po kampanji pada na 400 EUR; godišnji prag vlasništva postaje **38**, a prag prvogodišnjeg novčanog izdatka **128** kampanja. Zajednički najam za više susjednih poslova može bitno promijeniti računicu. Ne pretvarati prag 10 ili 32 u univerzalno pravilo nabave.

## C. Kupčeva vrijednost izbjegnutog zastoja

Ilustrativna formula: `pogođeni_MW × stvarno_ušteđeni_sati × neto_doprinos_EUR_MWh × udio_nepovratno_izgubljene_proizvodnje`.

Za 10 MW, 12 sati i pretpostavljenih 80 EUR/MWh:

| Nepovratni udio | Izbjegnuti ekonomski gubitak |
|---:|---:|
| 0% | 0 |
| 25% | 2.400 |
| 100% | 9.600 |

Ovo nije spot cijena, zajamčena ušteda, vrijednost cijelog remonta ili dokaz spremnosti na plaćanje. Mogući troškovi pristupa i alternativnog ispitivanja uspoređuju se odvojeno. Pražnjenje koje se svakako mora provesti radi popravka ne može se u cijelosti pripisati izbjegnutoj inspekciji.

## D. AI kao pomoć izvještavanju — razmjer

Pretpostavka pola inženjerskog dana uštede po kampanji: `40 × 0,5 × 450 = 9.000 EUR/godina` bruto vrijednosti kapaciteta prije softvera i održavanja. Novčana korist zahtijeva stvarno iskorištavanje oslobođenog kapaciteta. Nije pribrojeno marži iz A.

## Provjera i zapis izvršavanja

Provedeno **39/39 uspješnih automatskih provjera**, uključujući zbroj sastavnica, unaprijed izračunate rezultate, iste identitete kroz drugu formulu, Decimal/Fraction provjere pragova i njihove susjedne cijele vrijednosti. Provjera AI kapaciteta dodana je zasebno nakon osnovnog izračuna. Nikakvi interni sustavi, intervjui ili SQL upiti nisu korišteni.

Lokalni audit ovog izvršavanja spremljen je u `/mnt/data/koncar_o003/`: `check_economics.txt` (Python izvor kao tekst), `O003_economics_results.txt` (svi ulazi/izlazi/testovi), `O003_debug_log.txt` (DEBUG), `O003_run_stdout.txt`, `O003_run_stderr.txt` i `O003_final_test_summary.txt`. Putanje su zapis konkretne sesije, ne trajni javni URL. Kanonski trajni sažetak i svi poslovni rezultati su ovaj MD i povezani O003.

Opcionalni lokalni dohvat javnog GitHub teksta nije uspio zbog DNS ograničenja; repozitorij je čitan i ažuriran povezanim GitHub alatom. To ne utječe na lokalnu računicu bez mreže.
