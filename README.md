# 🎲 Kniffel Online

Ein Kniffel-Spiel direkt im Browser – lokal, online oder gegen den Computer.

**[▶ Jetzt spielen](https://adriansgitt.github.io/kniffel/)**

## Features

- 📱 **Lokaler Modus** – 1-4 Spieler am selben Gerät
- 🌐 **Online Multiplayer** – Echtzeit-Spiel über Raum-Code (bis zu 4 Spieler)
- 🤖 **Computer-Gegner** – KI mit strategischer Spielweise
- 🏆 **Globale Bestenliste** – Top 50 Scores mit Wahrscheinlichkeitsberechnung
- 🔊 **Sound-Effekte** – Web Audio API, keine externen Dateien
- 📊 **Scorecard** – Bonus-Tracking, Gesamt-Aufschlüsselung, letzte Eingabe markiert

## Wie funktioniert's?

### Lokal spielen
1. Spieleranzahl wählen (1-4)
2. Namen eingeben
3. Optional: 🤖 Gegen Computer aktivieren
4. Spiel starten!

### Online spielen
1. "Online" auswählen
2. **Spiel erstellen** → Raum-Code an Mitspieler senden
3. Oder **Code eingeben** → Spiel beitreten
4. Host startet das Spiel

## Technologie

- Vanilla HTML/CSS/JavaScript (Single-File)
- Firebase Realtime Database (Online-Multiplayer & Bestenliste)
- Web Audio API (Sounds)
- Gehostet auf GitHub Pages

## Spielregeln

Jeder Spieler hat pro Runde 3 Würfe mit 5 Würfeln. Nach jedem Wurf können Würfel behalten werden. Danach muss eine Kategorie gewählt werden:

| Kategorie | Punkte |
|-----------|--------|
| Einser - Sechser | Summe der jeweiligen Augenzahl |
| Dreierpasch | Summe aller Würfel (mind. 3 gleiche) |
| Viererpasch | Summe aller Würfel (mind. 4 gleiche) |
| Full House | 25 (3 gleiche + 2 gleiche) |
| Kleine Straße | 30 (4 aufeinanderfolgende) |
| Große Straße | 40 (5 aufeinanderfolgende) |
| Kniffel | 50 (5 gleiche) |
| Chance | Summe aller Würfel |

**Bonus:** 35 Punkte wenn der obere Block ≥ 63 erreicht.
