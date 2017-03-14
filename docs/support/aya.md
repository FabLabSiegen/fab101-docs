## Delta Robot 3D-Drucker "AYA"

AYA ist ein Delta Robot 3D-Drucker aus der RepRap Familie, genau genommen handelt es sich um das Modell Kossel Mini.
http://reprap.org/wiki/Kossel

Zur Nutzung benötigt werden:
* Ein Computer mit Windows oder Mac
* Eine SD-Karte
* Ein Slicer nach Wahl, wir erläutern weiter unten die Nutzung von Cura

## Einrichtung Cura

Cura kann zum slicen von Modellen für AYA verwendet werden. Dazu muss in wenigen Schritten eine neue Maschine eingerichtet werden.

* Menü: Maschine -> Add new machine…
  1. auf “Next >” klicken
  2. Maschinentyp “Andere (z.b.: RepRap, MakerBot, Witbox)” auswählen
  3. auf “Next >” klicken
  4. “DeltaBot” auswählen
  5. auf “Next >” klicken
  6. auf “Finish” klicken
* Menü: Maschine -> Geräte-Einstellungen…
  1. Maximale Breite (mm): 170
  2. Maximale Tiefe (mm): 170
  3. Maximale Höhe (mm): 250
  4. Beheizter Drucktisch: Ja
  5. Mittelpunkt der Bau Plattform (0,0): Ja
  6. Druckflächenform: Circular
  7. GCode Art: RepRap
  8. auf “OK” klicken
* Grundlegend
  Druckmaterial(mm): 1.75
  Größe der Druckdüse (mm): 0.4
* Weitere Parameter nach Bedarf ändern/anpassen

## Bedienungsanleitung:

#### Grundsätzliches
* Die Maschine wird über den Ein-/Aus-Schalter am Netzteil ein- bzw. ausgeschaltet.
* Zum Drucken wird kein Computer benötigt, der G-Code wird direkt über eine SD-Karte eingelesen.
* Der Filamentwechsel erfordert einen Computer. Wir haben mit printrun (http://www.pronterface.com) gute Erfahrungen gemacht
* Mit dem kleinen Drehknopf kann durch das Menu navigiert werden
* Es kommt vor, das der Drucker beim Aufheizen nicht reagiert. Genaue Ursachen sind noch unbekannt. Bisher hat komplett ausschalten und wieder einschalten geholfen

#### Drucken
 1. Die SD-Karte mit dem G-Code wird seitlich eingeführt
 2. Drehknopf einmal drücken, um das Menü zu öffnen
 3. Im Menü "Print from SD" auswählen und bestätigen
 4. Modell aus der Liste auswählen und bestätigen
 6. Der Drucker sollte nun aufheizen und den Druck nach einer Wartezeit starten
