# O005 — provjera ekonomike: vlakovi, tramvaji, ADAS i autonomni depo

**23. 9. 2026.** [Završni O005](../opportunities/O005_rail_fleet_battery_intelligence_service.md) · [Master](../MASTER_INDEX.md)

Svi iznosi su ilustrativni EUR bez PDV-a, ne stvarne cijene, troškovi KONČARA ili prognoza. Četiri modela su **odvojena**: A je doprinos pružatelja digitalnog servisa, B doprinos projektne ADAS ugradnje, C korist operatora vozovnice, D provjera energetske pretpostavke. Ne zbrajati kupčevu uštedu s dobavljačevim prihodom. Nema provedenih pilota, intervjua ili SQL upita.

## A. Digitalni servis srodne flote

### Ulazi

| Parametar | Pretpostavka |
|---|---:|
| P: godišnja naknada po vozilu/paketu | 4.500 |
| Ekspertni rad po vozilu: 12 h × 90 | 1.080 |
| Podaci/connectivity/pohrana | 240 |
| Podrška i rezerva po vozilu | 480 |
| C: zbroj varijabilnog troška | 1.800 |
| F: godišnja središnja programska funkcija | 90.000 |
| I: početno uvođenje na postojeći temelj | 100.000 |

N je broj punogodišnje naplaćenih vozila usporedivog opsega. Nije univerzalna cijena svih vlakova/tramvaja; nije broj isporučenih vozila. Hardver, safety retrofit i složeni charging optimizer odvojeno. F ne broji ponovno iste ekspertne sate. I ne predstavlja razvoj platforme od nule.

`R = N × P`

`B = N × (P − C) − F = 2.700N − 90.000`

`B1 = B − I`

| N | R | N×C | B | B1 |
|---:|---:|---:|---:|---:|
| 30 | 135.000 | 54.000 | −9.000 | −109.000 |
| 50 | 225.000 | 90.000 | 45.000 | −55.000 |
| 100 | 450.000 | 180.000 | 180.000 | 80.000 |
| 150 | 675.000 | 270.000 | 315.000 | 215.000 |

Operativni prag `ceil(90.000/2.700) = 34`: 33 daje −900; 34 daje 1.800. Prvogodišnji prag `ceil(190.000/2.700) = 71`: 70 daje −1.000; 71 daje 1.700.

| Osjetljivost pri N=100 | P | C | B | B1 |
|---|---:|---:|---:|---:|
| Osnovno | 4.500 | 1.800 | 180.000 | 80.000 |
| Niža cijena | 3.000 | 1.800 | 30.000 | −70.000 |
| C +50% | 4.500 | 2.700 | 90.000 | −10.000 |

Ovo nije neto dobit: bez poreza, financiranja, mjesečnog cash-flowa, radnog kapitala i eventualne dodatne korporativne režije. Već ugovoreni maintenance/warranty opseg ne smije se ponovno brojiti kao dodatni prihod.

## B. Sigurnosni ADAS dodatak — jedna serija

P = 35.000 po tramvaju, C = 25.000, doprinos 10.000. Jednokratna prilagodba/integracija/ispitivanje I = 300.000 za postojeću kvalificiranu osnovu i ograničen opseg. To nije dokaz da se za taj iznos može razviti/homologirati novi aktivni sustav kočenja ili puna autonomija.

`projektni_doprinos = N × (P − C) − I`

| N | Prihod | Varijabilno | Nakon I |
|---:|---:|---:|---:|
| 20 | 700.000 | 500.000 | −100.000 |
| 30 | 1.050.000 | 750.000 | 0 |
| 50 | 1.750.000 | 1.250.000 | 200.000 |
| 100 | 3.500.000 | 2.500.000 | 700.000 |

Prag 30. Ovo nije godišnji ARR; nisu dodani potencijalni kasniji ugovori podrške. Ako stvarni troškovi sigurnosti, jamstva ili prilagodbe prelaze pretpostavke, računica se mijenja. Različite serije/gradovi mogu zahtijevati zasebnu pripremu.

Ako ilustrativni preostali vlastiti razvoj iznosi 2.000.000 uz isti doprinos, prag postaje 200 ugradnji. Pri 40 ugradnji rezultat je −1.600.000. Taj iznos nije procjena ni gornja granica autonomnog razvoja; demonstrira rizik amortiziranja razvoja na maloj seriji. Povijesni SafeTram grant nije novi prihod.

### Odvojeni kupčev prag za ADAS

Ugradnja 35.000 kroz 10 godina, godišnja podrška 2.000: godišnji ekvivalent bez diskontiranja 5.500. Ako se **hipotetski** relevantni trošak materijalnih nezgoda/zastoja smanji 30%, neutralni početni godišnji trošak je `5.500/0,30 = 18.333,33`. To nije izmjeren rizik ili dokaz tog postotka. Ne monetizira se ljudski život; sigurnosna obveza/zahtjev može biti važniji od ovog uskog materijalnog povrata. Pri diskontiranju ili kraćem vijeku potreban ekonomski učinak raste.

