# JEWLIF Deepfake Detection Game

Ein Tinder-Style Spiel zum Erkennen von Deepfakes.

## Ordner-Struktur

```
deepfake-game/
├── index.html          ← Hauptdatei (hier Bilder eintragen)
├── images/
│   ├── real/           ← Echte Bilder hierhin
│   │   └── README.txt
│   └── fake/           ← Fake-Bilder hierhin
│       └── README.txt
└── README.md
```

## Bilder hinzufügen

### 1. Echte Bilder
- Lege sie in `images/real/`
- Trage die Dateinamen in `index.html` bei `REAL_IMAGES` ein

### 2. Fake-Bilder
- Lege sie in `images/fake/`
- Optional: Erstelle für jedes Bild eine `_marked` Version
  - Beispiel: `person01.jpg` → `person01_marked.jpg`
- Trage die Dateinamen in `index.html` bei `FAKE_IMAGES` ein

### Beispiel in index.html:
```javascript
const REAL_IMAGES = [
  'foto01.jpg',
  'foto02.jpg',
];

const FAKE_IMAGES = [
  'deepfake01.jpg',    // + deepfake01_marked.jpg
  'deepfake02.jpg',    // + deepfake02_marked.jpg
];
```

## Steuerung

- **← Pfeil / Links swipen**: FAKE
- **→ Pfeil / Rechts swipen**: REAL
- **Backspace / ↩️ Button**: Zurück
- **R**: Neustart
- **S**: Shuffle An/Aus
- **F11**: Vollbild

## Markierte Bilder

Die `_marked` Versionen werden gezeigt:
1. **Sofort** wenn jemand ein Fake als echt swiped (falsch)
2. **Bei Zurück** wenn jemand zu einem Fake-Bild zurückgeht

So können Spieler lernen, woran man Fakes erkennt!
