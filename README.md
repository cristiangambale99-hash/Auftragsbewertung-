# Auftragsbewertung · Clean Service Scaramuzzo AG

Statische Webapp im verbindlichen Clean-Service-App-Layout (Icon-Leiste links,
Topbar mit Schublade am Handy, Eisblau-Kopf mit Welle, Dashboard «Heute zu tun»,
Liste mit Detail-Panel, einspaltige Formulare, immer Hellmodus).

## Deployment

Nur eine Datei: `index.html`. Keine Abhaengigkeiten, kein Build-Schritt.

1. `index.html` im Repo-Wurzelverzeichnis ersetzen und committen.
2. Vercel deployt automatisch. Framework Preset: **Other**,
   Build Command leer, Output Directory leer bzw. `.`.
3. Nach dem Deploy einmal mit Strg+Shift+R neu laden.

## Menue fixieren

Unten in der Icon-Leiste sitzt der Pin. Ein Klick klappt die Leiste auf
228 px auf, zeigt das volle Logo und die Beschriftungen neben den Icons und
merkt sich die Einstellung pro Geraet. Erneuter Klick loest sie wieder.
Am Handy bleibt es beim Menue-Knopf mit Schublade.

## Inhalt

- Logo und Signet sind als Base64-PNG eingebettet, kein externer Bild-Host.
- Lottie-Icons werden von cdnjs geladen; ohne Internet zeigt die App
  statische Linien-Icons im gleichen Stil.
- Daten liegen im localStorage des Geraets, kein Server, keine Backups.
  Fuer den Echtbetrieb Supabase oder Firestore anbinden.
- Stundensaetze CHF 52.00 / CHF 38.00 sind Annahmen und in den
  Einstellungen der App zu hinterlegen.

## Startdaten

Baustelle BAUMA aus der Stundenuebersicht: 666 h verkauft, 105 h geleistet.
Aehrenweg 11 als geplanter Auftrag ohne Termin.
