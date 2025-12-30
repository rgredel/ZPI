# Instrukcja Konfiguracji Jira i Importu Backlogu

## Krok 1: Utworzenie Projektu
1.  Zaloguj się do Jira Software.
2.  Kliknij **Create project** (Utwórz projekt).
3.  Wybierz szablon: **Scrum**. Jest to kluczowe dla tego zadania (sprinty, backlog).
4.  Wybierz typ projektu: **Team-managed** (Zarządzany przez zespół) - jest prostszy w konfiguracji, LUB **Company-managed** (jeśli wolisz pełną kontrolę, ale polecam Team-managed dla szybkości).
5.  Nazwij projekt, np. **Intelligent LMS** i wpisz klucz (np. ILMS).

## Krok 2: Import Danych z CSV
1.  W górnym menu kliknij ikonę trzech kropek (lub "Filters") > **Advanced issue search**.
2.  W prawym górnym rogu kliknij ikonę trzech kropek (...) > **Import issues from CSV**.
3.  Wybierz plik `jira_import.csv`, który wygenerowałem.
4.  **Setup:**
    *   Zaznacz projekt, do którego chcesz importować.
    *   Delimiter: **Comma (,)**.
5.  **Mapowanie Pól (ważne!):**
    *   `Summary` -> **Summary** (PL: **Podsumowanie**)
    *   `Issue Type` -> **Issue Type** (PL: **Typ zgłoszenia**)
    *   `Description` -> **Description** (PL: **Opis**)
    *   `Story Points` -> **Story Points** (PL: **Punkty historyjki** lub czasem po prostu **Story Points**)
    *   `Issue Id` -> **Issue Id** (To pozwoli Jirze rozpoznać ID wiersza)
    *   `Parent Id` -> **Parent Id** (lub czasem **Parent** / **Element nadrzędny**) - *To pozwoli powiązać Story z Epic'iem po ID.*
 6.  Kliknij **Next** (Dalej), aby przejść do **Map Value** (Mapowanie Wartości).
7.  **Mapowanie Wartości (Kluczowe dla typu zgłoszeń!):**
    *   Upewnij się, że wartość `Epic` z pliku jest przypisana do typu **Epik** (lub Epic) w Jira.
    *   Upewnij się, że wartość `Story` z pliku jest przypisana do typu **Historyjka** (lub Story/Zadanie) w Jira.
    *   *Uwaga: Jeśli tego nie zrobisz, Jira utworzy wszystko jako domyślny typ (często Błąd/Bug).*
8.  Kliknij **Validate**, a potem **Begin Import**.

## Krok 3: Konfiguracja Widoków (Wymagania Zadania)

### Włączenie Epików i Roadmapy
W projektach *Team-managed*, niektóre funkcje mogą być domyślnie wyłączone:
1.  Wejdź w **Project settings** > **Features**.
2.  Upewnij się, że włączone są:
    *   **Roadmap** (Timeline) - to jest wymagany wykres Gantta dla Epików.
    *   **Backlog** - oddzielny widok planowania.
    *   **Reports** - przyda się do wykresów.

### Estymacja (Story Points)
Upewnij się, że na kartach zadań widać punkty:
1.  Wejdź w **Board settings** (lub Configure Board).
2.  W sekcji **Estimation**, wybierz **Story Points**.

## Krok 4: Organizacja Backlogu
Po imporcie, wszystkie zadania mogą trafić do Backlogu "luzem".
1.  Wejdź w zakładkę **Backlog**.
2.  Powinieneś widzieć panel **EPIC** (zwykle po lewej stronie, trzeba go rozwinąć).
3.  Przeciągnij odpowiednie historyjki (Story) do przypisanych im Epików ("Core Learning Experience" i "Management & Analytics").
    *   *To spełni wymóg struktury Epik -> Historyjka.*

## Krok 5: Roadmapa (Gantt)
1.  Wejdź w zakładkę **Timeline** (Oś czasu).
2.  Powinieneś widzieć swoje dwa Epiki.
3.  Rozciągnij paski epików w czasie, aby zaplanować je na osi (np. Core na miesiące 1-2, Management na miesiące 2-3).
