# Podgląd nowego wyglądu strony IM UWr

Repozytorium **tylko do podglądu**. Nie ma tu kodu strony. Workflow `.github/workflows/podglad.yml` pobiera kod z
[IM-UWr/Web-Core](https://github.com/IM-UWr/Web-Core) (gałąź `main`, kierunek „Założyciele”) i prawdziwe treści z CMS
(gałąź `main` repozytoriów IM-UWr/Web-*), buduje stronę i publikuje ją na GitHub Pages tego repozytorium. Od 7.11.2026
budowanie w Web-Core (`deploy.yml`) jest wyłączone; stan sprzed scalenia nowego wyglądu: znacznik `archiwum/2026-11-07-main`.

- **Podgląd:** https://im-uwr.github.io/Web-Podglad/ (nowy wygląd na komputerze i telefonie).
- **Stara strona** (ostatnia publikacja z Web-Core, już się nie przebudowuje): https://im-uwr.github.io/Web-Core/
- **Odświeżanie:** po zmianie treści w CMS, po nowym planie zajęć i po pushu kodu na `main` Web-Core (sygnał z Web-Core,
  `podglad-przekaznik.yml`), co godzinę, po zmianie workflow albo ręcznie (Actions → „Podgląd nowego wyglądu” → Run workflow;
  można podać inną gałąź Web-Core). Nowe uruchomienie przerywa budowę w toku (stan „cancelled”), więc seria zapisów w CMS
  daje jedną budowę z ostatnim zapisem; publikacja nie jest przerywana.
- **Czas budowy:** pakiety npm i zoptymalizowane zdjęcia są w pamięci podręcznej Actions, więc zdjęcia optymalizują się
  od nowa tylko po ich zmianie.
- Gałąź `zbudowana` zawiera ostatnią zbudowaną stronę (bez PDF-ów i dużych plików) — do zrzutów ekranu.
- Strona na github.io ma `noindex`, więc nie trafia do wyszukiwarek. Repozytorium można w każdej chwili usunąć bez skutków dla Web-Core.
