# O004 — kontrola scenarijske ekonomike

**22. 9. 2026.** [O004 završni izvještaj](../opportunities/O004_adaptive_heavy_fabrication_program.md) · [Glavni indeks](../MASTER_INDEX.md)

Ovo je provjera autorskog modela, ne dokaz stvarnih KONČAR troškova, kapaciteta, potražnje ili profita. Sve cijene/troškovi u EUR bez PDV-a su pretpostavke. Jedanaest javnih primarnih izvora za kontekst navedeno je u O004; povijesna investicija KMK-a iz 2022. nije osnova preračunavanja cijene ovog scenarija.

## 1. Obuhvat i ulazi

Model: ciljana nadogradnja postojeće kompatibilne ćelije, bez nove hale, kompletnog robota/linije ili velikog zasebnog AI tima. I = 120.000 početno: 25.000 softver/postprocesor, 35.000 senzori/naprave, 40.000 integracija/obuka/kvalifikacija, 20.000 prekid/rezerva. Zbroj = 120.000. To je scenarijski paket, ne dobavljačeva ponuda niti preporučeni automatski budžet.

F = 20.000 dodatnog godišnjeg troška licenci, servisa i dodatne programske podrške. H = 300/800/1.400 neto oslobođenih sati ograničavajuće ćelije godišnje; uključiti gubitke zbog mjerenja, traženja, izmjena, dorada i rukovanja prije određivanja H. u = 0,75 je dio tih sati koji se stvarno pretvara u kvalitetan prodan i isporučen izlaz. c = 150 doprinos po realiziranom satu nakon svih dodatnih troškova novih proizvoda, prije F.

c nije prodajna cijena niti satnica radnika. Plaće i isti sati ne broje se ponovno kao dodatna ušteda. Roba proizvedena na zalihu bez isporuke ne daje ovaj pretpostavljeni cash učinak. Novi kapacitet drugih potrebnih strojeva nije besplatan.

## 2. Formule

```
realizirani_sati = H * u
gross = H * u * c
B = gross - F
simple_payback = I / B  (samo B > 0)
first_full_year_after_I = B - I
max_I_for_2_year_simple_payback = max(0, 2 * B)
```

B je inkrementalni operativni doprinos prije amortizacije, poreza, financiranja, promjene radnog kapitala i nepoznate dodatne korporativne režije. Za pojednostavljeni payback/NPV pretpostavlja se da taj doprinos ujedno postaje operativni novčani priljev. To je dodatna pretpostavka, ne potvrđen stvarni cash flow. I je početni izdatak; amortizacija se ne oduzima još jednom u cash izračunu.

## 3. Potpuni rezultati tri scenarija

| H | u | c | Realizirani sati | Gross | F | B | I | Jednostavni povrat, godina | Prva puna godina nakon I | Najveći I za 2 godine povrata |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 300 | 75% | 150 | 225 | 33.750 | 20.000 | **13.750** | 120.000 | 8,7273 | −106.250 | 27.500 |
| 800 | 75% | 150 | 600 | 90.000 | 20.000 | **70.000** | 120.000 | 1,7143 | −50.000 | 140.000 |
| 1.400 | 75% | 150 | 1.050 | 157.500 | 20.000 | **137.500** | 120.000 | 0,8727 | 17.500 | 275.000 |

Provjera preko proizvoda: srednji red odgovara ilustrativnih 60 dodatnih sklopova × 1.500 doprinosa, ako sklop troši 10 sati ćelije. 60 × 1.500 = 90.000; to nije dodatni iznos povrh gross-a.

H = 800 je 20% hipotetskog fonda ćelije od 4.000 h/god.; H = 1.400 je 35%. Nisu pretpostavljene izmjerene rezerve. Ako takvi neto sati nisu oslobođeni, pripadajući red ne vrijedi.

## 4. Operativni prag i cilj povrata

Efektivni doprinos po oslobođenom satu: u × c = 0,75 × 150 = 112,50.

- Operativno pokriće: ceil(20.000 / 112,5) = **178 sati**. Pri 177 sati B = −87,50; pri 178 sati B = +25.
- Dvogodišnji jednostavni povrat pri punom godišnjem učinku: ceil((120.000/2 + 20.000) / 112,5) = **712 sati**. Pri 711 sati B = 59.987,50 < 60.000; pri 712 sati B = 60.100 ≥ 60.000.

Operativni prag ne znači povrat investicije. Dvogodišnji cilj je ilustrativni kriterij, ne KONČAR-ova odobrena stopa/prag ulaganja.

## 5. Osjetljivost srednjeg slučaja H = 800

