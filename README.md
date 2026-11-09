# Cellfast vault — szkielet systemu Obsidian + Claude Desktop

Sam szkielet i sposób działania. Zero treści. Folder `vault/` to gotowy, pusty vault.

## Jak to działa (w skrócie)
1. **Łapiesz** wszystko do notatki dziennej `00-daily/` (sekcje: Łap tu wszystko / Zadania / Pomysły).
2. **Raz w tygodniu** mówisz Claude'owi „zrób daily-review" — rozkłada rzeczy do `Zadania/`, `Ideas/`, `20-areas/` itd.
3. **Struktura PARA:** projekty (do zrobienia) / obszary (stałe) / zasoby (wiedza) / archiwum.
4. **Claude** czyta i pisze w vaulcie przez MCP. Reguły gry: `vault/AGENTS.md`. Workflowy: `vault/30-resources/prompts/`.

## Instalacja (Windows, ok. 15 min)
1. Zainstaluj **Obsidian**, **Claude Desktop** i **Node.js** (LTS).
2. Skopiuj zawartość folderu `vault/` do nowego folderu, np. `C:\Users\TY\Documents\VaultPraca` (razem z ukrytym `.obsidian`).
3. Obsidian → „Open folder as vault" → wybierz ten folder. Notatka dzienna ma się tworzyć z szablonem.
4. Połącz z Claude Desktop — wybierz JEDNĄ drogę:
   - **A (prostsza, zalecana na start):** `claude_desktop_config.filesystem.json`. Obsidian nie musi być włączony, Claude widzi zwykłe pliki.
   - **B (pełniejsza):** w Obsidianie zainstaluj plugin „Local REST API with MCP", skopiuj klucz, zapisz certyfikat z `https://127.0.0.1:27124/obsidian-local-rest-api.crt`, użyj `claude_desktop_config.obsidian-rest.json`. Klucz wpisz w `env` (nie w `args` — Windows psuje spacje). Obsidian musi być włączony.
5. Wklej config: Claude Desktop → Settings → Developer → Edit Config → `claude_desktop_config.json` (`%APPDATA%\Claude\`). Podmień `TWOJ_USER` / klucz. Jeśli plik już ma `mcpServers`, dopisz tylko nowy serwer.
6. **Zamknij Claude Desktop całkiem** (ikona w trayu → Quit) i uruchom ponownie. Przy czacie ma być ikona narzędzi.
7. Utwórz w Claude **Project** i wklej mu treść `CLAUDE-INSTRUKCJE-PROJEKTU.txt` jako instrukcje. (Claude Desktop sam nie czyta `AGENTS.md` — te instrukcje każą mu to robić.)
8. Test: napisz „wypisz foldery w moim vaulcie i przeczytaj AGENTS.md". Powinien wymienić 00-daily … 40-archive.

## Dla Claude (jeśli to czytasz jako instrukcję)
Pomóż użytkownikowi z kroków 4–8. Nie zakładaj, że dostęp już działa — sprawdź narzędziem, zanim cokolwiek zapiszesz. Zapytaj o ścieżkę vaultu i o to, które ścieżki (A/B) wybrał. Nie wpisuj kluczy API do plików w repo. Po teście zaproponuj pierwszą notatkę dzienną.

## Czego tu nie ma (celowo)
- Skryptów terminalowych (`add-idea`, `dodaj-zadanie`) — działają tylko na Linuksie; tu ich rolę pełnią szablony.
- Komend `/daily-review`, `/weekly`, `/lint` — tu to pliki w `prompts/`; mówisz Claude'owi nazwę.
- Obsidian Sync / Remotely Save / Git — dodaj sam, jeśli potrzebujesz kopii (najprościej plugin `obsidian-git` albo kopia folderu).

## Uwaga: dane firmowe
Zanim wrzucisz tu cokolwiek z pracy, sprawdź w IT, czy wolno łączyć notatki z Claude. Bez zgody: zostaw sam szkielet i używaj Obsidiana bez AI.
