# Zadanie 3: Planowanie Projektu i Symulacja Sprintu (Grupowe)

## Cel zadania

Celem zadania jest transformacja wymagań zdefiniowanych w dokumencie SRS na strukturę zadań w narzędziu typu Jira. Studenci wcielają się w rolę zespołu Scrumowego, który musi przygotować Product Backlog, zaplanować harmonogram prac (roadmapę) na jeden semestr (MVP) oraz szczegółowo przygotować się do realizacji pierwszego sprintu.

Zadanie ma na celu symulację rzeczywistego procesu planowania w metodykach zwinnych, z naciskiem na strukturę epik -> historyjka, priorytetyzację oraz szacowanie pracochłonności.

---

## Część A: Backlog Produktów i Roadmapa

Wymaganiem wstępnym jest posiadanie dokumentu SRS stworzonego w ramach **Zadania 2**. 
Waszym zadaniem jest przekształcenie tego statycznego dokumentu wymagań w dynamiczny rejestr zadań (backlog) w narzędziu Jira. Jeśli Wasz SRS z Zadania 2 wymaga poprawek, należy je uwzględnić przed rozpoczęciem pracy w Jira.

### 1. Tworzenie Backlogu Produktu
Zbudujcie hierarchię zadań odzwierciedlającą cele biznesowe:
*   **Epiki:** Zdefiniujcie główne obszary funkcjonalne lub cele biznesowe.
*   **Historyjki Użytkownika:** Rozbijcie Epiki na konkretne historyjki.
    *   **Wymagane:** Każdy student w zespole musi przygotować **szczegółowe opisy dla minimum dwóch Historyjek Użytkownika**.
    *   **Format szczegółowego opisu:**
        *   **Tytuł:** Jasny i zwięzły.
        *   **Opis:** Opis wymagań historyjki.
        *   **User Story:** *"Jako [rola], chcę [akcja], aby [korzyść]"*.        
        *   **Kryteria Akceptacji:** Lista warunków, które muszą być spełnione, aby uznać zadanie za wykonane (Definition of Done dla konkretnego zadania).
        *   **Priorytet:** np. High/Medium/Low.
        *   **Szacowanie:** Story Points (ciąg Fibonacciego).
        *   **Refinement:** Opisz co w ramach tej historyjki należy wykonać pod względem technicznym lub orgranizacyjnym.
    *   **Pozostałe historyjki:** Reszta zadań w Backlogu (poza tymi dwoma wybranymi) może być pusta (zawierać tylko tytuł), ale **musi mieć nadany priorytet**.
*   **Zadania:** Dla prac technicznych umożliwiających np. realizację atrybutów jakościowych.

#### Uwaga: 
Planujecie prace na **maksymalnie 3 miesiące**.
*   Nie musicie (i nie powinniście) planować realizacji całego systemu opisanego w SRS, jeśli jest on zbyt duży.
*   Wybierzcie kluczowe funkcjonalności (**MVP**), które dostarczą największą wartość biznesową i są możliwe do zrealizowania w tym czasie.

### 2. Oś czasy
Stwórzcie wizualizację planu w czasie.
*   **Wizualizacja na osi czasu (wykres Gantta):** Dotyczy **WYŁĄCZNIE Epików**.
*   Nie twórzcie wykresu Gantta dla pojedynczych historyjek.
*   Roadmapa ma pokazywać, w jakiej kolejności i w jakich ramach czasowych planujecie dostarczyć poszczególne Epiki.

---

## Część B: Planowanie Sprintu 1

Zaplanujcie szczegółowo pierwszy sprint. Zakładamy, że sprint trwa **2 tygodnie**.
**Założenie:** Pierwszy sprint poświęcamy na przygotowanie **PoC (Proof of Concept)** kluczowej funkcjonalności.

### Proof of Concept
**Opis:** Technika pozwalająca na weryfikację hipotez dotyczących wykonalności pomysłu lub rozwiązania poprzez stworzenie minimalnego, działającego prototypu. Skupia się na sprawdzeniu, czy dana koncepcja jest technicznie możliwa do zrealizowania, zanim zainwestuje się więcej zasobów w pełny rozwój.

**Uwaga: Każda grupa musi skonsultować swój pomysł na PoC z prowadzącym.**

