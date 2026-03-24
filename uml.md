# UML dijagrami — Habit Tracker

---
## 1. Use Case dijagram

Korisnik se mora prijaviti kako bi mogao koristiti sustav.
Nakon prijave može kreirati navike, označavati ih kao izvršene,
pregledavati statistiku i brisati navike.
Podsjetnik je opcionalno proširenje kreiranja navike.
`````plantuml
@startuml
left to right direction
actor Korisnik

rectangle "Habit Tracker" {
  usecase "Prijava" as UC1
  usecase "Kreiranje navike" as UC2
  usecase "Označi kao izvršeno" as UC3
  usecase "Pregled statistike" as UC4
  usecase "Brisanje navike" as UC5
  usecase "Podsjetnik" as UC6
}

Korisnik -- UC1
Korisnik -- UC2
Korisnik -- UC3
Korisnik -- UC4
Korisnik -- UC5

UC2 ..> UC1 : <<include>>
UC3 ..> UC1 : <<include>>
UC4 ..> UC1 : <<include>>
UC6 ..> UC2 : <<extend>>
@enduml
` ``

---
