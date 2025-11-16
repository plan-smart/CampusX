

---

# **Moduł 2: Analiza wymagań – CampusX**

## **Plan modułu 2**

* Analiza wymagań dla aplikacji CampusX
* Warsztat: identyfikacja interesariuszy – role i potrzeby
* Przygotowanie listy wymagań funkcjonalnych
* Warsztat: stworzenie przypadków użycia (Use Case Diagram)
* Opis wymagań niefunkcjonalnych
* Prezentacja przygotowanych dokumentów
* Podsumowanie i refleksja

**Efekt końcowy modułu:**
📄 **Dokument: Specyfikacja wymagań funkcjonalnych i niefunkcjonalnych CampusX**

---

# **1. Analiza wymagań – wprowadzenie**

### **Czym jest analiza wymagań?**

To proces odkrywania, dokumentowania i uzgadniania:

* **co system ma robić** → wymagania funkcjonalne
* **jak ma działać** → wymagania niefunkcjonalne

Celem jest zminimalizowanie ryzyka nieporozumień i zapewnienie, że projekt odpowiada na realne potrzeby użytkowników.

### **Dlaczego to ważne?**

* Błędy na etapie wymagań są najdroższe do naprawienia.
* Precyzyjne wymagania → prostsza implementacja + szybsze testowanie.
* Wspólne zrozumienie systemu przez cały zespół.

---

# **2. Etapy analizy wymagań w projekcie CampusX**

1. **Identyfikacja interesariuszy**
   Określenie użytkowników systemu i ich potrzeb.
2. **Zbieranie wymagań**
   Wywiady, burza mózgów, analiza obecnych procesów.
3. **Dokumentacja**
   Lista wymagań, diagramy przypadków użycia, user stories.
4. **Walidacja**
   Czy wymagania są kompletne, spójne i możliwe do realizacji.

---

# **3. Interesariusze CampusX**

## **3.1 Lista ról (aktorów)**

| Interesariusz                                                   | Opis roli                                   | Główne potrzeby                                                           |
| --------------------------------------------------------------- | ------------------------------------------- | ------------------------------------------------------------------------- |
| **Student**                                                     | Uczestnik wydarzeń, twórca prostych eventów | Szybkie wyszukiwanie wydarzeń, możliwość rejestracji i zgłaszania udziału |
| **Organizator wydarzenia** (koła naukowe, samorząd, wykładowcy) | Tworzenie i zarządzanie wydarzeniami        | Formularz tworzenia wydarzeń, lista zapisów, edycja terminów              |
| **Administrator systemu**                                       | Zarządzanie użytkownikami i bezpieczeństwem | Dane logów, kontrola błędów, panel admina                                 |
| **Dyrekcja / uczelnia**                                         | Nadzorowanie aktywności i statystyk         | Raporty uczestnictwa, przegląd frekwencji                                 |
| **System e-mail (zewnętrzny)**                                  | Wysyłanie powiadomień                       | Integracja do wysyłania potwierdzeń                                       |

## **3.2 Priorytety potrzeb**

* **Must Have:** wyszukiwanie wydarzeń, tworzenie wydarzeń, rezerwacje udziału
* **Should Have:** edycja wydarzeń, filtrowanie, proste powiadomienia
* **Could Have:** statystyki, integracja z kalendarzami
* **Won’t Have:** integracje z mediami społecznościowymi (poza zakresem)

---

# **4. Wymagania funkcjonalne CampusX**

Poniższa tabela przedstawia główne funkcjonalności w formie klasycznej specyfikacji.

## **4.1 Tabela wymagań funkcjonalnych**

| ID  | Opis wymagania                                                | Priorytet | Źródło              |
| --- | ------------------------------------------------------------- | --------- | ------------------- |
| F1  | Użytkownik może się zarejestrować i zalogować do systemu      | Must      | Student             |
| F2  | Użytkownik może przeglądać listę wszystkich wydarzeń          | Must      | Student             |
| F3  | Użytkownik może filtrować wydarzenia (data, tagi, miejsce)    | Should    | Student             |
| F4  | Użytkownik może wyświetlić szczegóły wydarzenia               | Must      | Student             |
| F5  | Użytkownik może zapisać się na wydarzenie                     | Must      | Student             |
| F6  | Organizator może utworzyć nowe wydarzenie                     | Must      | Organizator         |
| F7  | Organizator może edytować i usuwać własne wydarzenia          | Should    | Organizator         |
| F8  | System wysyła powiadomienie potwierdzające rezerwację         | Should    | Student             |
| F9  | Administrator może zarządzać użytkownikami i rolami           | Could     | Admin               |
| F10 | System wyświetla kalendarz wydarzeń                           | Must      | Student/Organizator |
| F11 | System generuje raporty o frekwencji                          | Could     | Dyrekcja            |
| F12 | Użytkownik może zobaczyć listę wydarzeń, na które się zapisał | Must      | Student             |

---

# **5. User Stories (podejście zwinne)**

