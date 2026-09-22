---
opportunity_id: O004
title: Adaptivno zavarivanje i digitalna kvaliteta — interna profitabilnost
as_of: 2026-09-22
status: completed-public-research
recommendation: targeted-existing-cell-upgrade-before-new-robot-or-platform
basis: public-primary-sources-and-explicit-scenarios
actual_profit_verified: false
pilot_executed: false
---

# O004 — Završna procjena: automatizacija zavarivanja i kontrole kvalitete

[Glavni indeks](../MASTER_INDEX.md) · [Šest zadataka](../validation/TASK_BOARD.md) · [Provjerena računica](../sources/O004_economics_check.md) · [Raniji B004](../benchmarks/B004_adaptive_welding_automated_ndt_smart_fabrication_2026-09-21.md)

## 1. Zaključak

**DA ciljanoj modernizaciji postojećih proizvodnih procesa i prikladne robotske ćelije, prvenstveno kroz offline programiranje, pozicioniranje, pronalaženje spoja i digitalnu sljedivost kvalitete. NE početnom razvoju vlastitog robota, općeg AI sustava za zavarivanje ili velikoj automatizaciji cijele tvornice.**

O004 je prvenstveno interna poslovna prilika: više prihvaćenih i isporučenih proizvoda iz ograničenog kapaciteta, odnosno manje stvarno plaćenih dorada i vanjskih usluga. Nije pretpostavljeni SaaS prihod ni nova robotska divizija.

Najprirodnije proizvodne domene su Metalne konstrukcije (KMK) i Transformatorski kotlovi (KTK). Javni izvori potvrđuju relevantne procese i ranije ulaganje, ali ne današnji raspored svih strojeva, iskorištenost, njihovu kompatibilnost ili slobodne zaposlenike. Ako predložene funkcije već postoje, preporuka je bolje koristiti postojeće, a ne ponovno nabavljati ili razvijati isto.

**O004 je dovršen kao javno istraživanje.** Preporučeni početni zahvat u nastavku nije izveden pilot ni dodatni research zadatak. Ne čeka se interne podatke korisnika. Brojke su transparentni scenariji, ne potvrđeno ulaganje ili marža KONČARA.

## 2. Što već postoji u KONČAR-u

**Povijesni dokaz KMK-a [S01].** Objava od 15. 2. 2022. navodi oko 173.000 EUR za prvu CLOOS robotsku stanicu i oko 146.000 EUR za obnovu automatiziranog portala. Za određeni ponavljajući sklop opisuje tri komada u vremenu ranije potrebnom za jedan, uz NDT-provjerenu kvalitetu. To nije današnja ponuda, dokaz 3× učinka cijelog pogona ili potvrda sadašnje lokacije/iskorištenosti te stanice.

**KTK [S02–S03].** Javno je opisana izrada prema nacrtima i 3D modelima, zavarivanje, kontrola nepropusnosti, kupcem određene NDT metode i probna montaža. Nova tvornica otvorena je 23. 1. 2026.; KTK je društvo u kojem KONČAR ima 60%, Siemens Energy 40%. To je proizvodno okruženje za ciljanu primjenu, a ne dokaz da mu automatizacija nedostaje. Ne poistovjećivati KTK s KPT-om niti staru KMK opremu automatski pripisati KTK-u.

**Kvaliteta [S04].** KMK navodi kvalificirane postupke, zavarivače, koordinatore, NDT osoblje i sljedivost materijala. Pregledana je javna stranica, ne pojedini važeći certifikat sa svim opsezima. Postojeći sustav kvalitete je osnova koju automatizacija treba podržati, ne zaobići.

## 3. Što se stvarno komercijalizira izvan Grupe

