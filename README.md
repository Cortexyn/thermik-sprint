# Thermik-Sprint 50 km

Kleiner Streckenflug-Simulator für den Browser. Fliege 50 km so schnell wie möglich:
Kreise in Thermikbärten, gleite zwischen den Wolken und komm mit Endanflughöhe ins Ziel.

Eine einzige Datei, kein Build, keine Abhängigkeiten. `index.html` im Browser öffnen.

## Bedienung

- **Touch:** Himmel gedrückt halten zum Kreisen, mit „Langsamer" und „Schneller" die Fahrt ändern.
- **Tastatur:** `↑` / `↓` für die Fahrt, Leertaste halten zum Kreisen, Enter für einen neuen Flug.

## Spielprinzip

- Start auf 1200 m, Wolkenbasis bei 1700 m, Ziel nach 50 km.
- Schneller fliegen kostet Höhe (Polare grob eines Doppelsitzers, Gleitzahl ca. 43).
- Um jeden Bart liegt ein Ring aus Sinken. Nicht jeder Bart lohnt sich.
- Der Endanflugrechner zeigt, ob die Höhe bis ins Ziel reicht.
- Die Zeit läuft 20-fach beschleunigt. Jede Wetternummer erzeugt dieselben Bärte.

## Bestenliste

Zeiten werden pro Wetter gespeichert. Im Browser-Spiel liegen sie lokal im `localStorage`.
In der gehosteten Claude-Artifact-Version nutzt die Liste zusätzlich eine gemeinsame Datenbank;
diese Anbindung greift nur dort, außerhalb davon fällt das Spiel automatisch auf die lokale Liste zurück.
Die Zeiten werden im Browser gemessen und sind nicht manipulationssicher.
