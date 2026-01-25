# Karta projektu

Karta projektu to pierwszy oficjalny dokument projektowy, który opisuje jego podstawowe założenia: dlaczego projekt powstaje, co ma osiągnąć, jakie są ograniczenia, kto za co odpowiada i jak będzie mierzony sukces.

## Struktura karty projektu 

|Sekcja|Co zawiera|Przykładowe treści|
|---------------------|-------------------------------------------------|--------------------------------------|
|1. Tytuł projektu|Nazwa projektu i akronim|CampusX (Aplikacja do zarządzania wydarzeniami studenckimi)|
|2. Cel projektu|Co projekt ma osiągnąć i dlaczego|Umożliwienie tworzenia, rezerwacji i wyszukiwania przez studentów 
|3. Uzasadnienie biznesowe / edukacyjne|Dlaczego projekt jest potrzebny|Obecnie rezerwacje odbywają się e-mailowo. System poprawi efektywność i przejrzystość procesu.|
|4. Zakres projektu|Co wchodzi w zakres i co jest poza zakresem|W zakresie: rezerwacja, kalendarz,tworzenie wydarzeń ; poza zakresem: integracja z systemem facebook, powiadomienia |
|5. Główne wymagania|Wstępna lista funkcjonalności|Użytkownik może wyszukać wydarzenia, dokonać potwierdzenia uczestnicwa (rezerwacji), tworzenie wydarzeń|
|6. Zespół projektowy i role|Lista członków i ich funkcji|Kierownik – A. Myśliwiec, Frontendowiec – A. Myśliwiec, Tester/Analityk systemowy – P. Dąbrowski, Dokumentalista – W. Kuźmicz|
|7. Zasoby i narzędzia|Technologie, środowisko, repozytorium, narzędzia komunikacji|GitHub, Miro, Java, Spring Boot, HTMLL\CSS, PostgreSQL.|
|8. Harmonogram wstępny|Etapy realizacji projektu|Analiza wymagań (1–2 tydz.), Projektowanie (3–4 tydz.), Implementacja (5–7 tydz.), Testy (8 tydz.), Prezentacja (10 tydz.)|
|9. Ryzyka i działania zapobiegawcze|Potencjalne zagrożenia i sposoby ich ograniczenia|Brak komunikacji w zespole → okresowe spotkania online. Problemy z realizacją zadań → Pomoc zespołu/Praca wspólna.|
|10. Oczekiwane rezultaty (produkty projektu)|Co powstanie na koniec|Działający prototyp aplikacji + pełna dokumentacja projektowa.|
|11. Kryteria sukcesu|Jak zostanie oceniony sukces projektu|Aplikacja działa w przeglądarce, dokumentacja zawiera wszystkie diagramy UML.|
|12. Akceptacja projektu|Podpisy|Zatwierdza: prowadzący, kierownik projektu.|


## KARTA PROJEKTU 
# 1. Informacje ogólne

Tytuł projektu:
CampusX (Aplikacja do zarządzania wydarzeniami studenckimi)

Data utworzenia: 19.10.2025
Wersja dokumentu: 1.0
Zespół projektowy:

Imię i nazwisko | Rola w projekcie | Zakres odpowiedzialności
----------------|------------------|-------------------------
Alan Myśliwiec | Kierownik projektu / Frontendowiec | - Planowanie i koordynacja prac zespołu<br>- Raportowanie postępów<br>- Kontakt z prowadzącym<br>- Prezentacja końcowa projektu<br>- Tworzenie interfejsu użytkownika (frontend)
Paweł Dąbrowski | Tester manualny / Analityk systemowy / Dokumentalista | - Analiza wymagań systemowych<br>- Tworzenie przypadków użycia<br>- Opracowanie diagramów UML<br>- Testy manualne aplikacji<br>- Przygotowanie danych testowych<br>- Redakcja dokumentacji projektowej
Wojciech Kuźmicz | Dokumentalista | - Współtworzenie dokumentacji projektowej<br>- Redakcja i formatowanie dokumentów<br>- Uporządkowanie opisów diagramów UML<br>- Przygotowanie wersji końcowej dokumentacji<br>- Wsparcie zespołu w zakresie dokumentacji

