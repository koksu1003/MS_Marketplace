# Historie Użytkowników (User Stories) - MS Marketplace

---

## US-01: Oddawanie przedmiotów za darmo przy wyprowadzce
**Jako:** Student kończący studia i wyprowadzający się z akademika  
**Chcę:** Wystawić ofertę oddania niepotrzebnych przedmiotów za darmo  
**Aby:** Szybko pozbyć się rzeczy przed wyprowadzką bez wyrzucania ich.

### Scenariusz 1: Wystawienie oferty "Za darmo"
* **Given** Zalogowany student znajduje się na platformie MS Marketplace
* **When** Student tworzy post z odpowiednim opisem i wybraną kategorią oraz oznacza go jako "Za darmo"
* **Then** System publikuje ofertę z widoczną etykietą "Za darmo" na liście ogłoszeń.

### Scenariusz 2: Akceptacja zgłoszenia odbioru
* **Given** Student dostaje powiadomienie o chęci odbioru wystawionego przedmiotu przez innego użytkownika
* **When** Student akceptuje odbiór przez wybraną osobę
* **Then** System automatycznie ukrywa odebrany przedmiot z publicznej listy ofert.

---

## US-02: Zgłaszanie zapotrzebowania i pożyczanie przedmiotów (Szukam)
**Jako:** Student potrzebujący sprzętu (np. kalkulatora) na egzamin  
**Chcę:** Opublikować ogłoszenie z informacją o potrzebie pożyczenia przedmiotu i określić czas zwrotu  
**Aby:** Znaleźć osobę z miasteczka studenckiego, która pożyczy mi potrzebny przedmiot.

### Scenariusz 1: Publikacja ogłoszenia o potrzebie
* **Given** Zalogowany student znajduje się na platformie
* **When** Student wypełnia opis ogłoszenia wraz z wyraźnie określonymi datami odbioru i oddania
* **Then** System publikuje ogłoszenie oznaczone jako "Szukam" z zaznaczonym okresem zwrotu.

### Scenariusz 2: Reakcja innego studenta na potrzebę
* **Given** Student innego kierunku przegląda ofertę na stronie i widzi ogłoszenie "Szukam"
* **When** Wyraża chęć pożyczenia przedmiotu i klikając przycisk "Mam", potwierdza dostępność
* **Then** Autor ogłoszenia otrzymuje powiadomienie systemowe o zgłoszeniu pomocy.

---

## US-03: Bezpośrednia wymiana przedmiotów (Barter)
**Jako:** Mieszkaniec akademika  
**Chcę:** Wystawić przeczytaną książkę w kategorii wymiany i podać oczekiwany przedmiot na zamianę  
**Aby:** Wymienić się na inną książkę bez używania gotówki.

### Scenariusz 1: Odrzucenie propozycji wymiany
* **Given** Student wystawiający ofertę otrzymuje propozycję wymiany z książką, która mu nie odpowiada
* **When** Student odrzuca przekazaną propozycję
* **Then** Oferta pozostaje aktywna na stronie, a osoba proponująca wymianę otrzymuje powiadomienie o odmowie.

### Scenariusz 2: Akceptacja propozycji wymiany
* **Given** Student dostaje inną propozycję wymiany przedmiotu
* **When** Student akceptuje propozycję
* **Then** Oferta książki znika z listy aktywnych ogłoszeń, a status zmienia się na zakończony.

---

## US-04: Sprzedaż używanych przedmiotów wartościowych
**Jako:** Student posiadający niepotrzebny, wartościowy sprzęt (np. rower)  
**Chcę:** Wystawić ogłoszenie sprzedaży wraz ze zdjęciami, opisem i ceną  
**Aby:** Sprzedać stary przedmiot innemu studentowi z miasteczka.

### Scenariusz 1: Wystawienie oferty sprzedaży
* **Given** Student posiada przedmiot, który chce sprzedać
* **When** Tworzy ofertę zawierającą opis, cenę oraz zdjęcia przedmiotu
* **Then** Oferta pojawia się w serwisie na liście ofert sprzedaży.

### Scenariusz 2: Zakup przedmiotu
* **Given** Inny student przegląda stronę i natrafia na ogłoszenie sprzedaży roweru
* **When** Klika opcję "Kup teraz" / chęć zakupu
* **Then** Oferta zostaje ukryta, a system rejestruje rozpoczęcie transakcji.

---

## US-05: Zarządzanie kontem, aktywnymi ogłoszeniami i historią
**Jako:** Aktywny użytkownik platformy  
**Chcę:** Przeglądać swoje aktywne ogłoszenia oraz historię odbytych transakcji w panelu profilu  
**Aby:** Śledzić status moich wymian, sprzedaży i odbiorów.

### Scenariusz 1: Sprawdzanie własnych aktywnych ogłoszeń
* **Given** Zalogowany student znajduje się na stronie swojego konta
* **When** Przechodzi do zakładki "Moje ogłoszenia"
* **Then** Widzi listę wszystkich wystawionych przez siebie ogłoszeń, które są obecnie aktywne.

### Scenariusz 2: Przeglądanie historii transakcji
* **Given** Zalogowany student znajduje się na stronie swojego konta
* **When** Przechodzi do zakładki "Historia transakcji"
* **Then** Widzi pełną historię odbytych transakcji wraz z ich szczegółowymi danymi (przedmiot, data, strona transakcji, status).