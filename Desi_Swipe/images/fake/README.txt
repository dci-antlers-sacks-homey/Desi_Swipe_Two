FAKE BILDER (Deepfakes)
=======================

Lege hier alle Deepfakes ab.

Für jedes Fake-Bild kannst du eine markierte Version erstellen:
  person01.jpg          ← Das Fake-Bild
  person01_marked.jpg   ← Deine markierte Version (mit Pfeilen auf Fehler etc.)

Die _marked Version wird gezeigt wenn:
1. Jemand das Fake fälschlich als "echt" swiped (sofort)
2. Jemand auf "Zurück" geht bei diesem Bild

Dateinamen-Tipps:
- Keine Leerzeichen (benutze _ oder -)
- Keine Umlaute (ä, ö, ü, ß)
- _marked muss vor der Dateiendung stehen!

Danach in index.html bei FAKE_IMAGES eintragen:
  const FAKE_IMAGES = [
    'person01.jpg',
    'celebrity_fake.jpg',
  ];

(Die _marked Versionen werden automatisch erkannt!)
