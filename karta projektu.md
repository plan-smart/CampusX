# Karta projektu

Karta projektu to pierwszy oficjalny dokument projektowy, który opisuje jego podstawowe założenia: dlaczego projekt powstaje, co ma osiągnąć, jakie są ograniczenia, kto za co odpowiada i jak będzie mierzony sukces.

## Struktura karty projektu 

|Sekcja|Co zawiera|Przykładowe treści|
|---------------------|-------------------------------------------------|--------------------------------------|
|1. Tytuł projektu|Nazwa projektu i akronim|„CampusX (Aplikacja do zarządzania wydarzeniami studenckimi)”|
|2. Cel projektu|Co projekt ma osiągnąć i dlaczego|„Umożliwienie tworzenia, rezerwacji i wyszukiwania przez studentów ”
|3. Uzasadnienie biznesowe / edukacyjne|Dlaczego projekt jest potrzebny|„Obecnie rezerwacje odbywają się e-mailowo. System poprawi efektywność i przejrzystość procesu.”|
|4. Zakres projektu|Co wchodzi w zakres i co jest poza zakresem|„W zakresie: rezerwacja, kalendarz,tworzenie wydarzeń ; poza zakresem: integracja z systemem facebook, powiadomienia ”|
|5. Główne wymagania|Wstępna lista funkcjonalności|„Użytkownik może wyszukać wydarzenia, dokonać potwierdzenia duczestnicwa (rezerwacji), tworzenie wydarzeń”|
|6. Zespół projektowy i role|Lista członków i ich funkcji|„Kierownik – A. Myśliwec, Analityk\Tester – P. Dąbrowski, Backendowiec – K. Dęga, Frontendowiec - A. Myśliwiec ”|
|7. Zasoby i narzędzia|Technologie, środowisko, repozytorium, narzędzia komunikacji|„GitHub, Miro, Java, Spring Boot, HTMLL\CSS, PostgreSQL.”|
|8. Harmonogram wstępny|Etapy realizacji projektu|„Analiza wymagań (1–2 tydz.), Projektowanie (3–4 tydz.), Implementacja (5–7 tydz.), Testy (8 tydz.), Prezentacja (10 tydz.)”|
|9. Ryzyka i działania zapobiegawcze|Potencjalne zagrożenia i sposoby ich ograniczenia|„Brak komunikacji w zespole → okresowe spotkania online. Problemy z realizacją zadań → Pomoc zespołu/Praca wspólna.”|
|10. Oczekiwane rezultaty (produkty projektu)|Co powstanie na koniec|„Działający prototyp aplikacji + pełna dokumentacja projektowa.”|
|11. Kryteria sukcesu|Jak zostanie oceniony sukces projektu|„Aplikacja działa w przeglądarce, dokumentacja zawiera wszystkie diagramy UML.”|
|12. Akceptacja projektu|Podpisy|„Zatwierdza: prowadzący, kierownik projektu.”|


## KARTA PROJEKTU 
1. Informacje ogólne

Tytuł projektu:
CampusX (Aplikacja do zarządzania wydarzeniami studenckimi)

Data utworzenia: 19.10.2025
Wersja dokumentu: 1.0
Zespół projektowy:

Imię i nazwisko|Rola w projekcie|Zakres odpowiedzialności
----------------|------------------------------------------------|----------------------------------------------
Alan Myśliwiec|Kierownik projektu|Frontendowiec|Planowanie, koordynacja, raportowanie postępów, kontakt z prowadzącym, prezentacja końcowa, tworzenie interfejsu użytkowego (frontend)
Kacper Dęga|Programista|Implementacja backendu (Spring Boot), integracja z bazą danych, testy jednostkowe/integracyjne, tworzenie REST API
Paweł Dąbrowski|Tester manualny||Analityk systemowy|Dokumentalista|Analiza wymagań, tworzenie przypadków użycia, diagramów UML , testy manualne i tworzenia danych, Redakcja dokumentacji projektowej, tworzenie przypadków użycia, diagramów UML


Prowadzący: mgr Wojciech Moniuszko
Jednostka dydaktyczna: ??

2. Cel projektu

Celem projektu CampusX jest opracowanie i wdrożenie webowej aplikacji do zarządzania wydarzeniami studenckimi, umożliwiającej:

- studentom i wykładowcom szybkie tworzenie i promowanie wydarzeń,
- rezerwowanie terminów wydarzeń studenckich,
- rejeestrowanie uczestników wydarzeń
- przeglądanie kalendarza dostępności wydarzeń,
- Projekt ma służyć jako prototyp systemu społecznościowego dla studentów oraz uczelni, z potencjałem dalszego rozwoju.