| Primarni dokaz | Što potvrđuje | Granica zaključka |
|---|---|---|
| Miller / IFH, objavljeno 26. 7. 2026. [S05] | Na približno 25 modela većih spremnika prijavljen je 25–40% veći izlaz nakon primjene robotskih ćelija i offline programiranja. Vrijeme programiranja uz zaustavljenu ćeliju s oko 15 h pada na 2–3 h dorade | Izjave korisnika objavljene kod dobavljača; nije garantirani KONČAR ROI. Offline programiranje i dalje troši inženjerski rad |
| Verbotics / TRT, projekt od 2019., studija 2. 8. 2022. [S06] | CAD programiranje robota i pronalaženje spoja koriste se u malim serijama i pojedinačnim proizvodima; primjer 4 h programiranja za 36 h robotskog rada | Omjer je 9:1, ne devetostruka produktivnost. Noćni oporavak bez nadzora u tekstu je idući izazov, ne dovršena sposobnost |
| CLOOS RoboPlan [S07] | Komercijalno offline programiranje na 3D modelima, dok robot proizvodi | Nije dokaz kompatibilnosti ili instalacije na određenoj KONČAR ćeliji |
| CLOOS C-Gate [S08] | Proizvodni podaci, upravljanje programima i njihova sljedivost, kvalitetni zapisi i održavanje već su komercijalne funkcije | Nema razloga pretpostaviti da sve to treba vlastito razviti. Predictive maintenance na pregledanoj stranici označen je kao buduća funkcija |
| SERVO-ROBOT ARC-SCAN [S09] | Dostupno je mjerenje geometrije zavara i geometrijskih nepravilnosti | Površinska geometrija nije dokaz unutarnjeg stanja cijelog zavara |
| Eddyfi PAUT/TOFD [S10] | Postoje mehanizirani ultrazvučni postupci s digitalnim zapisima za prikladne velike zavare | Primjer vjetro-stupova/monopilota nije automatska kvalifikacija za svaki transformatorski kotao; zahtjevi, geometrija i metoda određuju primjenjivost |
| Novarc NovAI Autonomy [S11] | Dobavljač nudi machine-vision/AI prilagodbu tijekom zavarivanja i pretplatničke nadogradnje | Produktni navod, ne neovisno izmjeren učinak na KONČAR proizvodima. Ne pretpostavljati da pokriva sve materijale i spojeve |

Zaključak: tržište dobavljača je dovoljno razvijeno za kupnju i integraciju. Dodatna vrijednost KONČARA bila bi u pravilnom izboru proizvoda, vlastitom procesnom znanju i povezanosti s kvalitetom, ne u izradi univerzalnog robot-programatora.

## 4. Što konkretno napraviti

**Prvi zahvat: jedna prikladna postojeća ćelija ili proces i 2–3 srodne obitelji sklopova, ne cijeli kotao ili cijela tvornica.** Sadržaj zahvata ovisi o stvarnom ograničenju; ne kupovati sve stavke u paketu samo zato što postoje.

| Uočeni problem u predloženoj primjeni | Smislen izbor |
|---|---|
| Robot dugo stoji dok se priprema novi program | Offline CAD programiranje i provjereni postprocesor |
| Česte varijacije položaja spoja zahtijevaju ručno popravljanje putanje | Senzorsko pronalaženje/praćenje spoja i bolja priprema dijelova |
| Previše vremena odlazi na okretanje, stezanje i pristup | Prikladno pozicioniranje/naprave; to može biti važnije od AI-a |
| Nalazi zavara teško se povezuju s nacrtom i izvedenim programom | Stabilni ID zavara, verzije i poveznica s kontrolnim zapisom |
| Kontrola dimenzija ili NDT je stvarno usko grlo | Ciljano mjerenje/skeniranje odgovarajućom metodom, ne ubrzavanje nepotrebnog procesa prije njega |

Predloženi interni nositelj je proizvodnja zajedno s tehnologijom zavarivanja i kvalitetom. Dobavljač ćelije/integrator vodi hardversko i upravljačko povezivanje. Digital/NEOS mogu sudjelovati u analitici i povezivanju podataka, ali to je prijedlog uloge, ne potvrđena interna implementacija ili nužan zaseban tim.

D&ST, željeznička i generatorska proizvodnja ostaju moguća proširenja nakon dokazane primjene; nisu automatski korisnici istog programa, naprave ili kvalifikacije.

## 5. Zašto 3× brzina nije 3× kapacitet tvornice

Ilustracija, **ne mjerenje KONČARA**: u jednostavnom serijskom procesu sklop troši 8 sati na zavarivanje i 16 sati na ostalo. Ako zavarivanje postane tri puta brže, ukupno vrijeme pada s 24 na 18,67 sati. To je 22,2% kraće vrijeme, odnosno teorijskih 28,6% više izlaza pri istom vremenskom fondu — ne 200% više.

Stvarni pogon ima paralelne procese, serije i različita ograničenja pa ni tih 28,6% nije predviđanje. Ako nakon zavarivanja čekaju obrada, kontrola, bojanje ili kupčev prihvat, dodatni rad robota možda ne povećava isporuku. Mjeriti prihvaćeni izlaz i ukupni ciklus, ne samo vrijeme aktivnog luka.

Smanjenje dorade također nije automatski ušteda plaće: stalno zaposleni ostaje trošak ako se njegov kapacitet ne iskoristi ili se ne izbjegne prekovremeni/vanjski rad. Isti oslobođeni sat ne može istodobno biti puna ušteda plaće i puna vrijednost dodatne proizvodnje.