Prowadzący: mgr Wojciech Moniuszko

# 2. Cel projektu

Celem projektu CampusX jest opracowanie i wdrożenie webowej aplikacji do zarządzania wydarzeniami studenckimi, umożliwiającej:

- studentom i wykładowcom szybkie tworzenie i promowanie wydarzeń,
- rezerwowanie terminów wydarzeń studenckich,
- rejestrowanie uczestników wydarzeń
- przeglądanie kalendarza dostępności wydarzeń,
- Projekt ma służyć jako prototyp systemu społecznościowego dla studentów oraz uczelni, z potencjałem dalszego rozwoju.

# 3. Uzasadnienie projektu

Obecnie organizacja wydarzeń studenckich odbywa się głównie za pośrednictwem mediów społecznościowych lub komunikatorów, co prowadzi do:

- braku centralnego miejsca gromadzenia informacji o wydarzeniach,
- trudności w koordynacji zespołów organizacyjnych,
- niskiej frekwencji wynikającej z ograniczonego przepływu informacji,
- braku możliwości analizy i archiwizacji danych o wydarzeniach.

Projekt rozwiązuje te problemy poprzez stworzenie zintegrowanej aplikacji do zarządzania wydarzeniami studenckimi, umożliwiającej planowanie i monitorowanie wydarzeń w jednym systemie. Dzięki temu zwiększa się efektywność organizacji, przejrzystość komunikacji oraz zaangażowanie społeczności akademickiej.

# 4. Zakres projektu

W zakresie projektu:

- Opracowanie wymagań funkcjonalnych i niefunkcjonalnych.
- Zaprojektowanie systemu z wykorzystaniem UML.
- Implementacja aplikacji webowej w technologii Spring Boot.
- Utworzenie relacyjnej bazy danych (PostgreSQL).
- Stworzenie dokumentacji projektowej i technicznej.
- Przeprowadzenie testów i zapełnienie danymi.
- Sprawdzenie projeku pod rodo.

Poza zakresem projektu:

- Integracja z facebookiem.
- Mobilna wersja.
- Integracja z narzedziami AI.

# 5. Wymagania

| ID  | Opis wymagania                                                | Priorytet | Źródło              |
| --- | ------------------------------------------------------------- | --------- | ------------------- |
| F1  | Użytkownik może się zarejestrować i zalogować do systemu      | Must      | Student             |
| F2  | Użytkownik może przeglądać listę wszystkich wydarzeń          | Must      | Student             |
| F3  | Użytkownik może filtrować wydarzenia (data, tagi, miejsce)    | Should    | Student             |
| F4  | Użytkownik może wyświetlić szczegóły wydarzenia               | Must      | Student             |
| F5  | Użytkownik może zapisać się na wydarzenie                     | Must      | Student             |
| F6  | Organizator może utworzyć nowe wydarzenie                     | Must      | Organizator         |
| F7  | Organizator może edytować i usuwać własne wydarzenia          | Must      | Organizator         |
| F8  | System wysyła powiadomienie potwierdzające rezerwację         | Should    | Student             |
| F9  | Administrator może zarządzać użytkownikami i rolami           | Must      | Admin               |
| F10 | System wyświetla kalendarz wydarzeń                           | Must      | Student/Organizator |
| F11 | System generuje raporty o frekwencji                          | Could     | Dyrekcja            |
| F12 | Użytkownik może zobaczyć listę wydarzeń, na które się zapisał | Must      | Student             |


# 6. Projekt systemu (UML)

W celu zaprojektowania architektury systemu CampusX oraz zobrazowania jego działania wykorzystano notację UML (Unified Modeling Language). Diagramy UML umożliwiają przedstawienie procesów biznesowych, struktury danych oraz komunikacji pomiędzy komponentami systemu.

6.1 Diagram przypadków użycia


<p align="center"> <img width="650" height="800" alt="diagram przypadków użycia" src="https://github.com/user-attachments/assets/bff5af1c-60ea-4c1e-9e5f-9db7a5687410" /> <p align="center"> *(Diagram przypadków użycia systemu CampusX)* </p> </p>

