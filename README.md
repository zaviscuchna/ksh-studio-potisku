# KSH Studio potisku

Editor potisku týmových mikin KSH Partners na mikinách Malfini. Běží celý v prohlížeči, nic se nikam neodesílá.

**Jak otevřít:** odkaz na GitHub Pages, nebo stáhni repo (Code → Download ZIP), rozbal a otevři `index.html` (nejlíp v Chrome). Funguje i offline.

## Co v něm jde
- **Mikina:** 6 modelů Malfini (431 Vibe Hoodie, 430 Vibe Crew, 420 Moon, 422 Chill, 428 Cloud GOTS, 413 Cape), 61 barev, u každého gramáž, materiál, střih a tabulka rozměrů.
- **Pohledy:** předek, záda, levý rukáv, model zepředu a zezadu. Kolečko myši = zoom, tažení prázdného místa = posun.
- **Vrstvy:** logo KSH (klíček, nápis, logo celé), logo KraKrám (i powered by KSH), tvary (obdélník, kruh, čára, tečkovaná čára), text (VT323, JetBrains Mono, Inter Tight, Permanent Marker), vlastní obrázek (PNG, JPG, SVG, WebP), koncepty A–D, šablony. Tažením posuneš, rohy = velikost, korálový bod = otočení. Rozměry v cm od středu a od švu u krku.
- **Paleta:** barvy KSH a KraKrám nahoře, vlastní barvy se ukládají do „Moje“ (pravý klik = smazat). Přebarvit jde i obrázek nebo koncept.
- **Šablona E** (KSH + KraKrám · Lineup) je složená z vrstev: každý text jde přepsat nebo smazat, velikost písma zůstává.
- **Stěna barev:** návrh na všech barvách všech modelů najednou, s přepínáním barev loga.
- **Kontrola tisku:** přesahy, malé písmo, limity výšivky, počet sít u sítotisku.
- **Balíček pro tisk** (Export → Balíček pro tisk…): jeden ZIP, který jde rovnou tiskárně nebo grafikovi:
  - pro každé místo potisku **PDF a SVG ve skutečné velikosti** (vektor, písmo převedené do křivek, loga i koncepty jako křivky) a **PNG 300 dpi** s průhledným pozadím,
  - **technický list** (PDF): náhled na mikině, kóty od HPS a od středu, rozměry, barvy (HEX, RGB, CMYK), technika, písma, počty kusů a poznámka,
  - náhledy na mikině, návrh `.json` a `CTI-ME.txt` s popisem souborů.
- **Další export:** PNG pohledu, PNG všech pohledů.

Zkratky: Cmd/Ctrl+Z zpět, Cmd/Ctrl+Shift+Z znovu, Cmd/Ctrl+D duplikovat, šipky posun (Shift = 2 cm), Delete smazat, + / − / 0 zoom, F přiblížit na vrstvu, G vodítka, 1–5 pohledy, mezerník + táhnout = posun, Alt = bez přichytávání.

## Sdílení návrhů v týmu
Každému se návrh ukládá v jeho prohlížeči. Pro sdílení: **Návrh → Uložit do souboru** a `.json` nahraj do složky `navrhy/` (na GitHubu Add file → Upload files). Na GitHub Pages se pak všem objeví v **Návrh → Návrhy týmu**. Hezčí název a popis jde dopsat do `navrhy/seznam.json`.

## Poznámky
- Fotky produktů: MALFINI, a.s. (shop.malfini.com). Model je AI vizualizace, střih odpovídá Vibe Hoodie, ostatní barvy se dopočítávají.
- Kapuce na zádech nepřekrývá potisk. Barvy na monitoru ≠ tisk, vždy chtít 1 kus na zkoušku.
- Podklady (`assets/`) generují skripty v projektu KSH (`podklady/priprav.py`, vektory pro tisk `podklady/tisk.py` → `assets/tisk.js` a `assets/tisk-koncepty.js`, načtou se až při exportu). Nový model nebo barva = znovu spustit a nahrát `assets/`.
- Písma viz `LICENSES.md`.