* **Jako student chcę wyszukać wydarzenia po nazwie, aby szybko znaleźć interesujące mnie wydarzenia.**
* **Jako student chcę zapisać się na wydarzenie, aby potwierdzić udział.**
* **Jako organizator chcę tworzyć wydarzenia, aby przekazywać informacje studentom.**
* **Jako organizator chcę edytować wydarzenie, aby poprawić szczegóły.**
* **Jako administrator chcę zarządzać użytkownikami, aby utrzymać bezpieczeństwo systemu.**
* **Jako dyrekcja chcę widzieć raporty uczestnictwa, aby analizować aktywność studentów.**

---

# **6. Przypadki użycia (Use Case)**

## **6.1 Główne przypadki użycia**

### **UC1 – Wyszukiwanie wydarzeń**

* **Aktor:** Student
* **Warunek początkowy:** Użytkownik na stronie głównej
* **Scenariusz:**

  1. Student wpisuje słowo kluczowe.
  2. System wyświetla pasujące wydarzenia.
  3. Student wybiera wydarzenie.

### **UC2 – Tworzenie wydarzenia**

* **Aktor:** Organizator
* **Warunek początkowy:** Organizator jest zalogowany
* **Scenariusz:**

  1. Organizator wybiera „Utwórz wydarzenie”.
  2. Wypełnia formularz.
  3. System zapisuje wydarzenie i publikuje je.

### **UC3 – Rezerwacja udziału**

* **Aktor:** Student
* **Scenariusz:**

  1. Student otwiera wydarzenie.
  2. Kliknięcie „Zapisz się”.
  3. System potwierdza zapis i wysyła e-mail.

### **UC4 – Zarządzanie użytkownikami**

* **Aktor:** Administrator
* **Scenariusz:**

  1. Admin otwiera panel zarządzania.
  2. Wyświetla listę użytkowników.
  3. Dodaje/usuwa/zmienia rolę użytkownika.

## **6.2 Opisowy diagram przypadków użycia (tekstowy)**

System: **CampusX**

Aktorzy:

* Student
* Organizator
* Administrator
* System e-mail

Przypadki użycia:

* „Przeglądaj wydarzenia”
* „Wyszukaj wydarzenie”
* „Zapisz się na wydarzenie”
* „Twórz wydarzenie”
* „Edytuj wydarzenie”
* „Usuń wydarzenie”
* „Zarządzaj użytkownikami”
* „Generuj raporty”
* „Wyświetl kalendarz”

Relacje:

* „Zapisz się na wydarzenie” **include** „Wyślij e-mail potwierdzający”
* „Twórz wydarzenie” **extend** „Dodaj tagi”
* „Przeglądaj wydarzenia” **include** „Filtruj”

---

# **7. Wymagania niefunkcjonalne CampusX**

## **7.1 Kategorie i przykłady**

### **Bezpieczeństwo**

* System szyfruje dane (SSL/TLS).
* Dostęp do panelu organizatora i admina wymaga zalogowania.
* Role użytkowników definiują dostęp do funkcji.
* System spełnia standardy RODO.

### **Wydajność**

* Czas odpowiedzi < 2 sekundy przy obciążeniu 50 użytkowników.
* Obsługa minimum 200 równoczesnych zapytań.
* Optymalizacja zapytań do bazy.

### **Dostępność**

* Dostępność systemu: **min. 99%** podczas testów.
* Aplikacja działa w przeglądarkach Chrome/Firefox/Edge.
* Stałe monitorowanie błędów.

### **Użyteczność**

* Intuicyjny interfejs zgodny z podstawowymi zasadami UX.
* Kolorystyka i rozmieszczenie elementów dostosowane do urządzeń laptopowych.
* Formularze walidują dane i wyświetlają czytelne komunikaty.

### **Integracje**

* Integracja SMTP do wysyłki e-maili.
* API REST do komunikacji front–backend.

## **7.2 Checklist wymagań niefunkcjonalnych**

🔒 **Bezpieczeństwo**
✔ HTTPS
✔ Role i uprawnienia
✔ Logi zdarzeń
✔ RODO

⚡ **Wydajność**
✔ Czas odpowiedzi
✔ Liczba użytkowników
✔ Testy obciążeniowe

🌐 **Dostępność**
✔ Obsługa głównych przeglądarek
✔ Stabilność działania

🎨 **Użyteczność**
✔ Przejrzysty UI
✔ Walidacja pól

🔄 **Integracja**
✔ E-mail
✔ REST API

---

# **8. Podsumowanie modułu**

Po przejściu modułu zespół projektowy posiada:

* pełną listę wymagań funkcjonalnych CampusX,
* szczegółowe wymagania niefunkcjonalne,
* zdefiniowanych interesariuszy i ich potrzeby,
* user stories,
* opis przypadków użycia,
* podstawę do stworzenia diagramów UML.

Dokument stanowi fundament do dalszych etapów: projektowania, implementacji i testowania.

---