3. Uzasadnienie projektu

Obecnie organizacja wydarzeń studenckich odbywa się głównie za pośrednictwem mediów społecznościowych lub komunikatorów, co prowadzi do:

- braku centralnego miejsca gromadzenia informacji o wydarzeniach,
- trudności w koordynacji zespołów organizacyjnych,
- niskiej frekwencji wynikającej z ograniczonego przepływu informacji,
- braku możliwości analizy i archiwizacji danych o wydarzeniach.

Projekt rozwiązuje te problemy poprzez stworzenie zintegrowanej aplikacji do zarządzania wydarzeniami studenckimi, umożliwiającej planowanie i monitorowanie wydarzeń w jednym systemie. Dzięki temu zwiększa się efektywność organizacji, przejrzystość komunikacji oraz zaangażowanie społeczności akademickiej.

4. Zakres projektu

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

5. Wymagania 

Typ | Opis
---------------------------|-----------------------------------------------------------------------------------


6. Projekt systemu (UML)

W celu zaprojektowania architektury systemu CampusX oraz zobrazowania jego działania wykorzystano notację UML (Unified Modeling Language). Diagramy UML umożliwiają przedstawienie procesów biznesowych, struktury danych oraz komunikacji pomiędzy komponentami systemu.

6.1 Diagram przypadków użycia

Diagram przypadków użycia przedstawia podstawowe funkcjonalności systemu CampusX oraz role użytkowników korzystających z aplikacji. Użytkownikami systemu są studenci, organizatorzy wydarzeń oraz administratorzy. Diagram ten umożliwia identyfikację głównych interakcji użytkowników z systemem oraz stanowi punkt wyjścia do dalszego projektowania systemu.

6.2 Diagram aktywności  

<img width="438" height="467" alt="diagram aktywności" src="https://github.com/user-attachments/assets/e7153b0e-8b60-4b92-b425-0b32c866303e" />

*(Proces tworzenia wydarzenia przez organizatora)*

Diagram aktywności przedstawia proces tworzenia wydarzenia przez organizatora w systemie CampusX. Proces rozpoczyna się w momencie otwarcia panelu organizatora i wybrania opcji „Utwórz wydarzenie”.

Następnie użytkownik wprowadza dane wydarzenia, takie jak nazwa, opis, data oraz lokalizacja. Równolegle system przeprowadza walidację pól formularza. W przypadku poprawnych danych następuje zapis wydarzenia w bazie danych oraz wyświetlenie komunikatu o pomyślnym zakończeniu operacji.

Jeżeli dane są niepoprawne, system informuje użytkownika o błędach formularza, umożliwiając ich poprawę. Proces kończy się po poprawnym zapisaniu wydarzenia lub po wyświetleniu komunikatu o błędach.

Diagram ilustruje zarówno przebieg główny procesu, jak i obsługę sytuacji wyjątkowych, co pozwala na pełne zrozumienie logiki procesu biznesowego.

6.3 Diagram klas  

<img width="384" height="506" alt="diagram klas" src="https://github.com/user-attachments/assets/afb802e6-46f7-4d47-ba17-4f09ca357fb2" />

*(Struktura danych systemu)*

Diagram klas przedstawia strukturę logiczną systemu CampusX oraz relacje pomiędzy głównymi obiektami domenowymi aplikacji.

Centralną klasą jest `User`, reprezentująca użytkownika systemu. Każdy użytkownik posiada przypisaną rolę (`UserRole`), która określa jego uprawnienia, takie jak STUDENT, ORGANIZATOR lub ADMIN.

Klasa `Event` opisuje wydarzenie tworzone przez organizatora i zawiera informacje takie jak tytuł, opis, data, lokalizacja oraz maksymalna liczba uczestników. Relacja pomiędzy klasami `User` i `Event` wskazuje, że jeden użytkownik może utworzyć wiele wydarzeń.

Klasa `Reservation` reprezentuje zapis użytkownika na wydarzenie. Umożliwia ona powiązanie konkretnego studenta z wybranym wydarzeniem oraz przechowuje informacje o czasie dokonania rezerwacji.

Diagram klas stanowi podstawę do implementacji relacyjnej bazy danych oraz warstwy backendowej aplikacji.

6.4 Diagram sekwencji  

<img width="679" height="414" alt="diagram sekwencji" src="https://github.com/user-attachments/assets/25f8cb94-9fe4-41d1-b993-b10fe9c3804c" />

*(Proces zapisu studenta na wydarzenie)*

Diagram sekwencji przedstawia proces zapisu studenta na wydarzenie w systemie CampusX oraz komunikację pomiędzy poszczególnymi warstwami aplikacji.

