# 🧙 MTG Commander Deck Pages

GitHub Pages ready — NFC-powered deck box ID system for 10 Commander decks.

## Struktur

```
mtg-decks/
├── index.html                    ← Übersicht aller Decks
└── decks/
    ├── kaalia/index.html
    ├── atraxa/index.html
    ├── edgar/index.html
    ├── urdragon/index.html
    ├── meren/index.html
    ├── breya/index.html
    ├── omnath/index.html
    ├── krenko/index.html
    ├── kenrith/index.html
    └── wilhelt/index.html
```

## GitHub Pages Setup

1. Neues öffentliches Repository auf GitHub erstellen, z.B. `mtg-decks`
2. Alle Dateien in das Repository hochladen (Upload via Web UI oder `git push`)
3. In GitHub → **Settings → Pages → Deploy from branch → main → / (root)**
4. Warten (~1 Minute), dann ist die Site live unter:
   `https://DEINUSERNAME.github.io/mtg-decks/`

## NFC-Tags programmieren

Für jede Deckbox brauchst du einen **NTAG213** oder **NTAG215** Sticker.

| Deck | NFC-Tag URL |
|------|-------------|
| Kaalia of the Vast | `https://DEINUSERNAME.github.io/mtg-decks/decks/kaalia/` |
| Atraxa | `https://DEINUSERNAME.github.io/mtg-decks/decks/atraxa/` |
| Edgar Markov | `https://DEINUSERNAME.github.io/mtg-decks/decks/edgar/` |
| The Ur-Dragon | `https://DEINUSERNAME.github.io/mtg-decks/decks/urdragon/` |
| Meren | `https://DEINUSERNAME.github.io/mtg-decks/decks/meren/` |
| Breya | `https://DEINUSERNAME.github.io/mtg-decks/decks/breya/` |
| Omnath | `https://DEINUSERNAME.github.io/mtg-decks/decks/omnath/` |
| Krenko | `https://DEINUSERNAME.github.io/mtg-decks/decks/krenko/` |
| Kenrith | `https://DEINUSERNAME.github.io/mtg-decks/decks/kenrith/` |
| Wilhelt | `https://DEINUSERNAME.github.io/mtg-decks/decks/wilhelt/` |

### App: NFC Tools (Android & iOS)
1. App öffnen → **Write** → **Add a record** → **URL/URI**
2. URL einfügen (aus Tabelle oben, mit deinem echten GitHub-Username)
3. **Write** → Tag an Handy halten

## Anpassungen

In jeder `decks/DECKNAME/index.html`:
- `<h1 class="commander-name">` → Commander-Name ändern
- `<img src="...">` → eigene Commander-Artwork-URL einsetzen
- Archidekt-Link im ersten Button (`href=`)
- Kontaktdaten im Lost-&-Found-Bereich
- Power Level, Farben, Strategie-Text, Mulligan-Hinweise

## Commander-Bild

Einfachste Option: Screenshot vom Commander-Bild via Scryfall.
`https://scryfall.com/search?q=kaalia+of+the+vast` → Karte öffnen → Bild-URL kopieren.
Das Bild dann entweder direkt verlinken oder in den `decks/DECKNAME/`-Ordner hochladen.
