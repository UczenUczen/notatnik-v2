# 0001 — Format pliku z notatkami

Kontekst: notatki muszą dać się otworzyć w każdym edytorze (konstytucja,
pkt 2). W Budowie 2 porównano pięć wariantów tej samej prośby; najlepiej
czytelny okazał się Markdown z nagłówkiem na każdą notatkę.

Decyzja: jeden plik `notatki.md`, każda notatka jako nagłówek `##` z datą,
godziną i tytułem, treść pod nagłówkiem, najnowsza notatka na górze.

Odrzucone: JSON — czytelny dla programu, nie dla człowieka w edytorze;
jeden plik na notatkę — folder zamienia się w bałagan po tygodniu.

Skutki: format da się sprawdzić gołym okiem; „najnowsza na górze” wymaga
przepisania całego pliku przy każdym zapisie, co trzeba wpisać do kryteriów.