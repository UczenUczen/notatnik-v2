# Specyfikacja: Notatnik

## 1. Cel

Celem programu jest umożliwienie użytkownikowi tworzenia, zapisywania i odczytywania własnych notatek. Program ma zapewniać prosty dostęp do zapisanych informacji oraz zachowywać je po ponownym uruchomieniu.

## 2. Dla kogo

Program jest przeznaczony dla osób, które chcą szybko zapisywać i przechowywać własne notatki na komputerze, bez konieczności korzystania z Internetu lub zewnętrznych usług.

## 3. Co robi

- Umożliwia tworzenie notatek zawierających tytuł i treść.
- Zapisuje notatki w lokalnym pliku `notatki.md`.
- Przechowuje notatki w formacie Markdown.
- Zapisuje datę i godzinę utworzenia notatki.
- Umieszcza najnowsze notatki na początku pliku.
- Obsługuje polskie znaki.
- Odczytuje wcześniej zapisane notatki po ponownym uruchomieniu programu.
- Informuje użytkownika o błędach podczas zapisywania danych.

## 4. Czego nie robi

- Nie wysyła notatek ani innych danych użytkownika poza komputer.
- Nie wymaga połączenia z Internetem do podstawowego działania.
- Nie przechowuje notatek w zewnętrznych usługach ani w chmurze.
- Nie wymaga korzystania z konta użytkownika.

## 5. Kryteria akceptacji

### K1. Zapisywanie notatek

Kiedy użytkownik zapisuje notatkę z tytułem i treścią, to notatka zostaje dodana do lokalnego pliku `notatki.md`.

Sprawdzenie: utworzyć notatkę, zapisać ją i sprawdzić zawartość pliku.

### K2. Kolejność notatek

Kiedy użytkownik zapisze kilka notatek, to najnowsza notatka znajduje się na początku pliku.

Sprawdzenie: zapisać kilka notatek i sprawdzić ich kolejność w pliku.

### K3. Polskie znaki

Kiedy użytkownik zapisuje notatkę zawierającą polskie znaki, to po ponownym odczytaniu znaki pozostają poprawne.

Sprawdzenie: zapisać notatkę zawierającą znaki ą, ć, ę, ł, ń, ó, ś, ź i ż, a następnie ją odczytać.

### K4. Zachowanie danych

Kiedy użytkownik zamknie i ponownie uruchomi program, to wcześniej zapisane notatki nadal są dostępne.

Sprawdzenie: zapisać notatkę, zamknąć program, uruchomić go ponownie i sprawdzić, czy notatka jest dostępna.

### K5. Pusta notatka

Kiedy użytkownik próbuje zapisać notatkę bez tytułu lub bez treści, to program nie zapisuje jej do pliku.

Sprawdzenie: spróbować zapisać notatkę bez tytułu, a następnie bez treści, i sprawdzić, czy plik nie został zmieniony.

### K6. Błąd zapisu

Kiedy podczas zapisywania wystąpi błąd, to program informuje użytkownika o problemie w języku polskim i nie usuwa wcześniej zapisanych notatek.

Sprawdzenie: wywołać sytuację uniemożliwiającą zapis i sprawdzić komunikat oraz zawartość pliku.

### K7. Zablokowany plik

Kiedy plik `notatki.md` jest otwarty w innym programie i nie można go zmodyfikować, to Notatnik informuje o problemie i nie powoduje utraty danych.

Sprawdzenie: otworzyć plik w sposób uniemożliwiający jego zapis, spróbować zapisać notatkę i sprawdzić komunikat oraz zawartość pliku.

## 6. Do ustalenia

Na ten moment nie ma nierozstrzygniętych kwestii. Przyjęto, że każda zapisywana notatka musi mieć niepusty tytuł i treść, a błędy zapisu nie mogą powodować utraty wcześniejszych danych.