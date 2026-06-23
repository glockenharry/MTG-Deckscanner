# 🧙 MTG Commander Deck Collection v2

GitHub Pages · NFC-powered · Edit-Modal für alle Decks

## Was ist neu in v2?

- **Edit-Modal direkt im Browser**: Kein HTML-Code mehr bearbeiten.
  Auf Stift-Icon klicken → Name, Bild-URL, Archidekt-Link, Farben, Power Level usw. ändern → Speichern.
- **Deck hinzufügen**: "+ Deck hinzufügen"-Button → Formular ausfüllen → fertig.
- **Bild-Vorschau**: Bild-URL eingeben und sofort sehen, ob das Bild stimmt.
- **NFC-URL mit Copy-Button**: Auf jeder Deck-Seite steht die fertige URL zum Kopieren.
- **5 Decks sind bereits als Beispiel vorgeladen** (Kaalia, Atraxa, Edgar, Meren, Krenko).

## Dateien

```
mtg-decks-v2/
├── index.html          ← Hauptseite (Übersicht + Edit-Modal)
├── deck.html           ← Dynamische Deck-Detailseite
├── README.md
└── decks/
    ├── kaalia/index.html   ← Redirect → deck.html
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

1. Neues **öffentliches** Repository anlegen (z.B. `mtg-decks`)
2. ZIP entpacken und alle Dateien hochladen (Safari → github.com → Add file → Upload files)
3. Settings → Pages → Deploy from branch → main → / (root) → Save
4. ~1 Minute warten → Live unter:
   `https://DEINUSERNAME.github.io/mtg-decks/`

## Bild-URL Tipp (Scryfall)

1. Gehe zu https://scryfall.com
2. Suche deinen Commander
3. Öffne die Karte → rechte Maustaste auf das Bild → "Bildadresse kopieren"
4. Diese URL ins Edit-Formular unter "Commander Bild-URL" einfügen

Beispiel: `https://cards.scryfall.io/art_crop/front/0/e/0eda2e3a...jpg`

## NFC-Tags

- **Chip**: NTAG213 oder NTAG215 Sticker
- **App**: NFC Tools (iOS & Android, kostenlos)
- **URL**: Auf jeder Deck-Seite angezeigt und per Klick kopierbar

Wenn du deinen GitHub-Username eingetragen hast (in index.html und deck.html `DEINUSERNAME` ersetzen), 
werden die NFC-URLs automatisch korrekt angezeigt.

## Kontaktdaten anpassen

In `deck.html` einmalig suchen & ersetzen:
- `dein.name@example.com` → deine E-Mail
- `DeinName#1234` → dein Discord
- `Hamburg, Deutschland` → dein Ort
