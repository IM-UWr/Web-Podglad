# Podgląd nowego wyglądu strony IM UWr

Repozytorium **tylko do podglądu**. Nie ma tu kodu strony. Workflow `.github/workflows/podglad.yml` pobiera kod z
[IM-UWr/Web-Core](https://github.com/IM-UWr/Web-Core) (domyślnie gałąź `wyglad/zalozyciele`, kierunek „Założyciele”)
i prawdziwe treści z CMS (repozytoria IM-UWr/Web-*), buduje stronę i publikuje ją na GitHub Pages tego repozytorium.

- **Podgląd:** https://im-uwr.github.io/Web-Podglad/ (nowy wygląd tylko na komputerze, ≥ 761 px; na telefonie strona wygląda jak obecna).
- **Obecna strona** zostaje bez zmian: https://im-uwr.github.io/Web-Core/
- **Odświeżanie:** co godzinę, po zmianie workflow albo ręcznie (Actions → „Podgląd nowego wyglądu” → Run workflow; można podać inną gałąź Web-Core).
- Gałąź `zbudowana` zawiera ostatnią zbudowaną stronę (bez PDF-ów i dużych plików) — do zrzutów ekranu.
- Strona na github.io ma `noindex`, więc nie trafia do wyszukiwarek. Repozytorium można w każdej chwili usunąć bez skutków dla Web-Core.
