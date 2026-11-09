# AGENTS.md — reguły dla AI w tym vaulcie

> Zasada 0: w razie wątpliwości NIE kasuj i NIE przepisuj — zaproponuj i zapytaj.
> Claude: przeczytaj ten plik na początku każdej sesji z vaultem.

## Mapa
- `00-daily/` — jedna notatka na dzień (`RRRR-MM-DD`). Główny lejek: wszystko wpada tu najpierw.
- `10-projects/` — jeden projekt = jedna notatka (Cel / Następny krok / Log). Tylko to, co może być ZROBIONE.
- `20-areas/` — obszary bez daty końca (np. dział, klienci, procesy). Każdy obszar ma hub `_nazwa.md`.
- `30-resources/` — wiedza wielokrotnego użytku. `szablony/` i `prompts/` to maszyneria systemu.
- `40-archive/` — skończone i martwe, płasko. Zaglądaj tu dopiero, gdy nie ma w innych folderach.
- `Ideas/` — pomysły do przemyślenia (szablon `pomysl`). `Zadania/` — jedno zadanie = jedna notatka (szablon `zadanie`).
- Każdy folder ma `_o-tym-folderze.md`. Max 2 poziomy zagnieżdżenia.

## Twarde reguły
1. Jeden temat = jedno miejsce. Duplikat w 2+ folderach → zgłoś, zaproponuj scalenie.
2. Test: „może być ZROBIONE?” TAK → `10-projects/`, NIE → `20-areas/` (stały obszar) albo `30-resources/` (wiedza).
3. Płasko > głęboko. Linki `[[wikilink]]` zamiast folderów.
4. Nazwy plików: małe litery, myślniki, bez polskich znaków, daty ISO (`2026-11-09`). Wyjątki: `AGENTS`, `README`.
5. Pod nagłówkiem `## Moje` nie edytujesz i nie kasujesz. Nigdy — to strefa człowieka.
6. Nie kasuj bez zgody. Archiwizuj (`40-archive/` albo `Zadania/_archiwum/`).
7. Nowa notatka: najpierw sprawdź, czy istnieje już taka (szukaj po sensie i słowach kluczowych). Istniejąca wygrywa z nową.
8. Dane firmowe wrażliwe (dane osobowe, ceny klientów, umowy): nie wklejaj do notatek, jeśli polityka firmy tego zabrania. Pytaj.

## Słowniki
- Statusy zadań: `todo → w-trakcie → oczekuje → zrobione → archiwum`. Przy `zrobione` przenieś notatkę do `Zadania/_archiwum/`.
- Statusy pomysłów: `parked → planned → building → live | shelved`.
- Pole `waga:` zadania: `1`–`3` (3 = ważne i pilne, 2 = ważne nie pilne, 1 = najmniej ważne), puste = bez wagi.
- Frontmatter zadań i pomysłów ma być 1:1 z szablonami w `30-resources/szablony/`. Brak `typ:` lub status spoza słownika = notatka wypada z przeglądów.

## Workflowy
Kroki w `30-resources/prompts/`: `daily-review.md` (co tydzień), `weekly.md` (piątek), `lint.md` (na żądanie, tylko raport).
Użytkownik mówi np. „zrób daily-review” → otwórz ten plik i wykonaj kroki.

## Styl odpowiedzi
Krótko, po polsku, najpierw wynik. Po większej robocie: co działa (3–5 linii) + jedna następna akcja.
