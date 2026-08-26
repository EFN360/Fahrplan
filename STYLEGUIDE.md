# Style Guide — Abfahrtsmonitor

## Farben / Design-Tokens

| Name        | Wert       | Verwendung                          |
|-------------|------------|-------------------------------------|
| `--bg`          | `#0a0a0b`  | Seiten-Hintergrund (dunkel)         |
| `--surface`     | `#141416`  | Tabellen-Fläche                     |
| `--surface-hover`| `#1c1c1f` | Zeilen-Hover                        |
| `--border`      | `#27272a`  | Zeilen-Trenner                      |
| `--text-primary`| `#fafafa`  | Primärtext (hoher Kontrast)         |
| `--accent`      | `#ffcc00`  | Header-Akzent (Gelb)                |
| `--headline`    | `#ffffff`  | Hauptüberschrift (weiß)             |
| `--ok`          | `#4ade80`  | Status "pünktlich" (Grün)           |
| `--warn`        | `#facc15`  | Status "Verspätung" (Gelb)          |
| `--late`        | `#f87171`  | Status "stark verspätet" (Rot)      |

## Typografie

| Element | Font                   | Größe | Gewicht |
|---------|------------------------|-------|---------|
| Body    | Courier New, monospace | —     | normal  |
| h1      | Courier New, monospace | 42px  | normal (bold) |
| th/td   | Courier New, monospace | 18px  | normal |

## Abstände & Layout

- Seiten-Padding: `40px`
- Tabelle max. Breite: `900px`, zentriert
- Zell-Padding: `12px`
- Zellen-Ausrichtung: links

## Status-Referenz

| Klasse          | Blick sofort  | Farb-Token |
|-----------------|---------------|------------|
| `.on-time`      | p aktiv       | `--ok`    |
| `.delay-warning`| +5 / +10 Min  | `--warn`  |
| `.delay-late`   | +15 Min u. mehr | `--late` |

## Empfehlung (Kontrast/Barrierefreiheit)

- Statusfarben v1.2 sind auf dunklem Grund WCAG-AA-fähig: `--ok` (#4ade80), `--warn` (#facc15), `--late` (#f87171) liegen über 4.5:1 Kontrast.
- Kopfzeilen-Zeilentrenner bleibt Gelb (#ffcc00).
- Überschrift (h1) bleibt weiß (§ v1.1-Konvention); Header/Accent ist gelb.
- Status ergänzt Farbe durch Symbol-Präfix (● / ▲) – nie Farbe allein als Signal.
- `prefers-reduced-motion` wird respektiert.