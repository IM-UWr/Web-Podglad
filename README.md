# Podgląd nowego wyglądu strony IM UWr

Repozytorium **tylko do podglądu**. Nie ma tu kodu strony. Workflow `.github/workflows/podglad.yml` pobiera kod z
[IM-UWr/Web-Core](https://github.com/IM-UWr/Web-Core) (domyślnie gałąź `wyglad/zlecenie-16`, kierunek „Założyciele”)
i prawdziwe treści z CMS (repozytoria IM-UWr/Web-*), buduje stronę i publikuje ją na GitHub Pages tego repozytorium.
Do treści z `main` dołącza gałąź `wyglad/zlecenie-16` repozytorium treści, jeśli ją ma: zmiany do oglądania leżą tylko tam,
bo z `main` repozytoriów treści buduje się obecna strona.

- **Podgląd:** https://im-uwr.github.io/Web-Podglad/ (nowy wygląd na komputerze i telefonie).
- **⚠️ TEST telefonu:** https://im-uwr.github.io/Web-Podglad/test-telefon/ — próbna wersja „Założycieli” na telefon
  (≤ 760 px), z plakietką „TEST · wersja na telefon”. To łatka `testy/telefon-TEST.patch` nakładana na tę samą gałąź
  tylko przy budowaniu podglądu. **Nie wzorować się, nie nakładać na Web-Core** — projekt telefonu nie jest ustalony.
  Gdy łatka przestanie się nakładać, główny podgląd publikuje się dalej, a w podsumowaniu workflow jest ostrzeżenie.
- **Obecna strona** zostaje bez zmian: https://im-uwr.github.io/Web-Core/
- **Odświeżanie:** co godzinę, po zmianie workflow albo ręcznie (Actions → „Podgląd nowego wyglądu” → Run workflow; można podać inną gałąź Web-Core).
- Gałąź `zbudowana` zawiera ostatnią zbudowaną stronę (bez PDF-ów i dużych plików) — do zrzutów ekranu.
- Strona na github.io ma `noindex`, więc nie trafia do wyszukiwarek. Repozytorium można w każdej chwili usunąć bez skutków dla Web-Core.
