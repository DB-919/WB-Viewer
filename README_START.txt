BECKER WB VIEWER WEBAPP V1.5
==============================

Vollständige Standalone-WebApp für Wärmebehandlungs-/Loggerdaten.

START
-----
1. index.html per Doppelklick im Browser öffnen.
2. TXT/CSV/TSV auswählen oder per Drag & Drop auf die Fläche ziehen.
3. Die Messdaten werden ausschließlich lokal im Browser verarbeitet.

Für iPhone/iPad oder Installation als WebApp:
- Den kompletten Ordner auf einen normalen Webserver bzw. GitHub Pages laden.
- Im Browser öffnen und anschließend „Zum Home-Bildschirm“ verwenden.
- Bei gehosteter Nutzung wird die App nach dem ersten Laden über den Service Worker offline zwischengespeichert.

ENTHALTENE FUNKTIONEN
---------------------
- Import von MN/AT-Logger-TXT sowie TXT/CSV/TSV-Tabellen.
- Automatische Erkennung von 1 bis 4 belegten Messkanälen.
- Positionsgetreuer Loggerimport: leere Zwischenkanäle verschieben keine Messwerte.
- Unterstützung von CH1-only, CH1+CH4 und CH1-CH4.
- Automatische Erkennung von UTF-8/UTF-16-Textdateien.
- Kanal ein-/ausblenden und frei benennen.
- Diagramm optional ab definierter Starttemperatur.
- Zeitachse Minuten/Stunden.
- Manuelle Y-Achsen-Grenzen.
- Bis zu 5 Solltemperaturbereiche mit Sollwert ± Toleranz.
- Haltebereich mit Start/Ende und Setzen direkt im Diagramm.
- Kennwerte/Übersicht zum geladenen Verlauf.
- Performante Darstellung großer Messdateien durch Min/Max-Downsampling.
- Export als PNG, SVG und CSV.
- Drucken bzw. PDF über die Browser-Druckfunktion.
- Responsive Darstellung für Desktop, Tablet und Smartphone.
- Komplett lokale Verarbeitung ohne Upload der Messdaten.

DATEIEN
-------
index.html             eigentliche WebApp; funktioniert auch direkt lokal
manifest.webmanifest   PWA-Metadaten für gehostete Nutzung
service-worker.js      Offline-Cache bei gehosteter Nutzung
icon-180.png           App-Icon iOS
icon-512.png           PWA-App-Icon
CHANGELOG_V1_5.txt     Änderungen dieser Version

HINWEIS
-------
Bei direktem Öffnen per file:// funktioniert der Viewer vollständig. PWA-Installation/Service-Worker benötigen aus Browser-Sicherheitsgründen eine HTTP/HTTPS-Bereitstellung.
