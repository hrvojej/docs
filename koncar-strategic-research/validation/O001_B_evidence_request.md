# O001-B — ciljani paket internih dokaza

**Status:** zahtjev pripremljen, nije poslan ni ispunjen. **Datum:** 2026-09-22.

[Board](TASK_BOARD.md) · [R006](../research/R006_O001_existing_stack_offer_audit_2026-09-22.md)

## Zašto i tko

Treba ustanoviti što je stvarno već isporučeno, što je naplativo, koja su prava i što bi točno bio dodatak O001. Početni davatelji: TMS product/engineering i servis u Institutu; financije/prodaja Instituta; D&ST postprodaja. Digital/NEOS uključiti za stvarno postojeću ili planiranu integraciju, ne automatski pretpostaviti njihovo vlasništvo proizvoda.

Osjetljive priloge dostaviti u odobren privatni prostor. Javni repo sadrži samo ovaj zahtjev, ID i odobreni agregirani zaključak. Ne slati vjerodajnice, ključeve, mrežne adrese kupaca ili neanonimizirane ugovore u javni repo.

## Minimalni paket — šest cjelina

| ID | Što tražimo | Zašto / format koji je dovoljan za početak |
|---|---|---|
| DR01 | Jedna aktualna arhitektura i tablica TMS/KonFID/iPDCore/software verzija, od lokalne akvizicije do korisničkog pristupa | Redigirani PDF/MD dijagram i opis trust granica; odvojiti deployed od roadmapa. Navesti tko održava koji sloj. |
| DR02 | Jedan anonimizirani export mjerenja i jedan alarm/event/diagnostic rezultat s dokumentacijom polja | Izvorni strojno čitljivi format ili vjeran sintetički fixture uz jasnu oznaku. Jedinice, tipovi, vrijeme, quality flag, verzije; uzorak nije reprezentativnost flote. |
| DR03 | Popis proizvodnih funkcija/licenci i teritorijalno-version matrica, uključujući DSync napomenu | Funkcija, izdanje, vlasnik/licenca, dopuštena tržišta, iznimke i alternativna konfiguracija; razlog zabrane ne nagađati. |
| DR04 | Reprezentativna ponuda, osnovni ugovor i service/SLA prilog te model obnove | Anonimizirati kupca. Odvojiti jednokratnu isporuku, periodični servis, licencu, SLA odgovor i availability jamstvo; opći uvjeti nisu zamjena. |
| DR05 | Agregirani aktualni inventory isporuka i ugovora | Broj TMS nasuprot drugim monitorima; aktivan/ugašen; verzija; povezivost; prava pristupa; zemlja; partner; service attach/renewal. Ne treba puni popis lokacija. |
| DR06 | Posljednjih 12 mjeseci product/service baseline i 3 tipična projekta troška | Anonimizirane stavke prihoda/troška, sati onboardinga/eksperata/podrške, put, licence, hosting, incidenti i neplaćene intervencije. Ukupan prihod Instituta nije dovoljan. |

Dodatno za produkcijsku odluku: aktualni certifikati s opsegom/verzijom; SLA roster/dežurstvo; politika zakrpa/SBOM gdje postoje; dokumentirana prava customer data, izvedenih featurea i treniranja; stvarna dodjela P&L/product odgovornosti. Pribaviti samo ono za što postoji ovlaštenje.

## Pitanja koja brzo mogu srušiti početnu tezu

1. Prodaje li se već fleet APM ili stalni ekspertni nadzor? Pod kojim nazivom/SKU-om, kome i s kakvom obnovom?
2. Koji precizan zahtjev kupca sada ne možemo ispuniti i je li kupac za njega ponudio budžet?
3. Postoje li customer-side APM i servis koji bi nova ponuda samo duplicirala?
4. Tko smije pristupiti i analizirati povijesne podatke te trenirati/prenijeti model između kupaca?
5. Što točno pokriva teritorijalna napomena za DSync? Postoji li podržana alternativa po tržištu?
6. Koliko vremena stručnjak troši po uređaju i alarmu; je li terenski odgovor već uključen u cijenu?
7. Može li postojeći tim isporučiti dodatnu uslugu bez uzimanja kapaciteta profitabilnijim obvezama?
8. Postoji li već odgovoran product/P&L owner? Nepostojanje javnog imena ne znači da ga nema.

## Test stvarne transformacije podataka

U DR02 prvo zadržati izvorni payload. Dokumentirati dekodiranje, jedinične konverzije, nedostajuće/invalid vrijednosti, timezone i source timestamp, kalibraciju, kvalitetu, model i konfiguracijski hash. Predloženi metapodaci nisu tvrdnja da takva polja već postoje u TMS-u.

Usporediti golden fixture s izvornim TMS prikazom i kontrolnim ekspertom. Reproducirati isti event dvaput, zamijenjen redoslijed, prekid veze/backfill i promjenu senzora/firmwarea. Test mora pokazati da nema tihe zamjene nule i nepoznate vrijednosti, gubitka jedinice, dvostrukog alarma ili miješanja asset ID-a.

Za visoko-frekventne signale odvojiti raw waveform, PRPD/features, health result i alarm. Ne izračunavati cloud trošak iz peak sampling ratea bez trigger duty cyclea, kodiranja i stvarnog export režima.

## Izlaz O001-B

`validation/results/O001-B.md`: potvrđena as-is arhitektura, postojeći SKU/servisni model, ownership/prava, popis izmjerenih gapova i dokazni lokatori u privatnom prostoru. Javni sažetak samo nakon odobrenja. Status može biti PARTIAL/HOLD; ne označiti VALIDATED ako su ostali ključni tokovi ili prava nepoznati.
