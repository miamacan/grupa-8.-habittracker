
# UML dijagrami – Habit Tracker

## Class dijagram

Class dijagram prikazuje osnovnu strukturu sustava Habit Tracker. Sustav se sastoji od klasa Korisnik, Navika i IzvrsenjeNavike. Korisnik može imati više navika, dok svaka navika pripada jednom korisniku. Svaka navika sadrži više dnevnih izvršenja koja predstavljaju zapise o tome je li navika izvršena određenog dana. Veza između klase Navika i IzvrsenjeNavike modelirana je kompozicijom, što znači da se brisanjem navike brišu i sva njezina izvršenja. Multipliciteti prikazuju odnose između klasa.


@startuml

class Korisnik {
  - korisnikId : int
  - ime : String
  - email : String
}

class Navika {
  - navikaId : int
  - naziv : String
  - opis : String
  - datumKreiranja : Date
}

class IzvrsenjeNavike {
  - izvrsenjeId : int
  - datum : Date
  - izvrsena : boolean
}

Korisnik "1" -- "0..*" Navika : ima
Navika "1" *-- "0..*" IzvrsenjeNavike : sadrzi

@enduml
