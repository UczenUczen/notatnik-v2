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