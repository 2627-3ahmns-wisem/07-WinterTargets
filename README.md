# Frosty Targets – 3AHMNS

Unity-Version: **6000.3.24f1**. Projekt: Frosty Targets.

## Projekt öffnen
1. Unity Hub öffnen, **Add project from disk** wählen und diesen Ordner auswählen.
2. Unity **6000.3.24f1** verwenden und den ersten Paketimport abwarten.
3. Szene `Assets/MyGame/Scenes/ShootingScene.unity` öffnen, **Play** drücken.
4. `Assets/MyGame/Scripts/GameManager.cs` und `Target.cs` untersuchen.

## Hinweis bei `UnityEngine.UI` / `Text`-Fehlern
Das Paket **Unity UI (uGUI)** ist unter `Packages/manifest.json` als `com.unity.ugui` eingetragen. Falls trotzdem CS0234 oder CS0246 erscheint: `Window > Package Management > Package Manager` öffnen und unter **In Project** prüfen, ob Unity UI geladen ist. Im Paketmanager **Refresh/Resolve** ausführen; gegebenenfalls Unity schließen und den Ordner `Library` löschen, dann erneut öffnen. Nicht die `using UnityEngine.UI`-Zeile entfernen: sie wird für die vorhandene Punkteanzeige gebraucht.

## Unterricht
Das vorhandene Spawning, der Score und der Sieg bei zehn Treffern sind **Ausgangscode**. Schüler:innen erweitern diese Mechaniken anhand der GitHub-Issues. Der Erstimport ist eine Ausgangsversion; keine Aufgaben sind vorweg implementiert.
Festgestellte Probleme – Crosshair und Zielscheiben
Beim Testen des Spiels sind mir mehrere Probleme mit dem Crosshair aufgefallen:
* Crosshair zu groß: Das Fadenkreuz ist beim Start des Spiels viel zu groß und erschwert dadurch das genaue Zielen auf die Zielscheiben.
* Bewegung über gesamten Bildschirm: Im Game-Modus bewegt sich das Crosshair über den ganzen Bildschirm. Die Steuerung wirkt dabei teilweise verzögert bzw. ruckelig (Lag).
* Probleme beim Treffen: Wenn ich mit dem Crosshair auf die oberen Bereiche der Zielscheiben ziele, werden die Treffer teilweise nicht erkannt und es werden keine Punkte gezählt.
Geplante Verbesserungen
Ich möchte das Crosshair verkleinern und seine Bewegung verbessern, damit es flüssiger und genauer gesteuert werden kann. Außerdem soll die Treffererkennung überprüft und angepasst werden, damit Treffer auf allen Bereichen der Zielscheiben zuverlässig erkannt und die Punkte korrekt gezählt werden.
Ziel ist es, eine genauere Steuerung und ein besser funktionierendes Spielerlebnis zu ermöglichen.
