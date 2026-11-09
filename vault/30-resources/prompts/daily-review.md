# daily-review — porządek w notatkach dziennych (co tydzień)

Trzymaj się `AGENTS.md`. Cel: po przeglądzie w `00-daily/` nie zostaje nic nieprzetworzonego — każda rzecz ma jeden dom.

## Zakres
- Pliki `00-daily/RRRR-MM-DD.md` w korzeniu folderu (podfoldery `RRRR-MM/` to archiwum — pomiń).
- Pomijaj puste punkty (`- `), przetworzone (`<!-- przeniesione ... -->`, `<!-- odrzucone ... -->`) i WSZYSTKO pod `## Moje`.

## Kroki
1. **Zbierz (tylko czytanie).** Przeczytaj pliki z zakresu. Podaj jedną linię: „X dni, Y rzeczy: Z zadań, P pomysłów, Ł luźnych”. Nic nie ma → powiedz i skończ.
2. **Sekcja `Zadania` → `Zadania/`.** Dla każdego punktu: sprawdź, czy takie zadanie już istnieje (szukaj w `Zadania/`). Jest → nie dubluj. Nie ma → nowa notatka wg szablonu `zadanie` (krótki tytuł, 1–3 zdania, `projekt:` jeśli pasuje).
3. **Sekcja `Pomysły`.** Wypisz ponumerowane (pełna treść). Dla każdego zapytaj: `Ideas` (zaparkuj) / `Zadanie` / `Odrzuć` / `Zostaw`. Zapisuj dopiero po odpowiedzi. `Ideas` → notatka wg szablonu `pomysl`.
4. **Sekcja `Łap tu wszystko`.** Oceń każdą rzecz: zadanie → jak w kroku 2; pomysł → jak w kroku 3; wiedza/informacja → najpierw szukaj istniejącej notatki i dopisz do niej (NAD `## Moje`); brak pasującej → nowa notatka w miejscu wg `AGENTS.md` (reguła 2) + link do huba; śmieć → tylko propozycja w raporcie. Niepewny między dwiema notatkami → zapytaj, nie zgaduj.
5. **Oznacz w dailym.** Przeniesione: `<!-- przeniesione RRRR-MM-DD: [[cel]] -->`. Odrzucone: `<!-- odrzucone RRRR-MM-DD: pierwsze słowa… -->`.
6. **Archiwum miesięcy.** Dailies z zakończonych miesięcy, w których nic nie zostało, przenieś do `00-daily/RRRR-MM/`.
7. **Log i raport.** W dzisiejszym dailym NAD `## Moje` dopisz `## Log daily-review` (max 5 linii z linkami). W czacie: jedna linia z liczbami, lista „rzecz → gdzie”, propozycje do kosza, jedna następna akcja.

## Zakazy
Nic nie kasuj. Nic nie edytuj pod `## Moje`.
