# AYA - EIN SELBSTGEBAUTER 3D-DRUCKER
![alt-text](http://fablab-siegen.de/content/images/2016/06/aya5-1.jpg)

AYA – das ist ein 3D-Drucker, den Studierende des Masters [Human-Computer-Interaction](http://hci-siegen.de/) im Wintersemester 2015/2016 im Rahmen des [Seminars „3D-Druck“](http://fablab-siegen.de/lv-3d-druck-1516/) hergestellt haben.

Zu Beginn des Seminares wurden die Studierenden zunächst mit den Grundlagen der digitalen Fabrikation vertraut gemacht: Welche Fertigungsverfahren gibt es, welche Materialien können für den Druck genutzt werden, was sind mögliche Anwendungspotenziale? Zudem erfuhren sie mehr über die einzelnen Schritte des 3D-Drucks: von der Modellierung, über das Slicing (die "Übersetzung" eines 3D-Modells in Instruktionen für den Drucker), bis hin zum Druck an sich. Für die anschließende Projektarbeit beschlossen vier Studierende, sich dem Bau eines eigenen 3D-Druckers zu widmen.

![alt-text](http://fablab-siegen.de/content/images/2016/06/aya4.jpg)

Als Basis diente den Projektbeteiligten ein Bausatz, der die meisten Teile, die zum Bau benötigt wurden, bereits enthielt. Alle Baupläne sowie die Steuerungssoftware sind open source verfügbar und so bauten die Studierenden den Drucker zunächst nach Vorlage des Vertreibers. Schnell stellten sie jedoch fest, dass nicht alles einwandfrei funktionierte. Deshalb entschieden sie sich dafür, einige Gehäuseteile mit einem anderen 3D-Drucker im Fab Lab selbst zu drucken und führten weitere Änderungen durch, die die Druckqualität verbessern sollten, wie zum Beispiel die Anpassung des Halters für das Verbrauchsmaterial. Anschließend folge eine längere Kalibrierungsphase, denn die automatischen Unterstützungssysteme, die der Drucker hierfür eigentlich besitzt, funktionierten leider nicht ganz so gut wie gedacht.

Ein ganzes Semester arbeitet die Studierenden an dem Drucker, den sie AYA (nach einer japanischen Filmfigur) nannten. AYA ist ein Delta Robot 3D-Drucker, dessen Besonderheit in der Bauform liegt: Das dreigliedrigen Achsensystem, das sich von konventionellen Druckern mit linearen Achsensystem unterscheidet, ermöglicht einen schnellen, präzisen Druck. Neben kleineren Testdrucken wurden bereits die ersten größeren Drucke wie eine Eule oder eine Vase angefertigt. Erste Testläufe deuten daraufhin, dass AYA mit einer sagenhaften Geschwindigkeit von bis zu 300-350 mm/Sekunde drucken kann.

![alt-text](http://fablab-siegen.de/content/images/2016/06/aya_detail.jpg)

Auch wenn das Studienprojekt inzwischen abgeschlossen ist, wollen die Studierenden weiter an der Optimierung des 3D-Druckers arbeiten. Angedacht ist hier zum Beispiel der Verbau der Steuerelektronik oder die Stabilisierung des Grundgerüstes, um AYA transportabler zu machen. Zudem ist geplant AYA mit anderen Materialien wie zum Beispiel ABS - das ist der Kunststoff, aus dem zum Beispiel Legosteine bestehen - zu testen, denn bis jetzt wurde lediglich PLA, ein umweltfreundlicher Kunststoff, der auf (Mais-)Stärke basiert, als Material genutzt.

Die Studierenden selbst haben im Rahmen des Seminars und durch den Bau von AYA viel über 3D-Druck gelernt. Am [Tag der Technik](http://fablab-siegen.de/tag-der-technik/) wurde der Drucker bereits das erste Mal vor einer breiten Öffentlichkeit präsentiert und benutzt.

AYA in voller Größe: 
![alt-text](http://fablab-siegen.de/content/images/2016/06/aya.jpg)

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
