# Angélique

Haushaltsbuch für den Umzug nach München. Läuft ohne Server, ohne Konto, ohne Tracker.
Alle Daten liegen im Speicher des Browsers auf dem Gerät.

## Auf GitHub und Vercel bringen

1. Auf github.com ein neues Repository anlegen, zum Beispiel `kontur`, ruhig privat.
2. Die fünf Dateien hochladen: `index.html`, `manifest.json`, `sw.js`, `icon-192.png`, `icon-512.png`.
   Direkt im Browser über "Add file" → "Upload files" möglich, ohne Git.
3. Auf vercel.com mit dem GitHub-Konto anmelden, "Add New Project", das Repository auswählen.
4. Keine Einstellungen ändern — Framework "Other", kein Build Command, Output Directory leer.
5. Deploy. Nach etwa dreißig Sekunden gibt es eine Adresse wie `kontur-xyz.vercel.app`.

## Aufs Handy legen

**iPhone:** Adresse in Safari öffnen (nicht Chrome), Teilen-Symbol, "Zum Home-Bildschirm".
**Android:** Adresse in Chrome öffnen, Menü, "App installieren".

Danach startet Angélique wie eine normale App, im Vollbild und ohne Browserleiste. Sie
funktioniert auch offline, weil ein Service Worker die Dateien vorhält.

## Daten sichern

Unter "Budgets" ganz unten. "Als Datei exportieren" legt eine JSON-Datei ab,
"In die Zwischenablage" kopiert denselben Inhalt als Text. Zum Wiederherstellen den
Text in das Feld einfügen und "Wiederherstellen" drücken.

Wichtig: Der Browserspeicher ist kein sicherer Ort. Wer den Verlauf samt Websitedaten
löscht, löscht auch die Buchungen. Einmal pro Woche exportieren genügt.

## Was fest eingebaut ist

Wiederkehrende Zahlungen und Referenzwerte sind Beispielwerte. Sie stehen
oben in `index.html` in den Konstanten `FIX`, `EINMAL` und `KAT` und lassen
sich dort direkt durch die eigenen Zahlen ersetzen.
