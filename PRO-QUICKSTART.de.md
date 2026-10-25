Calendar & Growth Pro — Schnellstart
Dokumentation des Versionskandidaten 2.1.0; noch nicht veröffentlicht.

1. Kopiere addons/rpg_time in dein Projekt und aktiviere das Plugin unter Project > Project Settings > Plugins. Entpacke das Beispielprojekt separat und öffne dessen project.godot. Überschreibe nicht die Datei deines Spiels.
2. Öffne Time & Seasons und wähle Deutsch unter Language. Die Panelsprache ändert weder Godot noch die globale Spielsprache.
3. Wähle unter Einrichtung einen res://-Pfad außerhalb von addons und speichere das Profil. Felder werden erst mit Anwenden wirksam. Vor dem Abschnittswechsel anwenden oder zurücksetzen.
4. Lege unter Kalender Monate, Wochentage und Jahreszeiten fest. Eigene Namen bleiben unverändert. Der erste Tagesabschnitt beginnt um 00:00; spätere Startzeiten müssen steigen.
5. Wähle für Wachstum eine Voreinstellung und passe das Tempo an. Reifezeit und Stufen lassen sich einzeln bearbeiten. Reglerbewegungen und neue Voreinstellungen ersetzen diese Änderungen. Die Werte gelten für die nächste erzeugte Szene.
6. Speichere das Profil und erzeuge den gewünschten Aufbau. Ziehe die Szene in deine Welt oder nutze die Einfügefunktion. Behalte eine maßgebliche Uhr pro Welt; füge einem verbundenen Canvas keinen zweiten CanvasModulate hinzu.
7. Die Vorschau prüft Zeit, Jahreszeiten und Ereignisse, ohne Laufzeituhr oder Spielstände zu ändern. Sprünge über mehr als 10.000 Vorkommnisse werden abgelehnt.

Wiederverwendbare Bedienelemente haben interface_language im Inspector. Rufe nach einer Änderung zur Laufzeit refresh() auf. Eigene Titel, Namen und Statusmeldungen übersetzt dein Inhaltssystem. Leerer Text aktiviert die automatisch übersetzte Standardbeschriftung der Schlaftaste.

save_file/load_file speichern die Uhr, kein vollständiges Spiel. Behalte Originalspielstände beim Testen von Updates. Kalender- oder Ereignisänderungen können eine Migration erfordern. Optionale Atmosphärenprofile erweitern die einfache Beleuchtung; Wetter, Kampf und NPC-Bewegung sind nicht enthalten.


Atmosphäre und Entwicklungswerkzeuge
Wähle unter Beleuchtung eine Atmosphären-Voreinstellung und wende sie ausdrücklich an. Effektschalter behalten manuell bearbeitete Kurven bei. Speichere das Profil und erzeuge einen neuen Aufbau. Öffne im optionalen Lumen-Vale-Beispiel den Kalender und scrolle zu Atmosphäre. Ohne Atmosphäre bleibt die Ausgangsansicht erhalten. Vorschau und Nebelschalter ändern das gespeicherte Profil nicht; das Entfernen der Vorschau stellt die ursprüngliche Beleuchtung wieder her.

Lokale Entwicklungswerkzeuge können bei der Erzeugung ausdrücklich eingeschlossen werden. Sie sind standardmäßig ausgeschaltet, werden automatisch mit der Uhr verbunden und bleiben im Release-Programm deaktiviert. Der Fableweld-Vertrag ist in DEVELOPMENT-BRIDGE.md beschrieben; er öffnet keinen Netzwerkzugang.
