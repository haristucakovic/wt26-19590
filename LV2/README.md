# Laboratorijska vježba 2 — svi zadaci

Otvoriti HTML datoteke direktno u web pregledniku:

- `zadatak1/proba.html` — zadani sadržaj i raspored sa slike; stil je u `stil.css`.
- `zadatak2/index.html` — četiri interna linka, hover stil i završni block prikaz menija.
- `zadatak2/inline.html` — isti meni u inline prikazu za poređenje.
- `zadatak3/index.html` — tri izleta, zajednička klasa i izdvojena preporučena ponuda.
- `zadatak4/index.html` — forma za datum rođenja i email, prikaz drugog od pet koraka i dugmad prema slici.
- `zadatak5/index.html` — tabela bodovanja sa žutom pozadinom, sivim zaglavljem i spojenim ćelijama prema slici.

Korišteni su osnovni HTML i CSS iz LV1 i LV2, bez JavaScripta, biblioteka, flex ili grid rasporeda. Prvi zadatak koristi float i clear. Google font Gabriela se učitava putem HTTPS adrese; za njegovo prikazivanje potrebna je internetska veza.

U četvrtom zadatku korišteni su HTML element `progress` i tipovi polja `date` i `email` za kontrole prikazane na slici. Izgled tih kontrola zavisi od preglednika i jezika sistema. Dugmad su tipa `button`: zadatak prikazuje samo jedan korak forme, pa prelazak na druge korake i slanje podataka nisu implementirani.

U petom zadatku `rowspan` spaja ćeliju SI kroz dva reda, a `colspan` spaja po dvije ćelije za vrijednosti 30 i ?. Svojstvo `border-collapse: collapse` daje jednu zajedničku ivicu susjednim ćelijama.

## Poređenje za zadatak 2

Predviđanje prije promjene: širina od 200px neće uticati na običan inline link, dok će kod block linka određivati širinu sadržaja.

U pregledniku otvoriti obje verzije i provjeriti svaki link klikom na tekst i padding. U block verziji kliknuti i na prazan obojeni dio desno od teksta: cijela površina linka vodi na odgovarajući odjeljak. U inline verziji širina zavisi od teksta i paddinga, pa nema dodatnog praznog prostora nastalog od width: 200px. Klik izvan linka, na njegovu marginu ili na ostatak reda, ne aktivira link.

Za završno rješenje izabran je block prikaz: linkovi imaju jednake širine, svaki je u svom redu i veća klikabilna površina olakšava korištenje menija. Uz padding i border ukupna širina svakog block linka je 200 + 2 × 10 + 2 × 2 = 224px.
