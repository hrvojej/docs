---
research_id: R005
title: Program dokazivanja i odbacivanja O001–O006
as_of: 2026-09-22
status: execution-plan-v1
scope: validation-program-not-investment-approval
---

# R005 — Program validacije O001–O006

[Glavni indeks](../MASTER_INDEX.md) · [Svi zadaci i statusi](../validation/TASK_BOARD.md)

## Cilj i granica

Za svaku tezu utvrditi postoji li dodatna, naplativa ili interno mjerljiva vrijednost povrh onoga što KONČAR i konkurencija već rade. Rezultat može biti nastavak, sužavanje, proširenje postojećeg proizvoda, odgoda zbog nedostupnih dokaza ili odbacivanje. Broj izrađenih dokumenata nije dokaz profitabilnosti.

Ulazi su [R004](R004_first_wave_cross_opportunity_synthesis_2026-09-21.md), B001–B006 i O001–O006. To su početne hipoteze, ne neovisno verificirane interne arhitekture ni investicijski elaborati. Svaka presudna tvrdnja ponovno se provjerava u primarnom izvoru. Ovaj plan je metodološki prijedlog; pragovi u njemu nisu industrijski standardi niti već prihvaćeni KONČAR kriteriji.

## 32 zadatka, bez prikrivenog zaključivanja

Svaka prilika ima pet odvojenih zadataka A–E. Dodatna dva portfeljna zadatka su X01 i X02. Ukupno: 6 × 5 + 2 = 32.

| Faza | Predmet dokazivanja | Minimalni izlaz | Što ne dokazuje |
|---|---|---|---|
| A | Javno provjerljiv postojeći proizvod, arhitektura i konkurentska ponuda | Registar tvrdnji i izvora, granica postojećeg proizvoda, mapa nepoznanica, test originalnosti teze | Ne dokazuje aktualnu internu implementaciju, cijenu ni slobodne kapacitete tima |
| B | Stvarna interna arhitektura, isporuka, prava i postojeća ekonomika | Verzije, dijagram toka podataka, uzorci poruka, prava po funkciji/tržištu, servisni proces, komercijalni baseline | Organigram ili prezentacija sami nisu dokaz operativne spremnosti |
| C | Kupac, problem, konkurent i spremnost platiti | Zapis dokaza kupaca, usporedivih ponuda/tendera i izgubljenih poslova; raspon testirane cijene | Vendor case study nije razgovor s našim kupcem; iskaz interesa nije narudžba |
| D | Inkrementalna unit economics i alternativni trošak | Provjerljiv model ulaza, troškova, doprinosa, novčanog toka, osjetljivosti i negativnog scenarija | Ukupan promet društva nije prihod proizvoda; simulacija nije stvarna marža |
| E | Pilot i odluka | E-design: unaprijed dogovoreni protokol. E-result: stvarni rezultati, odstupanja i odluka | Napisan plan pilota nije izveden pilot; mali pilot ne dokazuje smanjenje rijetkih katastrofalnih kvarova |

Detaljna pitanja, ovisnosti, uvjeti zaustavljanja i odredišta svih izlaza nalaze se u TASK_BOARD-u. Nisu kreirana 32 GitHub issuea niti automatizirana izvršavanja; ovo je dokumentirani red rada za zasebne istraživačke sesije.

## Ovisnosti i red rada

A zadaci mogu se raditi neovisno za svih šest prilika. B i C slijede nakon definiranja granice proizvoda i mogu teći paralelno. Javne dijelove C možemo istraživati i dok čekamo B. D se može pripremiti simbolički, ali ne zaključiti bez izmjerenih/ponuđenih ulaza. E-design slijedi nakon preliminarne ekonomike i prava; E-result tek nakon stvarnog izvođenja i prihvata rezultata.

Prvi zadatak je O001-A: provjera postojećeg TMS/diagnostika/servis sklopa. Rezultat je [R006](R006_O001_existing_stack_offer_audit_2026-09-22.md). Nakon toga prioritet ima zatvaranje O001-B; dok interni dokazi nisu dostupni, mogu se odraditi O001-C desk-research i O002-A–O006-A. Nema razloga čekati jedan interni podatak da bi se zaustavio cijeli program.

X01 radi se kada su barem dvije relevantne B arhitekture poznate. X02 objedinjuje pojedinačne odluke, uključujući HOLD i REJECT, i uspoređuje ih s opcijom ne ulagati. O004 se uspoređuje kroz tvornički doprinos i kapacitet, ne kroz SaaS ARR.

