# Übersicht DIY-Laser

Im Internet finden sich eine ganze Reihe von Lasercutter-Selbstbau- und Umbau-Projekten, sowie mehr oder weniger gute Bauanleitungen. Die ausschließliche Online-Recherchen unsererseits, brachten allerdings nur mäßig brauchbare Ergebnisse. Denn bei der Auswahlentscheidung helfen vor Allem Details, welche jedoch in den meisten Fällen kaum bis gar nicht beschrieben sind.

Aus diesem Grund entschlossen wir uns dazu, zwei Laserbauprojekte in Köln und Hamburg zu besuchen und mit Hilfe der gesammelten Erfahrungen zu entscheiden. Einen ausführlichen Reisebericht könnt ihr an folgender Stelle downloaden oder auch online lesen:


## DIT-LASERBAU-KLASSENFAHRT

Dresden-Köln-Hamburg-Berlin/Potsdam-Dresden. vom 29.-31. März 2013. 

[Reisebericht](attachments/reisebericht_-_klassenfahrt_dit-laserbau.pdf)

http://www.phase0.org/inside-view/reisebericht-einer-dit-laserbau-klassenfahrt


Auf dieser Wiki-Seite möchten wir die gängigen Laserbauprojekte mit ihren spezifischen Vor- und Nachteile auflisten. 
Mitarbeit erwünscht!

## Buildlog Laser 

http://Buildlog.net

Der Buildlog Laser 

*PRO:* günstig (ca. 1000€ bis 1500€), gut dokumentiert, oft gebaut 

*CONTRA:* Arbeitsfläche kleiner als Lasersaur (30cm x 50cm), Community vorrangig in USA, Stückliste nicht metrisch vorhanden

## Lasersaur 

* http://labs.nortd.com/lasersaur/
* "Google Group Lasersaur":https://groups.google.com/forum/#!forum/lasersaur


*PRO:* sehr gut dokumentiert, oft nachgebaut, aktive Communnity, grosse Arbeitsfläche(170cm x 117cm), durch die Größe sind hohe Laserleistungen möglich (100 Watt) was auch die Bearbeitung stärkerer Materialien zulässt, Stückliste für Europa vorhanden 

*CONTRA:* teuer (ca. 6000€), standardmäßig nicht fürs Gravieren ausgelegt (Gravieren noch in der Entwicklung)

### Klassenfahrt Erfahrung - Lasersaur Dingfabrik 

Im Unterschied zur offiziellen Bauanleitung und anderer Berichte aus dem Internet, besteht der spezifischen Aufbau des begutachteten Lasersaur aus folgenden Abänderungen und Speziallösungen:

  * Die dringend benötigte Absaugung ist in der Beschreibung des Lasersaur nicht vorhanden. Ein Hüpfburggebläse als Absauganlage erweist sich als ideal, der selbstentwickelte und selbstgebaute Wasserfilter, dagegen als nahezu wirkungslos.
  * Die bei dem Lasersaur mitgelieferte Elektronik und dazugehörige Software stellte sich als ungeeignet bis funktionsunfähig heraus und wurde durch eine eigene Variante ersetzt. Diese unterscheidet sich zum Original wie folgt:

    * _Nortd Labs Original:_ Verwendet eine selbstentwickelte Platine mit einem Atmega328 auf dem grbl läuft welches die Schrittmotoren  ansteuert. Als CAM-Modul wird die LasaurApp auf einem Beaglebone verwendet
    * _Dingfabrik Modifikation_: Verwendung von LinuxCNC zur Ansteuerung der Schrittmotoren. Als CAM-Modul wird eine modifizierte Version der LasaurApp verwendet. Das bedeutet eine komplett neu entwickelte einfachere Schaltung wurde verwendet und die nötigen Berechnungen auf einem externen PC durchgeführt.

  * Die Laserröhre wurde durch eine kleiner Laserröhre mit 60Watt ersetzt. Die Röhre ist auch keine LongLife-Röhre. Lasersaur verwendet laut original Teileliste eine 100W “LongLife”-Röhre. (Ersparnis: 1500€)
  * Die original Laser-Optik wurde durch eine fertige aus China ersetzt, bezogen über Ebay. Ersparnis: ca 500€


## Umbau China-Laser

*PRO:* wenig Arbeit, günstig (1300€ plus 100€ Umbau) 

*CONTRA:* wenig dokumentiert, sehr klein (Arbeitsfläche 30cm x 20cm), Umbau der Elektronik nötig (eingebaute Elektronik ist schlecht und nur mit gelieferter Software zu betreiben) → Umbau auf Laos-Laser

### Klassenfahrt Erfahrung - Umbauprojekt in Hamburg 

Von dem China-Fabrikat wurden Elektronik und Software komplett eliminiert und durch Alternativen ersetzt (Software: VisiCut, Hardware: Laos Board - beides Open Source). Die original Elektronik (Moshiboard) ist nur mit der schlechten original Software (verdongelt) zu nutzen. Um den Laser vernünftig zu verwenden muss die Elektronik getauscht werden. Aber auch die Software der neuen Elektronik (Open Source) hat, trotz ständiger Verbesserung leider ihre Makel. Dies konnten wir bei einem Test auch sehen. Hierbei fuhr der Laserstrahl quer durch das Werkstück, auch von anderen erratischen Bewegungen des Lasers wurde berichtet. Von der mechanischen Qualität des China-Lasers waren wir ebenfalls sehr enttäuscht. Trotzdem konnten wir sehen das auch dieser Laser fähig ist, feine Zahnräder auszuschneiden und saubere Schnitte zu machen. Aber die schlechte Qualität der Laser-Komponenten, z.B. fehlende Feingewindeschrauben, die umständliche Bedienbarkeit und die kleine Schnittfläche (in dieser Version etwa A4), machten die Option des Umbaus im Vergleich zum Neubau für unsere Zwecke schnell unattraktiv. 

## 3D-Printable Laser Cutter

http://www.thingiverse.com/thing:11653

## blackTooth 

http://buildyourcnc.com/blackToothLaserCutterAndEngraver.aspx

  * 40W 

## Andere (DIY) Lasercutter

### Andere Lasersaur

* "Chemnitz":http://fablabchemnitz.de/2015/09/16/lasercutter-cameo/ Zing 40W, 0,80€/1,60€ 
* "Dingfabrik Köln":http://wiki.dingfabrik.de/index.php/Lasersaur_(Lasercutter) 
  * 50W, etwa 8mm Acryl, 0,10€/min intern, 0,50€/min (extern), 
  * Software: Laserapp
* "Karlsruhe":http://wiki.fablab-karlsruhe.de/doku.php?id=projekte:lasersaur-overview
* Berlin "Berlinasaurus":https://groups.google.com/forum/#!topic/lasersaur/3ewSp7Pq2F8
  
### Andere Lasercutter in Fablabs
* Zing mit Visiut, 0,65€/0,80€ "Hamburg":http://www.fablab-hamburg.org/2011/12/27/howto-lasercut/
* Zing 30W, "München":http://wiki.fablab-muenchen.de/pages/viewpage.action?pageId=1179992
* "NY":https://wiki.nycresistor.com/wiki/Laser 


## Lasersicherheit

* kritischer Vergleich der "Lasersicherheit von DIY Lasern":http://www.laserlady.org/2015/08/26/katastrophenlaser-laserkatastrophen/