**Kroki:**
1.  Sformułowanie jasnej hipotezy do zweryfikowania (co chcemy sprawdzić?)
2.  Określenie kluczowych parametrów i kryteriów sukcesu dla eksperymentu
3.  Zbudowanie minimalnego prototypu skupionego tylko na testowanej funkcjonalności. **Uwaga: PoC wymaga realnego działania technicznego, a nie tylko planu.** - w ramach tego zadania ogarniczcie się jednak jedynie do opisania ogólnej koncpecji implementacji. 
4.  Przeprowadzenie eksperymentu i zebranie danych - w ramach tego zadania ogarniczcie się jedynie do opisu eksperymentu. 
5.  Analiza wyników i podjęcie decyzji o dalszych krokach - krótko opiszcie możliwe scenariusze i decyzje, które możecie podjąć.

### 1. Cel Sprintu
Zdefiniujcie jasny, biznesowy cel dla tego sprintu. Cel musi być **SMART**. Cel musi być realizowalny w trakicie jednego sprintu!

### 2. Backlog Sprintu i Szacowanie
Wybierzcie zadania z Product Backlogu, które zrealizujecie w tym sprincie.
*   Zespół musi oszacować pracochłonność wybranych zadań.
*   Wykorzystajcie **ciąg Fibonacciego** (1, 2, 3, 5, 8, 13, 21) jako Story Points.

### 3. Definition of Done (DoD)
Zdefiniujcie "definicję ukończenia". Są to uniwersalne kryteria jakościowe, które muszą zostać spełnione dla **każdego** elementu Backlogu, aby uznać go za zakończony.

### 4. Analiza Pre-Mortem
**Opis:** Technika pozwalająca na identyfikację potencjalnych problemów przed rozpoczęciem pracy. **W ramach tego zadania należy skupić się na analizowanej PoCa (nie całym projekcie). Analiza musi uwzględniać aspekty bezpieczeństwa lub konsekwencje niedostarczenia rozwiązania (co jeśli okaże się, że nie da się tego zrealizować w zakładany sposób).**

**Kroki wdrożenia:**
1.  Zespół wyobraża sobie, że **wdrożenie analizowanej funkcjonalności** zakończyło się niepowodzeniem (np. wystąpił incydent bezpieczeństwa lub rozwiązanie okazało się niewykonalne) 
2.  Każda osoba indywidualnie identyfikuje możliwe przyczyny tej konkretnej porażki 
3.  Zespół wspólnie omawia zidentyfikowane zagrożenia dla tej funkcjonalności 
4.  Opracowanie planu zapobiegawczego dla kluczowych zagrożeń 

---

## Narzędzia

Do realizacji zadania musicie wykorzystać narzędzie **Jira** (lub tożsame). 
*   W sprawozdaniu należy umieścić zrzuty ekranu (screenshoty) z narzędzia, pokazujące skonfigurowany backlog (z podziałem na epiki), roadmapę oraz tablicę sprintu.

---

## Forma i sposób oddania

*   **Format:** Jeden plik PDF (sprawozdanie) + Link do projektu w Jira.
*   **Termin:** Zgodnie z harmonogramem zajęć.

---

## Kryteria oceny

Maksymalna liczba punktów do zdobycia wynosi **50**.

### Część A: Product Backlog i Roadmapa (25 pkt)

| Elementy podlegające ocenie | Maks. punkty | Opis kryterium |
| :--- | :---: | :--- |
| **1. Product Backlog i MVP** | **10** | Poprawna hierarchia zadań (epiki, historyjki), sensowny zakres MVP (max 4 m-ce). |
| **2. Roadmapa Projektu** | **5** | Wizualizacja planu (epiki w czasie). |
| **3. Jakość Historyjek Użytkownika** | **10** | Szczegółowe opisy (dwa per student/studentka), poprawne user story, weryfikowalne kryteria akceptacji. |
| **SUMA CZĘŚCI A** | **25** | |

### Część B: Planowanie Sprintu 1 (25 pkt)

| Elementy podlegające ocenie | Maks. punkty | Opis kryterium |
| :--- | :---: | :--- |
| **1. Proof of Concept** | **10** | Hipoteza, wnioski i decyzje. |
| **2. Planowanie Sprintu 1** | **10** | Cel, backlog sprintu, definition of done |
| **3. Ryzyko** | **5** | Analiza Pre-Mortem. |
| **SUMA CZĘŚCI B** | **25** | |

**SUMA CAŁKOWITA: 50 pkt**