## C. Autonomni depo — kupčeva ekonomika

### Ulazi i obuhvat

| Parametar | Pretpostavka |
|---|---:|
| Vozila dnevno V | 60 |
| Operativni dani D | 330 |
| Trošak sata rada c | 35 |
| Dio oslobođenog rada stvarno realiziran u vrijednost u | 75% |
| Početni sustav/retrofit/infrastruktura/integracija K | 1.500.000 |
| Dodatni godišnji troškovi F | 100.000 |

K nije javna ponuda niti trošak novog vlastitog temeljnog razvojnog programa. F pretpostavlja održavanje, licence, dodatni nadzor i rezervu. Promijeniti F ako preostalo osoblje košta više. h su **person-hours po vozilu/danu stvarno oslobođeni za drugo korištenje**, ne trajanje automatske vožnje/pranja bez prethodno potrebnog ljudskog rada.

`gross = V × D × h × c × u = 519.750h`

`B = gross − F`

`jednostavni_povrat = K/B`, samo ako B > 0.

| h | Minute | Gross | B kupca godišnje | Jednostavni puni povrat |
|---:|---:|---:|---:|---:|
| 0,25 | 15 | 129.937,50 | 29.937,50 | 50,1044 god. |
| 0,5 | 30 | 259.875 | 159.875 | 9,3823 god. |
| 1 | 60 | 519.750 | 419.750 | 3,5736 god. |

Za petogodišnji jednostavni povrat uz puni učinak:

`h ≥ (K/5 + F)/(V×D×c×u) = 400.000/519.750 = 0,76960077 h`

odnosno **46,1760 minuta po tramvaju/danu**. Na 46 min uvjet nije dostignut, na 47 jest. To je scenarijski prag, ne univerzalna preporuka za nabavu depoa.

### Downside i uhodavanje

Pri h=0,5 i u=25%: gross=86.625; B=**−13.375**. Ako oslobođeni rad uopće nema ekonomsku realizaciju, B=−100.000 u ovom modelu. Nema implicitne uštede svih vozačkih plaća.

Za h=1, uz 50% bruto učinka u prvoj godini: B1=159.875, naredne godine 419.750. Povrat iznosi `1 + (1.500.000−159.875)/419.750 = 4,192674` godina uz ravnomjernu realizaciju unutar godine. Bez poreza, diskonta, financiranja ili rezidualne vrijednosti; nije NPV ili jamstvo. Pri većem početnom ulaganju/preostalom osoblju povrat se pogoršava.

Dobit KONČARA od projekta nije ova ušteda: ona bi bila ugovoreni prihod minus oprema, partneri, vlastiti razvoj/integracija, ispitivanje, podrška, garancije i režija. Ti ugovorni podaci nisu javni pa profit autonomnog-depot izvođača nije izmišljen.

## D. Energetski kontra-primjer

Ilustracija: 1.000 MWh prihvatljive energije, od čega se može vremenski pomaknuti samo 30%, uz razliku 20 EUR/MWh.

`gross = 1.000 × 0,30 × 20 = 6.000`

`net = 6.000 − 8.000 dodatnog trošenja/gubitaka/podrške = −2.000`

Sve pretpostavke, ne aktualna cijena struje ili izmjerena potrošnja. Ne koristiti buduće cijene kao poznate u backtestu; usporediti s jednostavnom izvedivom politikom punjenja. Nije zbrojeno s A/B/C.

## Kontrola

Izvršeno **51/51 provjera**, zatim ponovljeno izvršavanje s identičnim izlazom. Decimal preciznost 32; neovisna Fraction provjera depot računice, pragovi i susjedne cijele vrijednosti, osjetljivosti i računovodstveni identiteti. Izlazni SHA256:

`69feead902203693a8a2e5399e459a2b769202117da6b3a7e78e3c2f8ea20227`

Lokalni artefakti ove sesije u `/mnt/data/koncar_o005/`: `check_economics.txt` (izvršeni Python izvor kao tekst), `O005_economics_results.txt` (potpuni ulazi/izlazi i testovi), `O005_debug_log.txt`, kopija prvog izvođenja i zasebni stdout/stderr za oba izvođenja te `O005_test_summary.txt`. To su zabilježene lokalne putanje, ne trajni javni linkovi. Ovaj MD trajno čuva sve poslovne ulaze, rezultate i testni sažetak; javni izvori za kontekst su u O005. Nema mrežnog pristupa, SQL-a ili internih sustava u računskom skriptu.
