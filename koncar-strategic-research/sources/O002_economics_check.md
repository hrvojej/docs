# O002 — provjera scenarijske ekonomike

**Datum:** 22. 9. 2026. **Status:** izračuni dvaput izvršeni; testovi PASS. [O002 — završni izvještaj](../opportunities/O002_grid_inspection_intelligence_service.md) · [Master](../MASTER_INDEX.md)

Ovo je računski prilog istog O002 zadatka, ne dodatni research task. Cijene i troškovi su eksplicitne autorske pretpostavke, ne KONČAR-ovi podaci, tržišni cjenik ili prognoza. Iznosi su EUR bez PDV-a.

## A. Godišnji paket mobilne inspekcije

Jedinica: nova punogodišnje naplaćena lokacija, dva posjeta, ograničen dogovoreni opseg.

| Varijabla | Vrijednost | Značenje |
|---|---:|---|
| P | 6.000 | Prihod po lokaciji/godini |
| V | 3.500 | Varijabilni trošak po lokaciji/godini |
| F | 45.000 | Godišnji fiksni trošak programa |
| I | 30.000 | Jednokratna početna priprema |
| N | 10 / 30 / 50 | Broj punogodišnjih lokacija u scenarijima |

Provjera V:

`(2 osobe × 8 h × 2 posjeta × 45) + (12 h × 60) + (2 × 200) + (2 × 120) + 300 + 400 = 1.440 + 720 + 400 + 240 + 300 + 400 = 3.500`.

Obračun 32 terenska osobosata obuhvaća pripremu, put i pregled. Putni izdaci od 400 su vozilo/put, ne ponovno isti radni sati. Postojeća/partnerska oprema ima zasebnu godišnju alokaciju 240; veći najam, kupnja ili licence moraju povećati trošak. Sati analize nisu besplatni. F obuhvaća koordinaciju 25.000, zajedničku tehničku/sigurnosnu podršku 12.000 i komercijalnu administraciju 8.000; ne ponavlja iste terenske sate.

Formule:

- prihod = `N × P`;
- varijabilni troškovi = `N × V`;
- godišnji doprinos nakon F = `N × (P − V) − F`;
- rezultat nakon početne pripreme = `N × (P − V) − F − I`.

| N | Prihod | Varijabilni troškovi | Doprinos nakon F | Nakon F i I |
|---:|---:|---:|---:|---:|
| 10 | 60.000 | 35.000 | −20.000 | −50.000 |
| 30 | 180.000 | 105.000 | 30.000 | 0 |
| 50 | 300.000 | 175.000 | 80.000 | 50.000 |

To nije neto dobit ni potpuni cash-flow model: nema poreza, financiranja, rokova naplate ili eventualne dodatne korporativne režije. I je pojednostavljeno u cijelosti odbijen; računovodstvena kapitalizacija nije modelirana. Nije pretpostavljen prihod od sanacije, O001 pretplate ili izbjegnutog velikog kvara.

## B. Pragovi i osjetljivost

Doprinos po lokaciji prije F = `6.000 − 3.500 = 2.500`.

- operativno pokriće = `ceil(45.000 / 2.500) = 18` lokacija;
- prethodnih 17 daje `−2.500`, a 18 daje `0`;
- pokriće s I = `ceil(75.000 / 2.500) = 30` lokacija;
- 29 daje `−2.500` nakon pripreme, a 30 daje `0`;
- pri N=50 minimalna godišnja cijena za pokriće F = `3.500 + 45.000/50 = 4.400`;
- pri N=50 cijena za pokriće F+I = `3.500 + 75.000/50 = 5.000`.

| N | P | V | Godišnji doprinos nakon F |
|---:|---:|---:|---:|
| 50 | 4.500 | 3.500 | 5.000 |
| 50 | 6.000 | 4.500 | 30.000 |
| 50 | 4.500 | 4.500 | −45.000 |

Ako P≤V, veći broj lokacija ne pokriva pozitivan F. Ako novi paket zamjenjuje postojeći posao, računati promjenu prihoda i troška, a ne cijeli P kao dodatak postojećoj prodaji.

## C. Provjera kapaciteta

| Lokacije | Posjeti | Terenski osobosati | Uredska analiza, h |
|---:|---:|---:|---:|
| 10 | 20 | 320 | 120 |
| 30 | 60 | 960 | 360 |
| 50 | 100 | 1.600 | 600 |

Pri 50 lokacija i jednom posjetu dnevno riječ je o približno 100 ekipnih radnih dana s dvije osobe, prije dodatne rezerve za vrijeme i odstupanja. Ne pretpostavlja se neograničena sposobnost širenja pri nepromijenjenom F.

## D. Zasebna računica docka — jednaka svrha misije

Svi inputi su scenarijski. Uspoređuje se trošak zamjenjivog prikupljanja podataka; jednaka stručna analiza ostaje izvan obje strane. Ovaj model nije dodan u prihod godišnjeg paketa.

- mobilno: `1.200 × m`;
- dock: `18.000 + 150 × m`;
- m = broj stvarno potrebnih i izvedivih misija godišnje na istoj lokaciji.

| m | Mobilno | Dock | Ušteda docka nasuprot mobilnom |
|---:|---:|---:|---:|
| 2 | 2.400 | 18.300 | −15.900 |
| 12 | 14.400 | 19.800 | −5.400 |
| 24 | 28.800 | 21.600 | 7.200 |

Prijelom = `18.000/(1.200−150) = 17,142857...`. Na 17 misija mobilno je još jeftinije; na 18 dock postaje jeftiniji. Ako je razlika troška po misiji nula ili negativna, pozitivan dock fiksni trošak ne vraća se ovom logikom.

Stres-scenarij: mobilno 700, dock 30.000 fiksno i 200 po misiji. Na 60 misija obje opcije koštaju 42.000; dock je strogo jeftiniji tek od 61. Potrebna učestalost nije industrijski standard. Snimanje ne smije zamijeniti inspekciju koju funkcionalno ne može obaviti, a nepotrebni letovi nisu vrijednost.

## E. Izvršena kontrola

Python izračun s Decimal za pragove i zasebnim provjerama identiteta ponovno je izvršen nakon dodavanja stres-scenarija. Provjereni su: zbroj komponenti; oba načina računa doprinosa; sve tablice; cjelobrojni prag i red neposredno ispod njega; minimalne cijene; kapacitet; dock na 17/18 i 60/61 misija. Svi testovi prošli su. Tehnički log je odvojen od rezultata izračuna; ovaj dokument čuva ulaze, pune rezultate i zaključke provjera.

Provjera aritmetike ne potvrđuje tržišnu cijenu, potreban broj poslova, dostupnost osoblja ili profitabilnost stvarnog ugovora. Ti nedostupni inputi ostaju označene pretpostavke, bez dodatnog zahtjeva korisniku.