Diagram przypadków użycia przedstawia funkcjonalności systemu CampusX oraz role użytkowników korzystających z aplikacji. Wyróżniono trzech aktorów: Studenta, Organizatora oraz Administratora.

Student może przeglądać i wyszukiwać wydarzenia, zapisywać się na nie oraz anulować rezerwacje. Organizator posiada możliwość tworzenia wydarzeń oraz zarządzania uczestnikami. Administrator odpowiada za zarządzanie kontami użytkowników oraz moderację treści w systemie.

Diagram ten pozwala określić zakres odpowiedzialności poszczególnych użytkowników i stanowi podstawę dalszego projektowania systemu.

Diagram przypadków użycia przedstawia podstawowe funkcjonalności systemu CampusX oraz role użytkowników korzystających z aplikacji. Użytkownikami systemu są studenci, organizatorzy wydarzeń oraz administratorzy. Diagram ten umożliwia identyfikację głównych interakcji użytkowników z systemem oraz stanowi punkt wyjścia do dalszego projektowania systemu.

6.2 Diagram aktywności  
<p align="center">
<img width="438" height="467" alt="diagram aktywności" src="https://github.com/user-attachments/assets/e7153b0e-8b60-4b92-b425-0b32c866303e" />
<p align="center">
*(Proces tworzenia wydarzenia przez organizatora)*
  </p>
</p>

Diagram aktywności przedstawia proces tworzenia wydarzenia przez organizatora. Proces obejmuje wprowadzenie danych wydarzenia, ich walidację oraz zapis w bazie danych.

W przypadku poprawnych danych system zapisuje wydarzenie i wyświetla komunikat o sukcesie. Jeśli dane są błędne, użytkownik otrzymuje informację o błędach i możliwość ich poprawy.

6.3 Diagram klas  

<p align="center">
<img width="384" height="506" alt="diagram klas" src="https://github.com/user-attachments/assets/afb802e6-46f7-4d47-ba17-4f09ca357fb2" />
<p align="center">
  *(Struktura danych systemu)*
</p>
</p>


Diagram klas przedstawia strukturę danych systemu CampusX. Głównymi klasami są User, Event oraz Reservation.

Klasa User reprezentuje użytkownika systemu i zawiera informację o jego roli. Klasa Event opisuje wydarzenie, natomiast klasa Reservation odpowiada za zapisy użytkowników na wydarzenia. Diagram ten stanowi podstawę do zaprojektowania bazy danych systemu.

6.4 Diagram sekwencji  

<p align="center">
<img width="679" height="414" alt="diagram sekwencji" src="https://github.com/user-attachments/assets/25f8cb94-9fe4-41d1-b993-b10fe9c3804c" />
  <p align="center">
*(Proces zapisu studenta na wydarzenie)*
  </p>
</p>

Diagram sekwencji przedstawia proces zapisu studenta na wydarzenie. Pokazuje on komunikację pomiędzy interfejsem użytkownika, backendem, bazą danych oraz systemem e-mail.

Proces rozpoczyna się od wysłania żądania zapisu, następnie dane są zapisywane w bazie, a użytkownik otrzymuje potwierdzenie zapisu w aplikacji oraz wiadomość e-mail.



# 7. Zespół projektowy i role

Rola | Osoba | Odpowiedzialność
--------------|-------------------------|-----------------------------------------------------------------------
Kierownik projektu / Frontendowiec | Alan Myśliwiec | Planowanie i koordynacja prac zespołu, raportowanie postępów, kontakt z prowadzącym, prezentacja końcowa projektu, tworzenie interfejsu użytkownika (frontend)
Tester manualny / Analityk systemowy / Dokumentalista | Paweł Dąbrowski | Analiza wymagań, tworzenie przypadków użycia, opracowanie diagramów UML, testy manualne, przygotowanie danych testowych, redakcja dokumentacji projektowej
Dokumentalista | Wojciech Kuźmicz | Współtworzenie i redakcja dokumentacji projektowej, formatowanie dokumentów, przygotowanie opisów diagramów UML, wsparcie zespołu w zakresie dokumentacji

