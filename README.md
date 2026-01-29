FlashMaster Pro - System Wspomagania Nauki (SPA)



**FlashMaster Pro** to aplikacja webowa typu **Single Page Application (SPA)** służąca do efektywnej nauki języków obcych i pojęć technicznych. System wykorzystuje mechanizm fiszek (flashcards) oraz autorski algorytm kolejkowania powtórek, zapewniając optymalizację procesu zapamiętywania.

---

Funkcjonalności

Aplikacja oferuje kompletny zestaw narzędzi do zarządzania bazą wiedzy:

* **Pełny CRUD (Create, Read, Update, Delete):** edytor pozwalający na dodawanie, usuwanie i  edycję istniejących fiszek.
* **Dynamiczne Zarządzanie Kategoriami:** System automatycznie wykrywa kategorie i pozwala użytkownikowi tworzyć nowe grupy tematyczne (Custom Groups) w locie.
* **Algorytm Powtórek (Retry Logic):** Błędne odpowiedzi nie przerywają sesji, lecz są dynamicznie przenoszone na koniec kolejki (FIFO), wymuszając przyswojenie materiału.
* **Persistent State (Trwałość Danych):** Integracja z **LocalStorage API** zapewnia zapisywanie postępów i bazy danych po zamknięciu przeglądarki bez konieczności użycia backendu.
* **Interaktywny Interfejs 3D:** Wykorzystanie CSS3 Transforms do płynnych animacji odwracania kart.
* **Responsive Web Design (RWD):** Interfejs w pełni dostosowany do urządzeń mobilnych (Mobile First approach).

---

Technologie i Architektura

Projekt został zrealizowany w czystych technologiach webowych (Vanilla Stack), aby zapewnić maksymalną wydajność i kontrolę nad kodem.

* **Frontend:** HTML5 (Semantyczny), CSS3 (Grid, Flexbox, Zmienne CSS, 3D Transforms).
* **Logic:** JavaScript (ES6+), Programowanie Obiektowe (organizacja kodu w obiekcie `app`).
* **Data:** JSON & LocalStorage API.
* **Design System:** Autorski system zmiennych CSS (`:root`) zapewniający spójność wizualną (kolory, cienie, zaokrąglenia).

Struktura Kodu (MVC Pattern)
Mimo braku zewnętrznych frameworków, kod aplikacji naśladuje wzorzec **Model-View-Controller**:
1.  **Model:** Tablica obiektów `cards` i metody zarządzania danymi (`save`, `getUniqueCategories`).
2.  **View:** Metody renderujące DOM (`renderDashboard`, `renderEditorList`).
3.  **Controller:** Logika sterująca przepływem (`handleFormSubmit`, `rateCard`, `switchView`).

---

Jak uruchomić projekt?

Aplikacja jest statyczna i nie wymaga instalacji Node.js ani konfiguracji serwera.

### Metoda 1: Live Demo
Sprawdź działającą wersję online: **tranquil-cactus-58a1d3.netlify.app**

### Metoda 2: Lokalnie
1. Sklonuj repozytorium:
   ```bash
   git clone https://github.com/wiktoriasikerko05/projekt-fiszki.git
