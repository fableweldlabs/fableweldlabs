# Inventar und Ausrüstung — Schnellstart

Inventar und Ausrüstung 1.0.0. Godot 4.7.2, Windows x64. Beachten Sie die beiliegende Lizenz und die Komponentenhinweise.

1. Projekt und Spielstände als Kopie sichern. `addons/fableweld_inventory` in das
   Spiel kopieren. Vor dem Ersetzen Versionen vergleichen und eigene Änderungen
   sichern. Ein Uhr- oder NPC-Addon wird nicht benötigt.
2. Fableweld Inventory & Equipment in den Projekteinstellungen unter Plugins
   aktivieren. Die Sprache im Dock wählen; die globale Spielsprache bleibt unverändert.
3. Gegenstände erstellen oder Startgegenstände hinzufügen. Im Inspektor bearbeiten,
   den Katalog prüfen und als `.tres` außerhalb von `addons` speichern. Eine
   vorhandene Zieldatei vor dem Aktualisieren laden; das Laden verlangt eine
   Bestätigung. Gegenstands-IDs stabil halten.
4. Im Beispielprojekt `demo/inventory_quick_start.tscn` öffnen und F6 drücken.
   Die obere Sprachauswahl steuert Register und Bedienfelder gemeinsam. Die
   Startklinge ausrüsten, einen Trank zuweisen, einen Stapel teilen und Gegenstände
   in die Truhe übertragen.
5. In eigenen Szenen `controller_path` der Bedienfelder auf einen
   `FWSlotInventoryController` setzen. Austauschende Raster brauchen dieselbe
   Katalogressource und eine gemeinsame, nicht leere `transfer_group`. Effekte
   der Gegenstände und Grundwerte der Figuren liefert das Spiel.
6. Controller in `FWInventorySession.controllers` mit stabilen Speicher-IDs und
   NodePaths registrieren. `FWInventorySavePanel.session_path` auf diese Sitzung
   setzen. Pro Speicherplatz oder Welt einen eigenen `user://...json`-Pfad wählen.
7. Die Inventarsitzung speichern und laden. Sie enthält registrierte Taschen,
   Ausrüstung und Schnellzugriffe, aber nicht das ganze Spiel. Das ältere Beispiel
   verliert seinen Kontrollpunkt beim Schließen. Eine vorhandene `.fw-writing`
   vor dem erneuten Versuch einer blockierten Speicherung sichern. Gleichzeitige
   Schreibvorgänge werden nicht unterstützt.
8. Aktualisierungen zuerst an einer Kopie testen. Eigene Kataloge, Szenen und
   Spielstände außerhalb der Anbieterordner halten. Vor dem Entfernen abhängige
   Verweise ersetzen, das Plugin deaktivieren und erst dann den Addon-Ordner
   löschen. Noch referenzierte Skripte zu löschen beschädigt Szenen.

Sprachwechsel erhalten IDs und eigene Texte. Beispielkategorien und Werte werden
über `translate_example_names` übersetzt; in wiederverwendbaren Ansichten ist
diese Option standardmäßig aus. Unbekannte eigene Texte bleiben erhalten.
Muttersprachliche Prüfung, allgemeine Projektkompatibilität und abschließende
Abnahme exportierter Pakete werden nicht behauptet.