# 8. Zasoby i narzędzia

Kategoria|Narzędzie / Technologia|Cel zastosowania
-----------------|-----------------------------------|----------------------------------------------------------
Zarządzanie projektem|GitHub Projekt|Planowanie sprintów, śledzenie zadań
Repozytorium|GitHub|Kontrola wersji kodu
Analiza i projektowanie| Miro, Plant Text |Diagramy UML, mapa procesu
Programowanie|Java (Spring Boot), HTML/CSS|Implementacja aplikacji
Baza danych|PostgreSQL|Przechowywanie danych o wydarzeniach i urzytkonikach
Dokumentacja|Word|Tworzenie dokumentacji technicznej
Komunikacja|Telegram, Discord|Spotkania zespołowe

# 9. Harmonogram realizacji (10 spotkań)

Etap|Zakres|Czas realizacji|Rezultat
---|----------------------------------------------------|----------------|--------------------------------------
1|Tworzenie zespołów, wybór tematu, karta projektu|Tydzień 1|Karta projektu, struktura zespołu
2|Analiza wymagań|Tydzień 2|Dokument wymagań
3|Projekt systemu – UML|Tydzień 3–4|Diagramy UML
4|Konfiguracja środowiska|Tydzień 4|Repozytorium, narzędzia
5|Dokumentacja projektowa (I etap)|Tydzień 5|Projekt dokumentu
6|Implementacja prototypu (I etap)|Tydzień 6–7|Pierwsza wersja aplikacji
7|Testowanie i poprawki|Tydzień 8|Raport testów
8|Dokumentacja końcowa i prezentacja|Tydzień 9–10|Prezentacja, protokół odbioru

# 10. Analiza ryzyka

Nr|Ryzyko|Prawdopodobieństwo|Skutek|Działanie zapobiegawcze
--|---------------------------|-----------|-----------------------------------|---------------------------------
1|Opóźnienia w pracy zespołu|Średnie|Wysoki|Spotkania tygodniowe, śledzenie postępów w GitHub Projects
2|Brak doświadczenia w tworzeniu dokumentacji technicznej|Wysokie|Średni|Pomoc zespołu i szkolenie z  wykorzystaniem źródeł z internetu.
3|Konflikty w zespole|Niskie|Średni|Jasny podział ról, komunikacja na Discord
4|Utrata danych|Niskie|Wysoki|Regularne kopie oraz kontrola wersji w GitHub
5|Niedostateczna dokumentacja|Niskie|Wysoki|Wczesne rozpoczęcie opracowania przez dokumentalistę
6|Brak czasu|Średnie|Średnie|Wydłużenie deadline, ewentualne wsparcie zespołu w realizacji zadań

# 11. Kryteria sukcesu projektu

- Wszystkie wymagania funkcjonalne zostały zaimplementowane.
- Aplikacja uruchamia się lokalnie i działa poprawnie.
- Dokumentacja zawiera pełny zestaw diagramów UML.
- Testy zakończone wynikiem pozytywnym.
- Zespół zrealizował projekt w wyznaczonym czasie.
- Projekt został pozytywnie oceniony przez prowadzącego.

# 12. Rezultaty projektu

- Prototyp aplikacji webowej (CampusX).
- Dokumentacja projektowa (wymagania, UML, testy).
- Dokumentacja techniczna (instrukcja uruchomienia).
- Prezentacja zespołowa ( prezentacja na żywo).
- Raport końcowy i protokół zdawczo-odbiorczy.

# 13. Akceptacja projektu

Funkcja|Imię i nazwisko|Data|Podpis
------------|-------------------------------|--------------|----------------------------------|
Kierownik projektu|Alan Myśliwec|19.10.2025|___________
Prowadzący|mgr Wojciech Moniuszko|19.10.2025|___________

## Uwagi końcowe:

- Dokument powinien być przechowywany w repozytorium projektu.
- Aktualizacja wersji dokumentu wymaga zgody kierownika projektu i prowadzącego.
- Każdy członek zespołu ma obowiązek zapoznać się z treścią karty i ją zaakceptować.






