## 6. Scenarij ekonomike ciljane nadogradnje

**Sve vrijednosti su pretpostavke u EUR bez PDV-a.** Nije pronađena funkcionalno usporediva aktualna javna ponuda koja uključuje konfiguraciju, integraciju, sigurnost, kvalifikaciju i isporuku za KONČAR. Povijesnih 173.000 EUR iz 2022. nije cjenik za 2026. niti izvor donjeg scenarija.

Modelira se ograničena nadogradnja postojeće kompatibilne ćelije, ne nova kompletna linija ili automatizacija kotla teškog 100 tona.

| Ulaz | Pretpostavka / značenje |
|---|---|
| I — početni izdatak | 120.000; ilustrativno softver/postprocesor 25.000, senzori/naprave 35.000, integracija/obuka/kvalifikacija 40.000, početni prekid/rezerva 20.000 |
| F — godišnji dodatni trošak | 20.000; licence, servis i dodatna programska podrška. Nije sav postojeći trošak pogona |
| H — neto oslobođeni sati ograničavajuće ćelije | 300 / 800 / 1.400 godišnje; nakon dodatnog vremena traženja, stezanja, popravaka i ostalih efekata zahvata |
| u — realizacija kapaciteta | 75% sati pretvori se u prihvaćene, prodane i isporučene proizvode; ostatak nema pripisanu financijsku korist |
| c — doprinos po realiziranom satu | 150 EUR nakon svih dodatnih troškova novih proizvoda, prije zasebnog F; nije satnica radnika ni prodajna cijena |

`Godišnji dodatni operativni doprinos B = H × u × c − F`

`Jednostavni povrat pri punom godišnjem učinku = I / B`, samo ako je B pozitivan.

| Neto oslobođeni sati H | Realizirani sati | Dodatni doprinos proizvoda prije F | Godišnji rezultat B | Jednostavni povrat pri punom učinku |
|---:|---:|---:|---:|---:|
| 300 | 225 | 33.750 | **13.750** | **8,73 godine** |
| 800 | 600 | 90.000 | **70.000** | **1,71 godina** |
| 1.400 | 1.050 | 157.500 | **137.500** | **0,87 godina** |

Za razumijevanje srednjeg reda: 600 stvarno iskorištenih sati može u zasebnoj ilustraciji značiti 60 dodatnih sklopova po 10 sati, svaki s doprinosom 1.500 EUR. Daje istih 90.000, a ne još jedan prihod koji se dodaje izračunu.

Broj sati nije izveden iz stare 3× tvrdnje. Za orijentaciju, 800 oslobođenih sati odgovara 20% hipotetskog godišnjeg fonda ćelije od 4.000 sati; 1.400 odgovara 35%. To su zahtjevni ciljevi, ne utvrđena rezerva. Ako ćelija toliko vremena ne gubi na rješive uzroke, odgovarajući scenarij ne vrijedi.

**Uhodavanje:** ako se u prvoj godini ostvari samo 50% srednjeg bruto učinka, uz puni F, prva godina donosi 25.000 prije početnih 120.000. Potom po 70.000 godišnje daje pojednostavljeni povrat oko **2,36 godina**, ne 1,71. Petogodišnji neto sadašnji učinak s pretpostavljenim diskontom 10%, bez ostatka, jest oko **104.446 EUR**. To je scenarijski neto sadašnji iznos, ne KONČAR-ov odobreni NPV.

Usporedba je inkrementalna u odnosu na nastavak postojećeg rada. Nisu modelirani porez, financiranje, promjena radnog kapitala i nepoznata korporativna režija. Doprinos nije neto računovodstvena dobit; 120.000 je početni izdatak, ne ponovno godišnji trošak. Dodatno širenje drugih strojeva, ako je potrebno za isporuku, treba platiti i može poništiti model. Nema pretpostavljenog vanjskog ARR-a, dodatnih plaćenih AI licenci kupcima ili brojanja transfera između društava kao nove konsolidirane prodaje.

## 7. Kada se ulaganje ne isplati

Uz H = 800:

| Promjena jedne pretpostavke | B godišnje | Posljedica |
|---|---:|---|
| Samo 25% realizacije umjesto 75% | 10.000 | Jednostavni povrat 12 godina: ne preporučuje se taj izdatak |
| Doprinos 75 umjesto 150 EUR/h | 25.000 | Povrat 4,8 godina prije uhodavanja; bitno slabija prilika |
| Nema dodatne prodaje/isporuke, u = 0 | −20.000 | Kapacitet sam po sebi ne plaća investiciju |
| F poraste na 35.000 | 55.000 | Učinak je manji iako proizvodni sati ostaju isti |
| I naraste na 200.000 | 70.000 | Jednostavni povrat 2,86 godina prije uhodavanja |