## Statusi

- READY: zadatak je definiran i nema neispunjenu prethodnu obvezu za javni dio.
- WAITING_EVIDENCE: potreban je određeni interni dokument, pristup ili suglasnost; javni rad smije se nastaviti.
- DEPENDENT: nedostaje rezultat prethodne faze.
- COMPLETE_DESK: završen je deklarirani javni pregled, s popisom ograničenja.
- DESIGNED: pilot je projektiran, ali nije izveden.
- VALIDATED: zaključak podupiru stvarni, provjerljivi dokazi odgovarajuće faze.
- REJECTED / REFRAMED: izvorna teza je odbačena / promijenjena; razlog i posljedice ostaju zabilježeni.

COMPLETE_DESK nije isto što i VALIDATED. Nepoznato se označava U; ne pretvara se automatski u G2 ili G3 gap. Odsutnost javnog dokaza nije dokaz da funkcija, tim, SLA ili prihod ne postoji.

## Obavezni ugovor za svaki istraživački task

Artefakt mora navesti ID zadatka, input artefakte/verzije, datum, odluku koju treba podržati, tvrdnje za provjeru, primarne izvore s točnim lokatorom, potvrđeno, osporeno, nepoznato, podatke koji nedostaju, odredište rezultata i sljedeći korak. Jasno razlikovati planirano, ugovoreno, isporučeno, u pogonu i obnovljenu komercijalnu pretplatu.

Izvori dobivaju stabilni ID. Broj iz izvještaja mora imati godinu i definiciju populacije. Izvedeni broj mora imati formulu. Kontradikcije se ne prepisuju prešutno: navesti staru tvrdnju, novi dokaz i što se mijenja u O###. Više web-stranica koje prenose istu izjavu nisu više neovisnih potvrda.

## B: što znači provjeriti internu arhitekturu

Potrebni su stvarna verzija proizvoda i jedan reprezentativni end-to-end tok, ne idealizirani dijagram budućeg sustava.

Za svaki prijelaz podataka zabilježiti izvor, odredište, transport, autentikaciju, payload i kodiranje, identifikatore, jedinice, vremensku zonu, izvorno i prijemno vrijeme, kvalitetu mjerenja, NULL/zero semantiku, verzije, kalibraciju, redoslijed, ponavljanje, deduplikaciju, gubitke, retention i pristup. Za signal obuhvatiti frekvenciju uzorkovanja, filtre, agregiranje, okidač i vezu sirovog signala s izvedenim rezultatom.

Napraviti provjerljivi uzorak: ulaz → dekodiranje → normalizacija → pohrana → analitika → alarm/preporuka → ljudska potvrda → radni nalog. Sačuvati reprezentativne ulaze i očekivane izlaze. Testirati prekid veze, ponovljenu poruku, promjenu sata, promjenu senzora, neispravnu jedinicu, nedostajuću vrijednost, promjenu modela i povlačenje prava pristupa.

Prava se analiziraju zasebno za hardver, firmware, algoritam, podatke kupca, povijesne podatke, dokumentaciju, izvedene značajke/model, treniranje i međunarodnu prodaju. Kupnja uređaja ili pripadnost istoj Grupi ne zamjenjuje ta prava. Potrebne su stvarne licence/ugovori i ovlaštena provjera; nije dovoljan opći pravni naziv društva.

## C: dokaz tržišne potražnje

Krenuti od segmenta s konkretnim poslom i budžetom, ne od 'AI tržišta'. Usporediti najmanje: nastavak sadašnjeg rada, proširenje postojećeg proizvoda, kupnju partnerova rješenja i razvoj vlastitog dodatka.

Predložena početna istraživačka kvota je 6–10 dokumentiranih razgovora kroz najmanje tri organizacije u odabranom segmentu, uključujući nezainteresirane kupce ili izgubljene poslove. To nije statistički dokaz veličine tržišta. Potreban je iskaz budžeta, sadašnjeg troška, postupka nabave, integracijskih uvjeta i razloga kupnje/odbijanja. Za komercijalni pilot tražiti barem jednog vlasnika budžeta i pisani okvir opsega/cijene; besplatan PoC voditi odvojeno.

Nisu kontaktirani kupci u ovoj sesiji. Predložene uloge nisu imenovanja niti preuzete obveze KONČAR zaposlenika.

