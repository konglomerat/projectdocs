# Mechanik

  * Der mechanische Aufbau des Laser folgt weitgehend der nicht mehr aktuellen Version (EU v13.04) des Lasersaur siehe http://labs.nortd.com/lasersaur/manual/hardware
  * Die bis jetzt bestellen Teile umfassen die wichtigsten Teile von der Misumi BOM aus der Laussaur Anleitung http://labs.nortd.com/lasersaur/bom-suppliers-eur

h2. Upgrade Y-Achse
 
 * Die Y-Achse war in der Vergangenheit die Quelle vieler Probleme, die Riemen haben sich mindestens 20mm gelängt und durch die schräg stehende Achse traten Folgefehler auf. Jetzt sind die Acrylteile der Aufhängung gebrochen. Deswegen soll unbedingt ein Update vorgenommen werden. Welches folgende Eigenschaften hat.
   * ersetzen von Arcylteilen durch ALU
   * integrierte Vorrichtung zum spannen der Zahnriehmen, ev. sogar Feder für definierte Vorspannung
   * Verbesserung der nur einfach gelagerten Achse aus Version 13.04 entweder durch neue Version des Lasersaur oder durch Eigenentwicklung
   * Gegenlager auch durch Zahnriemenscheibe und nicht durch Kugellager 
   * erheblich höhere Zugspannung des Zahnriemens damit er sich nicht mehr längt
   * Eventuell Einbau der Untersetzung am Schrittmotor (gleiches Übersetzungsverhältnis)
  
h3. alter Stand Lasersaur v13.04
   * Keine Untersetzung am Schrittmotor, 2x Zahnriemen 5,08mm Pitch, Antriebsträder 12 Zähne, da=12*5,08mm=60,96mm 
   * 2x, Zahnriemen XT, 350 Zähne, 6,35mm Breite, Länge 1778mm, max Zugspannung 60N
   * Preise Zahnriemen 48€, 2xAntriebsräder 24€,  

h3. neuer Stand Lasersaur v17.03
   * Untersetzung am Schrittmotor 22 auf 60 Zähne 
   * 2x Zahnriemen 3mm Pitch "Powergrip" GT3 9mm breit
   * 2x Antriebsräder GPA20GT3090-A-P6, 20 Zähne, 15.26€/Stück  
   * Gesammtübersetzung  = 22/60*3mm*20=22mm
   * 
     


h2. Geschwindigkeit

Laut  https://groups.google.com/forum/#!topic/lasersaur/_E55zobwTKA
"I will build a lasersaur but a tube 100w and too big for me, ... lasersaur still has some resonance issues if you're going faster then 2000mm/min."

aktuell sind die folgenden Werte konfiguriert:

<pre>

<property name="xmaxacc" type="float" value="600.0"/>
<property name="xmaxvel" type="float" value="450.0"/>

<property name="ymaxacc" type="float" value="600.0"/>
<property name="ymaxvel" type="float" value="450.0"/>

</pre>

https://github.com/Fablab-Dresden/ditlaser-linuxcnc_config/blob/master/ditlaser.stepconf

h2. Motoren

  * Motoren wurden mit Elektronik getestet Typ siehe http://labs.nortd.com/lasersaur/manual/steppers
  * X-Achse wurde grob eingestellt. Je fester der Zahnriemen eingestellt wir um so höhere Geschwindigkeiten sind möhlichk bevor er rutscht. Die Einstellung der Spannung des Zahnriemens hat aber Verbesserungsbedarf. Folgendes Teil ist eine alternative Aufnahme für den Lasersaur (US und wahrscheinlich auch ältere Version) http://www.thingiverse.com/thing:29884

h2. Gehäuserahmen

!http://uk.misumi-ec.com/material/mech/MSM1/PHOTO/10302683830.jpg! http://uk.misumi-ec.com/vona2/detail/110302683830/  HFS5-2020


h2. Gehäuseverkleidung 

Die Maße der Beplankung für die gebaute Version 13.04 sind unter http://labs.nortd.com/lasersaur/bom-1304-subsystems-eur beim Punkt Frame-Panels

Ursprünglich vorgesehen waren folgende Platten

  * 1x Mount Panels rear bottom right NortdLabs la-mpan 71.0 0.00 
  * 1x metal sheet 1166x356x0.8mm left side Misumi PDSPHC4H-1166-356-0.8-F1110-G340-N5-UN10-XC8-YC8 41 41.00 
  * 2x metal sheet 1166x847x0.8mm bottom Misumi PDSPHC4H-1166-847-0.8-F1150-G790-N5-UN10-XC8-YC9 54 108.00 
  * 1x metal sheet 247x216x0.8mm right side Misumi PDSPHC4H-247-216-0.8-F190-G200-N5-UN10-XC9-YC8 24 24.00 
  * 2x metal sheet 847x200x0.8mm front Misumi PDSPHC4H-847-200-0.8-F790-G180-N5-UN10-XC48-YC8 33 66.00 
  * 2x metal sheet 847x268x0.8mm rear top Misumi PDSPHC4H-847-268-0.8-F790-G250-N5-UN10-XC48-YC8 33 66.00 
  * 2x metal sheet 847x356x0.8mm rear Misumi PDSPHC4H-847-356-0.8-F790-G340-N5-UN10-XC48-YC8 36 72.00 
  * 1x metal sheet 917x356x0.8mm right side Misumi PDSPHC4H-917-356-0.8-F900-G340-N5-UN10-XC8-YC8 38 38.00 
  * 2x polycarbonate sheet 847x156x3mm door cover front Misumi PCTBA-847-156-3 24 48.00 
  * 2x polycarbonate sheet 892x847x3mm door cover top Misumi PCTBA-892-847-3 100 200.00 