U baznim pretpostavkama godišnji operativni trošak pokriva se od 178 neto oslobođenih sati. Za ilustrativni cilj povrata do dvije godine uz puni učinak treba barem **712 sati godišnje**. Taj cilj je kriterij ovog scenarija, ne propisani KONČAR kriterij.

Alternativno, ako nema dodatne prodaje, investicija se može opravdati stvarnim smanjenjem vanjskih dorada, prekovremenih ili materijalnog škarta. Ali ako to donosi samo 26.000 godišnje, nakon 20.000 održavanja ostaje 6.000 i povrat 120.000 traje 20 godina. Taj odvojeni savings-only slučaj nije pribrojen modelu dodatne proizvodnje.

## 8. Kvaliteta i AI: ne pomiješati tri različite stvari

**Senzorsko vođenje** otkriva položaj spoja i pomaže robotu slijediti stvarnu geometriju. **Optička kontrola** mjeri površinu i oblik zavara. **Volumetrijski NDT** ispituje unutarnje indikacije odgovarajućom metodom. To nisu međusobno zamjenjivi dokazi. ARC-SCAN i Eddyfi pokazuju da su te kategorije već zasebni komercijalni proizvodi. [S09–S10]

Prvi AI dodatak može biti rangiranje odstupanja, povezivanje procesa i dorada te priprema dokumentacije. Ne treba vlastiti univerzalni model, a alarm o odstupanju struje nije sam po sebi dokaz lošeg zavara. Novarcova ponuda pokazuje smjer zatvorene adaptivne petlje, ali javna marketinška tvrdnja nije dozvola za proizvoljno mijenjanje kvalificiranih parametara na KONČAR proizvodu. [S11]

Automatizacija treba ostati unutar odobrenih postupaka i sigurnosnih funkcija. Prvi primjerni dio i primjenjiva ispitivanja prihvaća odgovorna kvaliteta/kupac; ne uklanjati obvezni NDT zato što kamera izgleda uvjerljivo. Ne tvrdi se da su aktualne KONČAR certifikacije ili sve norme pojedinačno provjerene za novu konfiguraciju. Millerov slučaj također zadržava stručnjake, ispitivanja i kupčev prihvat prvog proizvoda. [S04–S05]

## 9. Podaci, softver i prava — minimalni potrebni sloj

Predloženi tok, ne opis neviđene interne arhitekture:

`nacrt i revizija → ID sklopa/zavara → odobreni postupak i program robota → izvedba i procesni zapis → mjerni/NDT nalaz → dorada i ponovna kontrola → prihvat`

Sačuvati stvarne izvozne formate i jedinice, identitet dijela/zavara, verziju programa, vrijeme/vremensku zonu, mjernu kalibraciju i potpis odgovorne osobe. Neke naprave zahtijevaju transformaciju koordinata između CAD-a, fixturea, robota i skenera; pogrešno poravnanje nije AI problem. Nedostajući zapis ne znači dobar zavar.

Ne pretpostavljati postojeći REST API, MQTT, Kafka, određeni MES/ERP ili cloud. Početno povezivanje može biti ograničeni, dogovoreni izvoz i izvještaj. C-Gate već nudi dio mrežnih/procesnih funkcija, ali konkretni konektori, licence i generacija kontrolera moraju odgovarati izabranoj isporuci. [S07–S08]

Kupčevi nacrti, programsko znanje dobavljača, JV podaci i modeli ne postaju slobodno raspoloživi cijeloj Grupi. U predloženoj implementaciji zadržati izvoz/sljedivost te ugovoriti dopuštene uporabe; ne slati nacrte vanjskom AI servisu bez odobrenja. Nijedan privatni ugovor ili stvarni proizvodni uzorak nije analiziran u ovom researchu.

## 10. Praktični početak i vanjska komercijalizacija

Poslovna preporuka je plaćena i ograničena integratorska primjena na prikladnoj postojećoj ćeliji i nekoliko obitelji dijelova. Koristiti postojeći dobavljačev paket kad odgovara. Ugovoriti rezultat kroz ukupni ciklus, prihvat iz prve, dorade i raspoloživi kapacitet, ne marketinški broj o brzini luka. Scenarijskih 120.000 nije preporuka automatski potrošiti taj iznos; pri samo 300 sati i cilju dvogodišnjeg povrata gornji početni izdatak bio bi 27.500, a ne 120.000.