Proces rozpoczyna się w momencie, gdy student wybiera opcję „Zapisz się” w interfejsie użytkownika. Żądanie zapisu przesyłane jest z warstwy frontendowej do backendowego API w postaci zapytania HTTP.

Backend przetwarza żądanie, zapisuje dane rezerwacji w bazie danych oraz inicjuje wysłanie wiadomości e-mail z potwierdzeniem zapisu. Po pomyślnym wykonaniu operacji system zwraca odpowiedź do frontendu, który wyświetla użytkownikowi komunikat o sukcesie.

Diagram sekwencji obrazuje współpracę pomiędzy frontendem, backendem, bazą danych oraz systemem zewnętrznym.



7. Zespół projektowy i role

Rola|Osoba|Odpowiedzialność
--------------|-------------------------|-----------------------------------------------------------------------
Alan Myśliwiec|Kierownik projektu|Frontendowiec|Planowanie, koordynacja, raportowanie postępów, kontakt z prowadzącym, prezentacja końcowa, tworzenie interfejsu użytkowego (frontend)
Kacper Dęga|Programista|Implementacja backendu (Spring Boot), integracja z bazą danych, testy jednostkowe/integracyjne, tworzenie REST API
Paweł Dąbrowski|Tester manualny||Analityk systemowy|Dokumentalista|Analiza wymagań, tworzenie przypadków użycia, diagramów UML , testy manualne i tworzenia danych, Redakcja dokumentacji projektowej, tworzenie przypadków użycia, diagramów UML

8. Zasoby i narzędzia

Kategoria|Narzędzie / Technologia|Cel zastosowania
-----------------|-----------------------------------|----------------------------------------------------------
Zarządzanie projektem|GitHub Projekt|Planowanie sprintów, śledzenie zadań
Repozytorium|GitHub|Kontrola wersji kodu
Analiza i projektowanie, Miro|Diagramy UML, mapa procesu
Programowanie|Java (Spring Boot), HTML/CSS|Implementacja aplikacji
Baza danych|PostgreSQL|Przechowywanie danych o wydarzeniach i urzytkonikach
Dokumentacja|Word|Tworzenie dokumentacji technicznej
Komunikacja|Telegram, Discord|Spotkania zespołowe

9. Harmonogram realizacji (10 spotkań)

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

10. Analiza ryzyka

Nr|Ryzyko|Prawdopodobieństwo|Skutek|Działanie zapobiegawcze
--|---------------------------|-----------|-----------------------------------|---------------------------------
1|Opóźnienia w pracy zespołu|Średnie|Wysoki|Spotkania tygodniowe, śledzenie postępów w GitHub Projects
2|Brak doświadczenia w tworzeniu dokumentacji technicznej|Wysokie|Średni|Pomoc zespołu i szkolenie z  wykorzystaniem źródeł z internetu.
3|Konflikty w zespole|Niskie|Średni|Jasny podział ról, komunikacja na Discord
4|Utrata danych|Niskie|Wysoki|Regularne kopie oraz kontrola wersji w GitHub
5|Niedostateczna dokumentacja|Niskie|Wysoki|Wczesne rozpoczęcie opracowania przez dokumentalistę
6|Brak czasu|Średnie|Średnie|Wydłużenie deadline, ewentualne wsparcie zespołu w realizacji zadań

11. Kryteria sukcesu projektu

- Wszystkie wymagania funkcjonalne zostały zaimplementowane.
- Aplikacja uruchamia się lokalnie i działa poprawnie.
- Dokumentacja zawiera pełny zestaw diagramów UML.
- Testy zakończone wynikiem pozytywnym.
- Zespół zrealizował projekt w wyznaczonym czasie.
- Projekt został pozytywnie oceniony przez prowadzącego.

12. Rezultaty projektu

- Prototyp aplikacji webowej (CampusX).
- Dokumentacja projektowa (wymagania, UML, testy).
- Dokumentacja techniczna (instrukcja uruchomienia).
- Prezentacja zespołowa (PDF, prezentacja na żywo).
- Raport końcowy i protokół zdawczo-odbiorczy.

13. Akceptacja projektu

Funkcja|Imię i nazwisko|Data|Podpis
------------|-------------------------------|--------------|----------------------------------|
Kierownik projektu|Alan Myśliwec|19.10.2025|___________
Prowadzący|mgr Wojciech Moniuszko|19.10.2025|___________

## Uwagi końcowe:

- Dokument powinien być przechowywany w repozytorium projektu.
- Aktualizacja wersji dokumentu wymaga zgody kierownika projektu i prowadzącego.
- Każdy członek zespołu ma obowiązek zapoznać się z treścią karty i ją zaakceptować.





