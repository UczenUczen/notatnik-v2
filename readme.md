# Notatnik-v2 — klasyfikacja zasad projektu

## 1. Plik reguł (AGENTS.md)

- Metoda nie może być dłuższa niż dwadzieścia linii.
- Nie zmieniaj plików, o które nie było prośby.
- Wszystkie pliki w UTF-8.

## 2. Specyfikacja

- Kiedy tytuł notatki jest pusty, przycisk zapisu jest nieaktywny.
- Notatki sortujemy od najnowszej.
- Program uruchamia się w mniej niż dwie sekundy.

## 3. Konstytucja

- Program jest dla jednej osoby na jednym komputerze.
- Dane nigdy nie opuszczają komputera użytkownika.
- Program nie wymaga połączenia z internetem.
- Komunikaty o błędach są po polsku.

## 4. Zapis decyzji

- Wybraliśmy Markdown zamiast JSON, bo plik ma być czytelny w edytorze.
- Zrezygnowaliśmy z wyszukiwania w tej wersji, bo wydłużyłoby tydzień o drugi.

## 5. Zdania dwuznaczne — wyjaśnienie

**Komunikaty o błędach są po polsku.**

Jeżeli dotyczy to wszystkich komunikatów w całym programie, jest to zasada konstytucji. Jeżeli dotyczy konkretnej funkcji, należy umieścić ją w specyfikacji.

**Program nie wymaga połączenia z internetem.**

Jeżeli jest to niezmienna zasada dotycząca całego programu, należy umieścić ją w konstytucji. Jeżeli dotyczy tylko konkretnej funkcji, należy umieścić ją w specyfikacji.

## 6. Zasada z konstytucji Spec Kit

Źródło: https://github.com/github/spec-kit/blob/main/templates/constitution-template.md

Data odczytania: 26.11.2026

Jedna z zasad szablonu mówi, że konstytucja jest nadrzędna wobec pozostałych praktyk i dokumentów projektu.

Dla Notatnika rozbudowana konstytucja z wieloma artykułami byłaby niepotrzebna, ponieważ jest to niewielka aplikacja do zapisywania notatek. Wystarczy kilka jasnych i konkretnych zasad.
## 7. Kryteria akceptacji — pięć wymagań

### 1. Obsługa polskich znaków
Kiedy użytkownik zapisuje notatkę zawierającą polskie znaki, to po ponownym odczytaniu znaki są wyświetlane poprawnie.

Sprawdzenie: zapisać notatkę zawierającą znaki ą, ę, ć, ł, ń, ó, ś, ź, ż, a następnie sprawdzić jej treść.

### 2. Aktualność listy notatek
Kiedy użytkownik zapisuje nową notatkę, to lista notatek uwzględnia ją bez konieczności ponownego uruchamiania programu.

Sprawdzenie: zapisać nową notatkę i sprawdzić, czy pojawia się na liście.

### 3. Bezpieczny zapis
Kiedy zapis notatki kończy się błędem, to program informuje użytkownika o problemie i nie usuwa wcześniej zapisanych notatek.

Sprawdzenie: wywołać błąd zapisu i sprawdzić komunikat oraz zawartość pliku.

### 4. Niezapisywanie pustych notatek
Kiedy użytkownik próbuje zapisać notatkę bez tytułu lub bez treści, to program odrzuca zapis.

Sprawdzenie: spróbować zapisać notatkę bez tytułu, a następnie bez treści.

### 5. Działanie po ponownym uruchomieniu
Kiedy użytkownik zamknie i ponownie uruchomi program, to wcześniej zapisane notatki są nadal dostępne.

Sprawdzenie: zapisać notatkę, zamknąć program i uruchomić go ponownie.

## 8. Przykładowy prompt — podział na cztery dokumenty

Na potrzeby ćwiczenia przygotowano przykładowy prompt opisujący program Notatnik.

**Treść promptu:**

„Stwórz prosty program Notatnik dla jednej osoby, działający na jednym komputerze. Program ma umożliwiać tworzenie i zapisywanie notatek w pliku Markdown. Notatki powinny być wyświetlane od najnowszej. Program ma obsługiwać polskie znaki, działać bez internetu i informować użytkownika o błędach po polsku. Puste notatki nie powinny być zapisywane. Dane użytkownika nie mogą opuszczać jego komputera.”

**Podział treści promptu:**

- **Konstytucja (`konstytucja.md`):** program jest przeznaczony dla jednej osoby, działa lokalnie, nie wysyła danych poza komputer i nie wymaga internetu.
- **Specyfikacja (`spec.md`):** program umożliwia tworzenie i zapisywanie notatek, obsługuje polskie znaki, sortuje notatki od najnowszej i nie zapisuje pustych notatek.
- **Plan (`plan.md`):** opisuje sposób realizacji programu, potrzebne pliki i kolejność prac.
- **Zadania (`tasks.md`):** zawiera konkretne kroki implementacji i sprawdzenia ich wykonania.

**Wniosek dotyczący brakującego dokumentu:**

W przykładowym promptcie zabrakło szczegółowego planu realizacji. Bez niego wykonawca musi samodzielnie zdecydować o strukturze plików i kolejności prac, co może prowadzić do niepotrzebnych zmian i dodatkowej pracy.