Ako modernizacija nije kompatibilna ili nema dovoljno prikladnog posla, zadržati ručni/automatizirani postojeći proces, poboljšati pozicioniranje ili ciljano rješavati stvarni NDT/obradni bottleneck. Zamjenska ćelija je zasebna proizvodna odluka, ne unaprijed odabrani ishod.

**Vanjska prodaja softvera ili robotskih rješenja nije prvi cilj.** Nakon interne ponovljivosti moguća je domenska nadogradnja, primjerice sljedivost zavara i kvalitetni dosje za slične pogone, ali nema ovdje javnog dokaza kupčeve spremnosti da to kupuje od KONČARA. Ne dodajem prihod koji ne postoji. Licence dobavljača i kupčeva prava također mogu ograničiti reprodaju.

**Završna ocjena:** ciljano ulaganje može biti vrlo razumno jer koristi stvarne industrijske kompetencije i postojeću opremu. Najbolji smjer nije više robota pod svaku cijenu, nego više prodajivog i kvalitetnog izlaza po ograničavajućem satu. Javna podloga opravdava ograničeni manufacturing retrofit, ne veliki novi AI/robotics poslovni program. Stvarna dobit ostaje nepoznata; research je zaključen scenarijima i jasnom preporukom.

## Izvori

Provjereno **22. 9. 2026.** Primarni izvori; produktne izjave nisu neovisni testovi. Svi poslovni izračuni izvan izričito povijesnih javnih iznosa autorski su scenariji.

| ID | Izvor | Lokator / ograničenje |
|---|---|---|
| S01 | [KONČAR KMK: Investments in welding technology](https://koncar.hr/en/kmk/news/investments-welding-technology) | 15. 2. 2022.; dvije investicije i konkretni sklop; nije aktualna cijena ni iskorištenost |
| S02 | [KONČAR KTK: Transformer tanks](https://www.koncar.hr/en/ktk/transformer-tanks) | Proces, nacrti/3D, NDT i probna montaža; nije as-built linije |
| S03 | [Otvaranje KTK tvornice](https://www.koncar.hr/en/news/croatia-gains-new-production-center-for-global-energy-transformer-market) | 23. 1. 2026.; KTK 60/40 i otvorena tvornica, ne aktualni broj isporučenih kotlova |
| S04 | [KMK: Quality and certifications](https://koncar.hr/en/kmk/quality-and-certifications) | Kvalifikacije, koordinatori, kontrola/sljedivost; pojedini PDF certifikati nisu analizirani |
| S05 | [Miller / IFH: throughput 25–40%](https://www.millerwelds.com/en-us/case-studies/how-ifh-group-increased-throughput-with-robotic-welding-automation) | Objavljeno 26. 7. 2026.; odjeljci o offline programiranju, većim spremnicima i prihvatu. Jedna grafička tablica piše 24–40; naslov i ponovljeni tekst 25–40. Ne koristiti kao precizno neovisno mjerenje |
| S06 | [Verbotics / TRT](https://verbotics.com/news/2022-08-02-trt-case-study/) | Projekt 2019., objava 2022.; 4/36 h i budući noćni oporavak; povijesni korisnički slučaj |
| S07 | [CLOOS QIROX RoboPlan](https://cloos-group.com/en/digital-solutions/qirox-roboplan/) | Aktualna produktna stranica; stari cloos.de URL preusmjerava na naslovnicu, zato provjeren novi izravni link |
| S08 | [CLOOS C-Gate Ultimate](https://cloos-group.com/en/digital-solutions/c-gate/ultimate-modul/) | Production, Programme management, Quality i Maintenance; predictive maintenance označen future |
| S09 | [SERVO-ROBOT ARC-SCAN](https://servo-robot.com/arc-weld-inspection/) | Geometrijska kontrola zavara; nije volumetrijski NDT |
| S10 | [Eddyfi: mechanized PAUT/TOFD](https://www.eddyfi.com/en/appnote/mechanized-paut-and-tofd-inspection-techniques-for-monopile-and-wind-tower-welds) | Aplikacijski tekst za velike zavare; kvalifikacija i priprema nisu sadržane u čistoj brzini skeniranja |
| S11 | [Novarc NovAI Autonomy](https://www.novarctech.com/products/novai/novai-autonomy/) | Adaptivno vođenje, video/podaci i subscription; dobavljačeva funkcijska ponuda, ne izmjeren KONČAR učinak |

Prethodni B004 ostaje povijesna podloga. Ovaj izvještaj ima prednost u vremenskoj interpretaciji, ekonomici i odluci. Preporuka ne ovisi o nedostupnom internom dokumentu niti uvodi dodatne zadatke izvan šest prilika.
