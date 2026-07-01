# Release V2.2.0

## Neue Features:

- **Foto-Rotation** 🔄
  - Hintergrundbilder und einzelne Foto-Layer können jetzt um beliebige Grad gedreht werden (z. B. 90, 180, 270)
  - Nützlich zur Korrektur von Fotos mit falscher Orientierung
  - Neue Eigenschaft `Rotate Background` (Number, Standard: 0)
  - Verwendet SVG `transform="rotate(...)"` zentriert auf dem Bild

## Änderungen:

- README.md aktualisiert mit neuer Dokumentation für die Rotations-Funktion
- SVG MergeModul.msapp aktualisiert mit Rotations-Unterstützung
- Feature-Liste erweitert: "Rotate background image and individual photo layers"

## Anleitung zum Erstellen des Releases:

Da das Release manuell auf GitHub erstellt werden muss, folge diesen Schritten:

1. Gehe zu https://github.com/mlnc21/PowerApps-SVG-Merge-Modul/releases/new
2. Erstelle einen neuen Tag: `V2.2.0`
3. Titel: `V2.2.0`
4. Kopiere die Release Notes oben in die Beschreibung
5. Wähle den `main` Branch als Target
6. Klicke auf "Publish release"
