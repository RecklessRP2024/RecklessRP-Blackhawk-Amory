# Kaliber-Bilder - Anleitung zum Einfügen von Links

Die Caliber-Icons wurden von Emojis auf Bilder umgestellt. Jedes Kaliber hat nun ein `<img>` Element mit einem leeren `src` Attribut.

## Wie man Bilder einfügt

### 1. Bild-Links hinzufügen

Öffnen Sie `blackhawkammunition.html` und suchen Sie nach `<img class="caliber-icon" src="" alt="...">`.

Ersetzen Sie das leere `src=""` mit einem Link zu Ihrem Bild:

```html
<!-- Beispiel: Vorher -->
<img class="caliber-icon" src="" alt="Pistole">

<!-- Beispiel: Nachher -->
<img class="caliber-icon" src="https://example.com/pistole-bild.png" alt="Pistole">
```

### 2. Bild-Quellen

Sie können folgende Quellen verwenden:
- **Discord CDN**: `https://media.discordapp.net/attachments/...`
- **Externe URLs**: Beliebige gehostete Bilder
- **Lokale Dateien**: `/images/kaliber/pistole.png`

### 3. Bildempfehlungen

- **Größe**: 32x32 Pixel (optimal, da CSS `width: 32px; height: 32px;` ist)
- **Format**: PNG oder JPG (mit Transparenz PNG bevorzugt)
- **Stil**: Konsistent mit dem Seiten-Design halten

## CSS-Eigenschaften

Die Bilder werden mit folgendem CSS styling angezeigt:

```css
.caliber-icon {
    width: 32px;
    height: 32px;
    object-fit: contain;
    object-position: center;
    opacity: 0.85;
    filter: brightness(0.95) saturate(0.9);
}
```

Die Bilder werden automatisch:
- Auf 32x32 Pixel skaliert
- Mit `object-fit: contain` zentriert (verhindert Verzerrung)
- Mit leicht reduzierter Helligkeit und Sättigung angepasst

## Beispiele für alle Kaliber

Alle Platzhalter für Bilder finden Sie im Modal "ALLE VERFÜGBAREN KALIBER":

```html
<!-- Pistolen -->
<img class="caliber-icon" src="" alt="Pistole">
<img class="caliber-icon" src="" alt="Munition">

<!-- Gewehre -->
<img class="caliber-icon" src="" alt="Gewehr">

<!-- Revolver -->
<img class="caliber-icon" src="" alt="Revolver">

<!-- Spezial/Präzision -->
<img class="caliber-icon" src="" alt="Spezial">
```

## Schnelle Bearbeitung

Suchen Sie in der HTML-Datei nach:
- `<img class="caliber-icon" src="" alt="`

Und ersetzen Sie alle leeren `src=""` Attribute mit Ihren Bildlinks.

---

**Hinweis**: Die leeren `src` Attribute sind bereits vorbereitet. Fügen Sie einfach Ihre Bildlinks ein!



<img class="caliber-icon-preview" src="" alt="">



