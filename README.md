# Octosello – strona www

Statyczna strona marki **Octosello** – parasolowej marki compliance dla e-commerce (usługi środowiskowe, doradztwo prawne, sprzedaż cross-border, procesy AI).

## Zawartość

| Plik | Opis |
|---|---|
| `index.html` | Strona główna |
| `uslugi-srodowiskowe.html` | Usługi środowiskowe (EPR, BDO, KOBiZE, EUDR, PPWR) |
| `doradztwo-prawne.html` | Doradztwo prawne |
| `sprzedaz-cross-border.html` | Sprzedaż cross-border |
| `procesy-ai.html` | Procesy AI |
| `case-study.html` | Case study |
| `panel/index.html` | Demo panelu klienta |
| `img/` | Zdjęcia ekspertów i logotypy |

Strona to czysty HTML/CSS/JS – nie wymaga budowania ani zależności. Czcionki ładowane są z Google Fonts.

## Podgląd lokalny

Otwórz `index.html` w przeglądarce albo uruchom prosty serwer:

```bash
python3 -m http.server 8000
# http://localhost:8000
```

## Wdrożenie

### GitHub Pages
1. W repozytorium wejdź w **Settings → Pages**.
2. W sekcji *Build and deployment* wybierz **Deploy from a branch**, gałąź `main`, folder `/ (root)`.
3. Po chwili strona będzie dostępna pod `https://proftheone.github.io/octosello/`.
4. Własna domena (np. `octosello.com`): wpisz ją w polu *Custom domain* i ustaw u rejestratora rekord `CNAME` na `proftheone.github.io` (lub rekordy `A` dla domeny głównej).

### Netlify
1. **Add new site → Import an existing project** i wskaż to repozytorium.
2. Build command: puste, Publish directory: `/`.
3. Podłącz domenę w *Domain management*.

### Zwykły hosting (FTP)
Wgraj całą zawartość repozytorium (z zachowaniem folderów `img/` i `panel/`) do katalogu `public_html` na serwerze.