Aus Kostengründen (etwa 200€ statt 800€) und da die Stahlbleche gestrichen werden müssten ,wurden die Teile der Beplankung nicht mit bei Misumi bestellt und einige Änderungen vorgenommen. Dabei müssen Brandschutz (z.B. kein PC für Boden) und Lasersicherheit beachtet werden. Gleichzeitig sollten ausreichet Schrauben verwendet werden um den LaserSaur mit den Platten weiter auszusteifen und dicht für die Absaugung und die Lasersicherheit zu bekommen. Für einige Versionen und Platten gibt es Bohrschablonen zum Ausdrucken auf der Webseite.  

*Geplantes Vorgehen*

  * Es wird eine Polycarbonatplatte mit **2050x1250x3mm** für 75€ bei Amazon bestellt
  * Daraus werden die Polycarbonatplatten mit im Vergleich zur Anleitung V.13.04 geänderten Maßen gesägt.
  * Die genauen Maße werden am Prototypen angerissen und vor Ort auf der Kreissäge gesägt  

    * Deckel oben aus PC 2x 892x847mm wird 1x 1700x892mm
    * Klappe vorn aus PC 2x 847x156mm  wird 1x 1700x156mm
    * Damit bleiben bei 2mm Schnittbreite noch  PC Reste von 1700x198mm und 1250x348mm 
    * Front unten statt Blech 0,8mm 2x847x200mm wird der PC Rest 1700x198mm verwendet ->optisch attraktiver, da    Front komplett transparent (**Achtung da kein Verschnitt bleibt beim Anreißen genau auf die Breite des Sägeblatts achten und die Maße der gelieferten Platte vorher kontrollieren **)
    * Boden laut Anleitung Blech mit 0,8mm und 2x847x1166 statt dessen wird der Lasersaur mit der Grundfläche von 1700x940 auf einen größeren Tisch mit ???x??? geschraubt. Die Tischplatte aus Aludibond bildet den Boden des Lasersaur.  
    * Seiten: Das Blech auf der linken Seite wird wie auf der rechten Seite geteilt. Die Bleche für die Anschlüsse werden nach innen versetzt um die angesteckten Kabel und Schläuche zu schützen. 

      * Die Bleche für die Anschlüsse sind fertig aus dicken Alu 
      * Rechts: Anschlüsse für Strom mit extra Kaltgerätebuchsen für die externen Geräte (PC, Monitor, Lüfter Absaugung, Kühlung Aggregat, Kühlung Pumpe, ev. Druckluft extern) sowie Parallelport zur Steuerung 
      * Links: 2x Anschlüsse für Kühlschläuche 

    * Es werden M5 statt M6 Schrauben mit Kragen für die Beplankung verwendet, statt Nutensteinen werden dünne M5 Messingmuttern in die Nuten eingeschoben (Ersparnis 80€) 

  * *Noch offene Teile der Beplankung*

    * Bestellung PC Platte
    * Die Rückwand mit **2x847x356** kann auch zu einer Platte mit etwa 1700x356 zusammengefasst werden. Das Material ist relativ egal Blech >0,8mm, Al >1mm, PC >3mm, Aludibond  >1,5mm wäre möglich. Hier können Reste mit schlechter Oberfläche verwendet werden, da der Laser an der Wand stehen soll
    * Hinten oben statt **2x847x268** kann auch eine Platte mit 1700x268 verwendet werden, das Material ist relativ egal Blech >0,8mm, Al >1mm, PC >3mm, Aludibond  >1,5mm wäre möglich. Bei PC wäre die Röhre von oben zu sehen, damit könnte man das Funktionsprinzip zeigen dies ist gegen die bessere Lasersicherheit von Alu abzuwägen
    * Seiten

      * Im Gegensatz zur Anleitung Links genauso geteilt wie Rechts
      * 2x kleine Bleche für Seite oben, hinten links und rechts noch genau ausmessen und etwa **2x 250x270** ALU >1mm bevorzugt (links wegen Lasersicherheit [ohne Spiegel volle 100W], rechts wegen einheitlicher Optik)
      * Große Platten für Seiten rechts und links etwa **2x917x356mm**, Material wie oben aber wenn möglich einheitlich Rechts und Links. Der PC Rest 1250x348mm wäre oben und unten 4mm schmaler ->prüfen ob verwendebar
      *  
   

h2.  Wabengitter - honeycomb 

  * fehlt in BOM des Lasersaur, teuer
  * im WSL ist eine kleine Platte mit etwa 1/2 Fläche etwa 900x600 aber sehr stark verschmutzt  
  * Paul fragt bei Messinghaus,  Matti bei Metallbau Seidel Freiberg
  * eventuell durch gespanntes Metallgitter, dünnen Maschendraht ersetzten (Kaninchendraht)
  * http://www.plascore.com/honeycomb-cores-aluminum.php etwa 35€ für die benötigte Größe

h2. Recherchequelle

https://github.com/nortd/lasersaur/wiki/Aluminium-honeycomb \\
http://www.lasersaur.com/manual/accessories

*Eigenstabil:*

http://www.ebay.com/itm/MILL-SILVER-Aluminum-Eggcrate-1-2-Cells-2-X-4-NEW-/260798102979?pt=LH_DefaultDomain_0&hash=item3cb8c73dc3

*Komprimiert:*

http://easycomposites.co.uk/products/core-materials/19mm-aluminium-honeycomb.aspx\\
Komprimiertes Wabengitter kann einfach auseinander gezogen werden. Man müsste dann Vorkehrungen treffen die Arbeitsfläche eben zu halten.

h2. Optimierungen

  * Es gibt schon Ideen (H-Bot) zur Optimierung des Antriebs diese sollen aber erst nach Abschluss der Inbetriebnahme angegangen werden