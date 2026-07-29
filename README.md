# Farsi in 5 Minuten

Eine kleine Web-App zum Farsi-Lernen: 84 Lektionen à ungefähr fünf Minuten, verteilt auf zwölf Wochen.
Umgangssprache aus Teheran, Du-Form, mit Schwerpunkt auf Gesprächen in Familie und Partnerschaft.

**Live:** siehe Einstellungen → Pages im Repository

## Was drin ist

- 360 Vokabeln und 72 Sätze, alles in lateinischer Lautschrift
- Aussprache über die Sprachausgabe des Geräts (Persisch), zusätzlich in halbem Tempo
- Sprechübungen mit Mikrofon-Prüfung, wo der Browser das unterstützt
- Verteilte Wiederholung (Leitner-System), damit Gelerntes hängen bleibt
- Fortschritt: Serie, XP, Wochenraster, Festigkeit jeder Vokabel
- Läuft offline, alle Daten bleiben auf dem Gerät

## Installieren

**Android:** Seite in Chrome öffnen, dann auf „Jetzt installieren" tippen (oder Menü → App installieren).

**iPhone/iPad:** Seite in Safari öffnen, Teilen-Symbol → „Zum Home-Bildschirm".

## Aussprache einrichten

Die App nutzt die persische Stimme des Systems. Falls keine vorhanden ist:

- **Android:** Einstellungen → System → Sprachen → Text-in-Sprache → Sprachdaten → Persisch
- **iPhone:** Einstellungen → Bedienungshilfen → Gesprochene Inhalte → Stimmen → Persisch

## Dateien

| Datei | Zweck |
|---|---|
| `index.html` | Die komplette App inklusive Lehrplan |
| `manifest.webmanifest` | Damit sie sich als App installieren lässt |
| `sw.js` | Service Worker für den Offline-Betrieb |
| `icon-*.png`, `apple-touch-icon.png` | App-Symbole |

## Nach einer Änderung

Wenn `index.html` bearbeitet wird, in `sw.js` die Zeile `const CACHE = "farsi5-v1";` hochzählen
(`farsi5-v2` und so weiter). Sonst zeigen installierte Geräte weiter die alte Version.

## Fortschritt sichern

Der Lernstand liegt im Speicher des Browsers. Unter *Mehr → Sicherung herunterladen* lässt er sich
als Datei exportieren und auf einem anderen Gerät wieder einspielen.
