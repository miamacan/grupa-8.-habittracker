# Projekt: Habit tracker
## Članovi tima
- Mia Macan
- Marija Ferinović
- Ivan Bakša
  
## GitHub repozitorij
- Link: https://github.com/miamacan/grupa-8.-habittracker
- Svi članovi dodani: DA
  
## User storyji

**US-01**
Kao korisnik, želim svakodnevno označavati navike kao izvršene,
kako bih pratio jesu li moje navike redovite i vidio napredak kroz vrijeme.

**US-02**
Kao korisnik, želim pregledati statistiku i streak za svaku naviku,
kako bih se motivirao i uočio koje navike zanemarujem.

---

## Funkcijski zahtjevi

**FZ-01** Sustav mora omogućiti korisniku dodavanje nove navike s nazivom i opisom.
- Prioritet: Must
- Kriterij prihvaćanja: korisnik ispuni naziv i opis te potvrdi, navika se pojavljuje na popisu.

**FZ-02** Sustav mora prikazati popis svih korisnikovih navika na početnom ekranu.
- Prioritet: Must
- Kriterij prihvaćanja: sve dodane navike vidljive su odmah po otvaranju aplikacije.

**FZ-03** Sustav mora omogućiti korisniku označavanje navike kao izvršene za tekući dan.
- Prioritet: Must
- Kriterij prihvaćanja: korisnik klikne oznaku, navika se bilježi kao izvršena za taj dan.

**FZ-04** Sustav mora spriječiti dvostruko označavanje iste navike u istom danu.
- Prioritet: Must
- Kriterij prihvaćanja: jednom označena navika ne može se ponovo označiti isti dan.
  
**FZ-05** Sustav mora prikazati streak (broj uzastopnih dana) za svaku naviku.
- Prioritet: Should
- Kriterij prihvaćanja: streak se povećava za 1 svaki dan kad je navika izvršena, resetira se ako dan bude preskočen.

**FZ-06** Sustav mora omogućiti korisniku brisanje navike.
- Prioritet: Should
- Kriterij prihvaćanja: obrisana navika više se ne prikazuje na popisu, svi njezini zapisi se brišu.

## Nefunkcijski zahtjevi
 
**NZ-01** Aplikacija mora prikazati popis navika u roku od 1 sekunde za 95% slučajeva.
- Prioritet: Should
- Kriterij prihvaćanja: mjerenjem vrijeme učitavanja ne prelazi 1 sekundu.

**NZ-02** Aplikacija mora biti prilagođena mobilnim uređajima s ekranom od najmanje 360px širine.
- Prioritet: Must
- Kriterij prihvaćanja: svi elementi su čitljivi i klikabilni na ekranu širine 360px.
  
**NZ-03** Podaci o navikama moraju ostati sačuvani nakon zatvaranja i ponovnog otvaranja aplikacije.
- Prioritet: Must
- Kriterij prihvaćanja: navike i oznake vidljive su i nakon ponovnog pokretanja aplikacije.
 
---

## Taskovi
 
**TASK-01** Dizajnirati model podataka za naviku (naziv, opis, datum kreiranja)

**TASK-02** Dizajnirati model podataka za dnevno izvršavanje navike

**TASK-03** Implementirati ekran za prikaz popisa navika

---

## Raspodjela zadataka

**Mia Macan** FZ-01, FZ-02, NZ-01, TASK-01

**Ivan Bakša** FZ-03, FZ-04, NZ-02, TASK-02

**Marija Ferinović** FZ-05, FZ-06, NZ-03, TASK-03
