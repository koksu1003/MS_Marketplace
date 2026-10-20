# Przypadki Użycia (Use Cases) - MS Marketplace

## Aktorzy Systemu
* **Student (Wystawiający):** Osoba publikująca ogłoszenie (sprzedaż, oddanie za darmo, wymiana, wypożyczenie).
* **Student (Odbiorca / Kupujący):** Osoba przeglądająca oferty i wchodząca w interakcję z ogłoszeniami.

---

## Mapowanie Przypadków Użycia na User Stories

### 1. Moduł: Oddawanie za darmo (US-01)
* **UC-01: Wystawienie oferty "Za darmo"**
  * *Aktor:* Student (Wystawiający)
  * *Opis:* Użytkownik wypełnia formularz i publikuje przedmiot z etykietą "Za darmo".
* **UC-02: Akceptacja przekazania przedmiotu**
  * *Aktorzy:* Student (Wystawiający), Student (Odbiorca)
  * *Opis:* Wystawiający akceptuje zgłoszenie chętnego odbiorcy, a system ukrywa przedmiot.

### 2. Moduł: Pożyczanie / Szukam (US-02)
* **UC-03: Publikacja ogłoszenia "Szukam"**
  * *Aktor:* Student (Wystawiający)
  * *Opis:* Użytkownik publikuje potrzebę pożyczenia przedmiotu z określoną datą zwrotu.
* **UC-04: Reakcja na potrzebę (Przycisk "Mam")**
  * *Aktor:* Student (Odbiorca)
  * *Opis:* Użytkownik deklaruje chęć pożyczenia przedmiotu i zgłasza się do ogłoszeniodawcy.

### 3. Moduł: Wymiana Barterowa (US-03)
* **UC-05: Wystawienie oferty na wymianę**
  * *Aktor:* Student (Wystawiający)
  * *Opis:* Użytkownik dodaje przedmiot z informacją, na co chciałby go wymienić.
* **UC-06: Obsługa propozycji wymiany**
  * *Aktorzy:* Student (Wystawiający), Student (Odbiorca)
  * *Opis:* Wystawiający akceptuje lub odrzuca zaproponowaną przez drugą osobę ofertę wymiany.

### 4. Moduł: Sprzedaż Przedmiotów (US-04)
* **UC-07: Wystawienie oferty sprzedaży**
  * *Aktor:* Student (Wystawiający)
  * *Opis:* Użytkownik dodaje opis, cenę oraz zdjęcia sprzedawanego przedmiotu.
* **UC-08: Zakup przedmiotu ("Kup teraz")**
  * *Aktor:* Student (Odbiorca)
  * *Opis:* Użytkownik klika chęć zakupu, co ukrywa ogłoszenie i rozpoczyna transakcję.

### 5. Moduł: Panel Profilu Użytkownika (US-05)
* **UC-09: Przeglądanie własnych aktywnych ogłoszeń**
  * *Aktorzy:* Student (Wystawiający), Student (Odbiorca)
  * *Opis:* Użytkownik sprawdza listę aktualnie opublikowanych przez siebie ogłoszeń.
* **UC-10: Przeglądanie historii transakcji**
  * *Aktorzy:* Student (Wystawiający), Student (Odbiorca)
  * *Opis:* Użytkownik przegląda zakończone transakcje i ich szczegóły.