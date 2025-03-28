# 🧪 Laboratoria z Podstaw Javy – Zadanie: Walidator PESEL

## 🎯 Cel zadania

Celem ćwiczenia jest stworzenie prostego walidatora numeru PESEL oraz klasy `Person`, która będzie na jego podstawie odczytywać podstawowe dane.

---

## ✅ Część 1: Klasa `PeselValidator`

🔧 Stwórz klasę `PeselValidator` z publiczną, statyczną metodą `isValid`, która sprawdzi, czy PESEL jest poprawny. Umieść klasę w pakiecie `com.pjatk.pesel.model`.

### ✨ Wzór implementacji:

```java
package com.pjatk.pesel.model;

public class PeselValidator {
    public static boolean isValid(String pesel) {
        // Algorytm sprawdzający, czy nr PESEL jest poprawny 
        // (wyrażenie regularne + suma kontrolna)

        return false;
    }
}
```

📌 Wskazówka: Algorytm wyliczania sumy kontrolnej znajdziesz [tutaj](https://www.gov.pl/web/gov/czym-jest-numer-pesel)

---

## ✅ Część 2: Klasa `Person`

🔧 Stwórz klasę `Person` w tym samym pakiecie: `com.pjatk.pesel.model`.

### 🔨 Wymagania:

- Konstruktor przyjmujący numer PESEL jako argument
- Właściwości klasy (z getterami i setterami tam, gdzie potrzebne):

### Właściwości:

- Imię i nazwisko – z getterami i setterami
- Numer PESEL – tylko getter
- Płeć – odczytywana z numeru PESEL
- Data urodzenia – odczytywana z numeru PESEL

📌 Wskazówki:
- Płeć zakodowana jest w 10. cyfrze PESEL-a.
- Data urodzenia zakodowana jest w pierwszych 6 cyfrach – zwróć uwagę na miesiąc, który może mieć dodane 20/40/60 dla określenia wieku i stulecia.

---

## 🗂️ Diagram klas

Poniżej znajduje się diagram klas pomocny w implementacji:

![Class Diagram](http://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/PJMPR/lab04-introduction-to-properties/main/UML/diagram3.puml)

---

Powodzenia! 💻✨
