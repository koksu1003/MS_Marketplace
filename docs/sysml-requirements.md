# Wymagania Systemowe SysML (ISO/IEC 25002) - MS Marketplace

## 1. Struktura Wymagań (System Hierarchy)
* **REQ_00_SYSTEM:** Główny węzeł wymagań MS Marketplace
  * **REQ_01_SYSTEM:** Wymagania Funkcjonalne
  * **REQ_02_SYSTEM:** Wymagania Niefunkcjonalne (NFR)

---

## 2. Wymagania Funkcjonalne (Functional Requirements)
* **ID: FR_01_LIST** — System umożliwia przeglądanie i filtrowanie listy ogłoszeń.
* **ID: FR_02_ADD** — Użytkownik może dodawać nowe ogłoszenia w różnych kategoriach.
* **ID: FR_03_PROFILE** — Użytkownik może sprawdzać informacje o odbytych transakcjach na swoim profilu.
* **ID: FR_04_CHAT** — Użytkownicy mogą wymieniać wiadomości tekstowe w celu dogadania odbioru.

---

## 3. Wymagania Niefunkcjonalne (NFR wg ISO/IEC 25002)

* **ID: NFR_01_AVAIL (Dostępność / Availability)**
  * *Opis:* Dostępność systemu wynosi minimum **96%** w skali miesiąca.
* **ID: NFR_02_MTBF (Niezawodność / Reliability)**
  * *Opis:* Średni czas bezawaryjnej pracy (MTBF) wynosi co najmniej **720 godzin** ciągłej pracy.
* **ID: NFR_03_MTTR (Odtwarzalność / Maintainability)**
  * *Opis:* Średni czas naprawy po awarii (MTTR) nie przekracza **30 minut**.
* **ID: NFR_04_PERF (Wydajność / Performance)**
  * *Opis:* Czas odpowiedzi serwera przy ładowaniu widoku ogłoszeń wynosi **poniżej 1 sekundy** przy obciążeniu **200 zapytań na sekundę**.