## D: model ekonomike i test rušenja

Za vanjske usluge odvojiti jednokratni prihod od ponavljajućeg. Izračunati doprinos po kupcu i imovini nakon integracije, hardvera/rente, povezivosti, platforme, ekspertnih sati, korisničke podrške, terena, partnerovih licenci i ugovorenog rizika. Troškove prikazati jednom: izbjegavati dvostruko brojanje amortizacije i istog CAPEX novčanog izdatka u istoj metrici.

Radne formule, ne tvrdnje o KONČAR financijama:

- godišnji doprinos kupca = ponavljajući prihod − izravni godišnji troškovi isporuke;
- inkrementalni rezultat programa = doprinos novih/obnovljenih ugovora − dodatni fiksni troškovi − izgubljeni doprinos kanibaliziranih poslova;
- točka pokrića standardiziranih kupaca = dodatni godišnji fiksni troškovi / pozitivan doprinos po kupcu;
- prag cijene za ciljnu maržu g = izravni trošak / (1 − g), uz odvojeno pokriće fiksnog razvoja;
- klijentska vrijednost = provjerljive uštede + procijenjena promjena očekivanog gubitka − ukupni trošak rješenja. Procjena očekivanog gubitka mora imati raspon i dokaz, ne retoričko 'izbjegli smo katastrofu'.

Za O004: inkrementalni doprinos = dodatna prodajiva i isporučiva količina × doprinos po jedinici + stvarno izbjegnuti trošak dorade/prekovremenih − dodatni operativni troškovi. Oslobođeni sati bez prodajive dodatne količine nisu automatski dodatni prihod. Ne zbrajati istu uštedu kroz radne sate i povećanu proizvodnju dvaput.

Obavezno stresirati cijenu, obujam, iskorištenost, vrijeme integracije, ekspertne sate, lažne alarme, partnerove naknade, gubitak kupca, rok naplate i odgovornost. Svi izmišljeni ulazi ostaju označeni SCENARIO, nikad BASELINE. Model bez privatnih podataka može izračunati break-even pragove, ne konačnu profitabilnost.

## E: pilot koji može i srušiti tezu

Prije izvođenja zamrznuti postojeći baseline, ciljne metrike, referentni skup, trajanje, način usporedbe, tko potvrđuje nalaz, način mjerenja troška i uvjete zaustavljanja. Pilot počinje read-only gdje god je to primjereno; zaštitno upravljanje i sigurnosne funkcije nisu dio generičkog AI pokusa.

Kod AI/diagnostike odvojiti rezultate na razini impulsa, alarma i stvarnog kvara. Koristiti odvojene vremenske intervale/imovinu za evaluaciju, uključiti negativne primjere i promjene uvjeta. Mjeriti preciznost, odziv, lažne alarme po asset-mjesecu, vrijeme ekspertne obrade, latenciju i pokrivenost. Nula kvarova u malom pilotu nije dokaz da je model spriječio kvarove.

E-result je dovršen tek s dokazima stvarnog izvođenja. Odluke: GO na ograničenom opsegu, REFRAME, HOLD uz imenovani nedostajući dokaz ili REJECT. Predloženi CAPEX i zapošljavanje ne odobravaju se samo na osnovi javne studije.

## Informacijska sigurnost i trajno spremanje

GitHub repozitorij hrvojej/docs je pri pokretanju ove faze potvrđen kao public. Tu idu javni izvori, metodologija i odobreni sažeci. Interni dokumenti, cijene, uzorci proizvodnih podataka i dijagrami sigurnosnih zona trebaju odobren privatni prostor. Javni registar smije sadržavati samo nesenzitivni ID zahtjeva i status, bez povjerljivog priloga.

Svaki završeni task upisuje se u TASK_BOARD i MASTER_INDEX; ažuriraju se relevantni O###, CURRENT_CONTEXT i sažetak sesije. Planned lokacije u boardu nisu poveznice na nepostojeće datoteke. Arhitekturne i ekonomske pretpostavke ažuriraju se, a stari zaključci ostaju u Git povijesti.

## Stanje ove sesije

Program je definiran. O001-A završen je kao COMPLETE_DESK kroz R006. O001-B čeka ovlaštene interne dokaze, O001-C je spreman za javni komercijalni pregled. Nijedna prilika nije dobila E5 ni odobrenje ulaganja.
