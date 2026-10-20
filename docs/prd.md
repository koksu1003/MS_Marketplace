# Product Requirements Document (PRD) — MS Marketplace

**Nazwa projektu:** MS Marketplace  
**Autorzy / Zespół:** Michał Skrzyczek, Filip Sikora, Mikołaj Samek  
**Przewidywany stos technologiczny:** Next.js  
**Wersja:** 1.0  
**Data utworzenia:** Październik 2026  

---

## 1. Przegląd i Wizja Produktu

**MS Marketplace** to dedykowana platforma e-commerce i P2P (Peer-to-Peer) przeznaczona do wymiany, wypożyczeń, sprzedaży oraz darmowego przekazywania przedmiotów pomiędzy studentami w obrębie Miasteczka Studenckiego AGH. 

Głównym celem projektu jest stworzenie bezpiecznego, wygodnego i zsynchronizowanego lokalnie miejsca handlu i wymiany bezpotrzebnych lub potrzebnych tymczasowo przedmiotów (notatki, sprzęt naukowy, meble, książki, rowery) bez konieczności używania tradycyjnych przesyłek kurierskich.

---

## 2. Problemy Użytkowników i Propozycja Wartości

### 2.1. Identyfikowane problemy (Pain Points)
* **Chaotyczny handel na grupach Facebookowych:** Wiadomości giną w powiadomieniach/spamie, a przeszukiwanie ofert według własnych kryteriów (np. konkretny akademik, stan, kategoria) jest niemożliwe.
* **Brak zaufania i obawa przed wypożyczaniem:** Strach przed pożyczaniem przedmiotów nieznajomym bez weryfikacji tożsamości.
* **Marnotrawstwo i kupowanie na jeden raz:** Konieczność kupowania drogiego sprzętu (np. kalkulatora naukowego) na jeden egzamin lub wyrzucanie sprawnego sprzętu, mebli i notatek na koniec roku akademickiego przy wyprowadzce.
* **Niezjawianie się na odbiór ("Ghosting"):** Anonimowość na ogólnych platformach sprzyja ignorowaniu ustaleń odbioru osobistego.

### 2.2. Korzyści dla użytkowników (Value Proposition)
* **Szybka dostępność lokalna:** Znalezienie przedmiotu w promieniu kilkuset metrów (w obrębie akademików).
* **Zamknięta i bezpieczna społeczność:** Eliminacja anonimowości dzięki weryfikacji studentów.
* **Formalizacja wypożyczeń:** Czytelne definiowanie ram czasowych zwrotu sprzętu.
* **Oszczędność finansowa i ekologia:** Przedłużenie życia przedmiotów, redukcja śmieci i mniejsze koszty dla studenckiego budżetu.

---

## 3. Analiza Modelu Biznesowego (Kanwa Modelu Biznesowego)

| Obszar Kanwy | Opis / Elementy |
| :--- | :--- |
| **Segmenty Klientów** | Mieszkańcy Miasteczka Studenckiego AGH, Reklamodawcy |
| **Propozycja Wartości** | Dedykowane miejsce do szybkiej wymiany, wypożyczania i sprzedaży przedmiotów w zamkniętej społeczności studenckiej. |
| **Kanały** | Social media, maile uczelniane, ogłoszenia papierowe w akademikach. |
| **Relacje z Klientami** | Komunikacja mailowa, oficjalne profile w Social Media, powiadomienia systemowe. |
| **Kluczowe Działania** | Produkcja oprogramowania, marketing, rozwiązywanie problemów użytkowników, moderacja ofert. |
| **Kluczowe Zasoby** | Zasoby ludzkie (zespół programistyczny), finansowe, własność intelektualna. |
| **Kluczowi Partnerzy** | Reklamodawcy, władze miasteczka studenckiego / uczelni. |
| **Struktura Kosztów** | Utrzymanie serwerów/domeny, utrzymanie i rozwój (maintenance), moderacja treści. |
| **Struktura Przychodów** | Wyświetlanie reklam, konta premium dla użytkowników. |

---

## 4. Główne Przypadki Użycia (Use Cases)

* **UC1: Oddawanie przedmiotów przy wyprowadzce (Za darmo)**  
  Student kończący ostatni semestr studiów wyprowadza się z akademika i chce pozbyć się przedmiotów, których nie będzie już potrzebował. Wystawia ofertę z etykietą "Za darmo". Inny student zgłasza się przez platformę i odbiera przedmioty pod akademikiem.

* **UC2: Wypożyczenie na określony czas (Kalkulator/Sprzęt)**  
  Student potrzebuje kalkulatora naukowego na egzamin. Wystawia ogłoszenie o zapotrzebowaniu na sprzęt. Student z innego kierunku wypożycza mu kalkulator na ściśle określony w aplikacji czas zwrotu.

* **UC3: Wymiana bezgotówkowa (Barter)**  
  Student po przeczytaniu książki wystawia ją na stronę w kategorii wymiany. Mieszkaniec tego samego domu studenckiego odpowiada z propozycją innej książki. Wystawiający akceptuje ofertę i następuje bezpośrednia wymiana.

* **UC4: Sprzedaż sprzętu wartościowego (np. Rower)**  
  Student po zakupie nowego roweru chce sprzedać stary. Wystawia ofertę sprzedaży ze zdjęciami i ceną. Inny student kupuje go przez platformę, po czym następuje płatność i przekazanie przedmiotu.

---

## 5. Kluczowe Wymagania Funkcjonalne (Functional Requirements)

1. **Weryfikacja i Logowanie:** System uwierzytelniania kont studenckich (powiązanie z e-mailem uczelnianym).
2. **Kategoryzacja Ofert:** Możliwość wyboru typu ogłoszenia: *Sprzedam*, *Wymienię*, *Wypożyczę (Szukam)*, *Za darmo*.
3. **Filtrowanie i Wyszukiwanie:** Wyszukiwanie po nazwie, kategorii, stanie przedmiotu oraz lokalizacji (akademik/blok).
4. **Moduł Umawiania Odbioru:** System akceptacji/odrzucania zgłoszeń od innych użytkowników i zarządzania czasem wypożyczenia.
5. **Profil Użytkownika:** Zakładka "Moje ogłoszenia" oraz "Historia transakcji" pozwalająca śledzić status aktywności.

---

## 6. Architektura i Technologie

* **Frontend & Backend Framework:** `Next.js` (React / Node.js) — zapewniający szybki rendering (SSR/SSG), dobre wsparcie dla PWA (Progressive Web App) oraz prostą integrację API.
* **Model Wdrożenia:** Hostowanie na serwerze chmurowym z podpiętą domeną MS Marketplace.
