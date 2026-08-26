# Abfahrt / Departures

Ein minimalistischer **Live-Abfahrtsmonitor** für den Bahnhof – gestaltet im Stil einer klassischen Anzeigetafel. Die Seite zeigt aktuelle Abfahrten mit Uhrzeit, Linie, Ziel, Gleis und Status.

## Features

- **Klassische Anzeigetafel-Optik** – dunkler Hintergrund, leuchtende Akzente
- **Klar ablesbare Tabelle** – Zeit, Linie, Ziel, Gleis/Steig, Status
- **Status auf einen Blick** – farbcodiert plus Symbol-Präfix:
  - `●` **pünktlich** (grün)
  - `▲` **+5 / +10 Min** (gelb, Verspätung)
  - `▲` **+15 Min und mehr** (rot, stark verspätet)
- **Barrierefrei (WCAG AA)** – ausreichende Kontraste, `prefers-reduced-motion`
- **Responsive** – passt sich an Mobilgeräte an
- **Semantisches HTML** für bessere Zugänglichkeit und SEO

## Demo

Öffne `index.html` direkt im Browser. Kein Build-Schritt oder Server nötig.

```bash
# optional: lokalen Server starten für saubere Pfade
python -m http.server
```

## Projektstruktur

```
.
├── index.html        # Abfahrtstafel (Struktur & Inhalt)
├── style.css         # Gestaltung (Design-Tokens, responsiv)
├── STYLEGUIDE.md     # Design-System & Tokens
├── readme.md         # diese Datei
└── opencode.json     # Projekt-Skill-Konfiguration
```

## Technologie

- **HTML5** – semantische Struktur
- **CSS3** – Custom Properties, Flexbox, Media Queries
- Kein externes Framework oder Bibliothek

## Style Guide

Design-Entscheidungen, Farbpalette und Typografie sind im [STYLEGUIDE.md](STYLEGUIDE.md) dokumentiert. Kernwerte:

| Token         | Wert      | Verwendung              |
|---------------|-----------|-------------------------|
| `--accent`    | `#ffcc00` | Header-Akzent           |
| `--ok`        | `#4ade80` | Status „pünktlich"      |
| `--warn`      | `#facc15` | Status „Verspätung"     |
| `--late`      | `#f87171` | Status „stark verspätet"|

## Versionshinweis

Die aktuelle Version wird in der Browser-Konsole ausgegeben (z. B. `Fahrplan v1.2.0`).

## Lizenz

Noch nicht definiert.