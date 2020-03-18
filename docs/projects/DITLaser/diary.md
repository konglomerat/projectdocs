# Bautagebuch

## 9.3.2017

* Einstellung Skalierung der x und y Achse, da vorher kleine Abweichungen(501,5mm statt 500mm) ev. auf Grund des gespannten Zahnriemens vorhanden waren.
* Dauertest für etwa 1,5h mit voller Laserleistung
* Max. Geschwindigkeit in der Software jetzt 3000 mm/min 

## 16.03.2017

 * Test eines kleiner Airbrush Kompressors, Ergebnis: laut, zu wenig Luftvolumen

## 23.03.2017

 * Test des Kompressors vom Zing Laser am Lasersaur liefert sehr gute Ergebnisse, dieser Kompressor ist sehr leise, ein ähnlicher Typ sollte verwendet werden
 * Test PMMA 8mm: Sehr gute Schnittkanten, Speed 300mm/min 
 * Test mit Sperrholz 

## 27.03.2017
 
 * Lasern von HDF 12mm rund 

## 5.4.2017

 * Ausbau des internen kleinen Kompressors, die geschaltete Leitung wird auf eine Netzbuchse auf dem Anschlusspanel geführt 
 * Reflexionen (Schatten neben Schnitt) in der Laserdüse nach neuer Justage beseitigt
 * Test 3mm MDF 1500/1200mm/min

## 23.04.2017

 * Zahnriemen für die X-Achse nachgespannt, danach war der Fehler mit dem Nullpunktversatz weg und es konnte wieder mit 3000mm/min gearbeitet werden

## 27.04.2017

 * Löcher unten in Laserbett
 * Nassreinigung Gitter und Laserbett 
 * die Zahnriemen der Y-Achse springen und die X-Achse bekommt einen Versatz. Danach hat es rund 1h gedauert den Laser wieder neu zu justieren. Die Riemen der Y-Achse müssen also auch nachgespannt werden. Vorher müssen wir sie aber kürzen. Bis dahin wieder in der Linux CNC Oberfläche die max. Geschwindigkeit auf 1600 mm/min begrenzen. 
 * Mit der langsameren Geschwindigkeit für die Leerfahren lief der Laser Gestern aber auch 300 Minuten ohne Probleme durch. 5mm MDF bei S100, F600
 
## 4.5.2017

 * Test markieren von Feinsteinzeug Fliesen und Beton ->geht gut
 * Test von schneiden und ritzen von dickerer Pappe ->geht gut
 * Defekt an Y-Achse, SM rattert nur noch (1 Phase defekt), Ursache war ein "selbstausgelöteter" Shunt Widerstand
 * merkwürdige Logikpegel auf X-Step und Y-Step, Masse(GND) des Parallelport war nicht verbunden (Masse für über Gehäuse, Schutzleiter). *Es wurde noch nicht getestet ob die Logikpegel nachher  ok waren!* 

## 17.08.2017

 * Die Linse war gesprungen. Durch falsche Justage des Laserstrahls traf der Laserstrahl auf die Gummidichtung am Rand des Spiegels im Laserkopf. Der verbrennende Gummi hat die Linse mit einem schwarzen Belag bedampft. Dadurch hat die Linse einen großen Teil der Laserleistung absorbiert und war gesprungen. Linse wurde getauscht. 
 * Y Achse schräg, beseitigt
 * Laser neu justiert
 * Test Kohlefasermatte 2.2mm dick mit F250, Focus 2mm. Fasern gehen durch, Material verschmiltzt jedoch wieder leicht. Teil lässt sich trotzdem trennen. Kanntenqualtität "Mittel" bis "schlecht" für die die meisten Anwendungen wahrscheinlich trotzdem brauchbar.
* Test Maximalgeschwindigkeit etwa 400mm/s für X und Y Achse

## 18.10.2017

  * Die Acryl Teile der Y Achse (Aufnahme Kugellager) waren gerissen. Diese wurden durch ALU Teile ersetzt. Die 2. Befestung der Achse wurde entfernt.
  * Speedtest ergab folgende Werte
     * alt 50 mm/s und 400 mm/s²
     * X-neu 400 mm/s (Fehler bei 500 mm/s) und 10000 mm/s² (Fehler bei 12000 mm/s²)
     * Y-neu 400 mm/s 3000 mm/s²  (Fehler bei 3500 mm/s²) 
  * Test Laserjustage ok



 

