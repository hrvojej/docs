# S014 — dovršen O005: vlakovi, tramvaji, baterije i autonomija

**23. 9. 2026. Status: 5/6 dovršeno.** [O005](../opportunities/O005_rail_fleet_battery_intelligence_service.md) · [Računica](../sources/O005_economics_check.md) · [Master](../MASTER_INDEX.md)

Korisnik je izričito proširio O005 na tramvaje koji sami voze. Proširenje je obrađeno u istom zadatku; nema sedmog taska ni čekanja internih dokumenata.

## Glavni novi nalaz

KONČAR već ima vlastiti razvojni trag tramvajske percepcije/AI-a: Institut/FER SafeTram 2016.–2020.; prototip na TMK2200 testiran 24. 9. 2019. za senzore, otkrivanje vozila/pješaka i upozorenja. To nije potvrda današnje serijske homologacije, prodaje, dostupnog tima ili vožnje bez čovjeka. O005 ima izvore S03–S05.

## Preporuka

Digitalno održavanje vlakova i tramvaja + sigurnosni dodatak/ADAS predstavljaju najbliže naplative proizvode. SafeTram ili partnerske funkcije mogu biti osnova vlastitog OEM proizvoda. Autonomni depo je razumna prva prava autonomna primjena uz operatora/konkretan budžet. Puna autonomija u otvorenom gradskom prometu ostaje strateški razvojni program, ne obećanje brzog ukidanja vozača.

## Razlike koje treba sačuvati

- Baterijska/vožnja bez kontaktnog voda nije autonomna vožnja.
- ADAS/aktivno kočenje nije potpuna autonomija.
- Škoda Tampere 2025. je opis pilota; 2026. opisuje implementaciju; Mannheim 27. 5. 2026. je demonstracija. Ne proglasiti svaki slučaj serijskim operativnim deploymentom.
- Siemensov cilj spremnosti AStriD za 2026. iz objave 2021. nije dokaz ispunjenja.
- Moskva ima opisanu automatsku putničku liniju, ali službeni izvor navodi zaposlenika u vozilu spremnog intervenirati. Ne pretpostaviti uštedu svih plaća ili preuzeti jamstvo da se sudar ne može dogoditi.
- Kotoriba/six BEMU ugovor 2026. ima isporuke 2028./2029.; centralna KONČAR platforma 2025. bila je u razvoju.

## Scenariji, ne potvrđeni profit

A digitalni servis: P4.500, C1.800, F90.000/god., I100.000. N100 daje prihod450.000, godišnji doprinos180.000, nakon pripreme80.000. Pokriće34/71. Isto ugovoreni maintenance ne naplaćuje se dvaput.

B ADAS jedne serije: P35.000, C25.000, I300.000; 50 ugradnji daje200.000 projektnog doprinosa prije neobuhvaćenih godišnjih troškova. Vlastiti razvoj I2milijuna pri istom doprinosu traži200 ugradnji; ilustracija, ne budžet pune autonomije.

C operatorov depot: 60 tramvaja,330d,35EUR/h,u75%,K1,5milijuna,F100.000. Pola sata stvarno oslobođenog rada/vozilo/dan daje159.875/god. i9,38god.; sat419.750 i3,57god. Petogodišnji prag46,18min. Korist operatora nije KONČAR profit. Uz pola sata i u25% rezultat−13.375. Pola bruto učinka prve godine u boljem slučaju produljuje povrat na4,19god.

D energetika:1000MWh×30%×20=6000; dodatni troškovi8000 daju−2000. Ne pretpostaviti da se sva energija može vremenski pomaknuti.

51/51 računskih testova i identičan ponovljeni izlaz. Svi izvori u završnom O005, lokalni DEBUG i rezultati zabilježeni u računskom prilogu. Bez SQL-a, internih sustava, intervjua ili pilota.

## Nastavak

O006 završiti iz javnih izvora i uključiti konačnu usporedbu svih šest. U portfeljsku usporedbu prenijeti da O005 sada obuhvaća i vlastiti tramvajski sigurnosni proizvod i selektivnu depot autonomiju, a ne samo baterijske vlakove. O005 je završen; ne otvarati novi tramvajski research task.