| Varijanta | u | c | F | I | B | Jednostavni povrat, godina |
|---|---:|---:|---:|---:|---:|---:|
| Osnovno | 75% | 150 | 20.000 | 120.000 | 70.000 | 1,7143 |
| Realizacija samo 25% | 25% | 150 | 20.000 | 120.000 | **10.000** | 12 |
| Doprinos prepolovljen | 75% | 75 | 20.000 | 120.000 | **25.000** | 4,8 |
| Nema dodatne isporuke | 0% | 150 | 20.000 | 120.000 | **−20.000** | Nema povrata |
| Viši godišnji trošak | 75% | 150 | 35.000 | 120.000 | 55.000 | 2,1818 |
| Viši početni izdatak | 75% | 150 | 20.000 | 200.000 | 70.000 | 2,8571 |

Pozitivan gross ne znači automatski atraktivan projekt. Ako u = 0, dodatni kapacitet nema monetizaciju u ovom modelu. Posebne stvarne uštede mogu se računati odvojeno samo bez preklapanja.

## 6. Uhodavanje i diskontiranje

Srednji slučaj; u prvoj godini postiže se pola kasnijeg bruto doprinosa, a F se plaća u cijelosti. Troškovi početne integracije/prekida ostaju u I; sporiji komercijalni rast odražava se u manjem gross-u, bez ponovnog zbrajanja istog prekida.

| Godina | Operativni priljev po pretpostavci | Početni izdatak | Kumulativno bez diskonta |
|---:|---:|---:|---:|
| 0 | 0 | −120.000 | −120.000 |
| 1 | 45.000 − 20.000 = 25.000 | 0 | −95.000 |
| 2 | 70.000 | 0 | −25.000 |
| 3 | 70.000 | 0 | 45.000 |
| 4 | 70.000 | 0 | 115.000 |
| 5 | 70.000 | 0 | 185.000 |

Povrat uz ravnomjerni priljev unutar treće godine: 2 + 25.000/70.000 = **2,3571 godina**. To nije 1,7143 iz tablice punog učinka.

Pretpostavka diskonta 10%, pet godina, ostatak 0:

`NPV = -120000 + 25000/1.1 + 70000/1.1^2 + 70000/1.1^3 + 70000/1.1^4 + 70000/1.1^5`

**NPV = 104.445,98 EUR.** Pretporezni scenarij bez financiranja/radnog kapitala; 10% nije utvrđeni KONČAR WACC. Nije investicijsko odobrenje.

## 7. Odvojeni savings-only scenarij

Bez dodatnog volumena, ali uz 26.000 stvarno izbjegnutih godišnjih vanjskih dorada/prekovremenih/materijalnog škarta: 26.000 − 20.000 = **6.000** godišnje. I = 120.000 / 6.000 = **20 godina** jednostavnog povrata. Ne pribraja se prethodnoj proizvodnoj marži i ne pretpostavlja se automatsko smanjenje plaće stalno zaposlenog.

## 8. Primjer zašto 3× zavarivanje nije 3× proizvodnja

Jednostavan potpuno serijski hipotetski proces, bez paralelizma:

- prije: 8 sati zavarivanja + 16 ostalih = 24;
- poslije: 8/3 + 16 = 56/3 = 18,6667;
- smanjenje ukupnog vremena: 1 − (56/3)/24 = 2/9 = **22,2222%**;
- teorijski faktor izlaza pri istom fondu: 24/(56/3) = 9/7 = **1,2857**, odnosno **28,5714%** više.

Nije model stvarne KONČAR tvornice. U protočnoj/paralelnoj proizvodnji odlučuje stvarno usko grlo; ovaj jednostavni račun služi samo za sprečavanje neispravnog generaliziranja 3×.

## 9. Provjera i audit

**43/43 automatske provjere uspješne.** Decimal račun provjeren je neovisnim Fraction identitetima i susjednim cjelobrojnim pragovima; provjereni su iznosi, scenariji, uhodavanje, NPV do centa, alternativni model i odbijanje nevaljanih ulaza. Cijeli obračun zatim je ponovljen u novom procesu i proizveo identičan JSON rezultat.

Lokalni audit izvršavanja je u `/mnt/data/koncar_o004/`: `check_economics.txt` (Python izvor spremljen kao tekst), `O004_economics_results.txt` i `.json` (svi ulazi/izlazi i pojedinačni testovi), `O004_debug_log.txt`, `O004_debug_log_run1.txt`, `O004_run_stdout.txt`, `O004_run_stderr.txt`, `O004_rerun_stdout.txt`, `O004_rerun_stderr.txt`, `O004_test_summary.txt` i `O004_rerun_check.txt`. To su putanje konkretne sesije, ne trajni javni URL. Ovaj MD čuva sve relevantne poslovne ulaze, rezultate i formule u repozitoriju.

Nema SQL upita, internih sustava, intervjua ili izvedenog proizvodnog testa. Matematička provjera ne potvrđuje tržišnu cijenu, raspoloživost kapaciteta ili potražnju.
