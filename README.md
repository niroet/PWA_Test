# Schlüsselübergabe — PWA Prototyp

Non-funktionaler Prototyp für eine digitale Schlüsselübergabe (Lastenheft: Perpetuum Progress GmbH).

Zwei Unterschriftsfelder (Ausgeber / Empfänger), ein **Übergabe**-Button. Installierbar als PWA auf Android & iOS.

## Lokal testen

```bash
python3 -m http.server 8080
# dann http://localhost:8080
```

Service Worker und Installation funktionieren nur über HTTPS oder `localhost`.

## Auf dem Handy als App installieren

- **Android (Chrome):** Menü ⋮ → „App installieren" / „Zum Startbildschirm hinzufügen"
- **iOS (Safari):** Teilen-Symbol → „Zum Home-Bildschirm"

## Stack

- Vanilla HTML/CSS/JS — keine Build-Tools
- [signature_pad](https://github.com/szimek/signature_pad) via CDN
- Service Worker für Offline-Nutzung
- Deploy auf GitHub Pages
