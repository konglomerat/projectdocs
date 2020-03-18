# Materialien

## Übersicht

 * Sammlung von bearbeitbaren und nicht bearbeitbaren Materialien, sowie Einstellungen und Hinweisen
 * es besteht keine lineare Abhängigkeit von Laserleistung zu Geschwindigkeit, die Daten von anderen Lasercuttern sind also nur bedingt vergleichbar
 * Metalle lassen sich mit unseren Lasern nicht schneiden oder direkt gravieren, es ist möglich einen Lack mit dem Laser strukturiert einzubrennen um Metallteile zu beschriften. 
 * PVC und Polycarbonat gehen nicht zu lasern
 * Die maximale Materialstärke ist etwa 20mm für Acryl und Balsasperrholz für alle dichteren Materialien z.T. deutlich weniger  

## Links zu anderen Materialsammlungen

 * "Happylab":http://wiki.happylab.at/w/Laser_Cutter#Materialien
 * "FabLab München":http://wiki.fablab-muenchen.de/pages/viewpage.action?pageId=1802248 
 * "RWTH Aachen":http://hci.rwth-aachen.de/lasercutter
 * "ATX":http://atxhackerspace.org/wiki/Laser_Cutter_Materials
 * "Dingfabrik Köln 50W":http://wiki.dingfabrik.de/index.php/Lasersaur_(Lasercutter)http://wiki.dingfabrik.de/index.php/Lasersaur_(Lasercutter) 

## Sammlung getesteter Materialien 

### Erklärung Parameter

 * "100%" Laserleistung etwa 100W 
 * a=5mm gibt den Abstand von der Materialoberfläche zur Laserkopf an z.B. 5mm
 * Fxxxx Geschwindigkeit in mm/min
 ** Die Geschwindigkeitsangabe z.B. "F200" kommt vom G-Code  bedeutet 200 mm/min
 ** Die maximale Geschwindigkeit ist F15000 also 15000 mm/min
 ** In Visicut stellt gibt man die Geschwindigkeit in % der Maximalgeschwindigkeit an. 100% sind also F15000, 50% F7500, 10% F1500 usw.

 
### Kunststoffe

 * Anleitung zur Bestimmung unbekannter "Kunststoffe":http://hackaday.com/2015/03/14/how-to-identify-plastics-before-laser-cutting-them/
 * Identification of "Polymers":www.chymist.com/Polymer%20Identification.pdf 
PMMA, Acryl, Plexiglas (nicht mit PC verwechseln) getestet bis 12mm mehr sollte möglich sein
 * 0.1mm, 70%, a=8mm, F1500 (Folie Laserdrucker für Overhead), eignet sich für Schablonen u.ä.  
 * 6mm, 100%, a=5mm, F500
 * 10mm, 100%, a=4mm, F300
 * 12mm, 100%, a=4mm, F150 (F200 nicht überall ganz ganz durch)
 

#### Polymid, Nylon

 * https://www.eurolaser.com/de/materialien/polyamid-pa/

h3. Polystyrol

 * dünne Platten ca. 3mm fest kein Schaum, Kanten werden unsauber, riecht stark nach Klebstoff, weißer Niederschlag auf Wabengitter, lasern möglich aber unerwünscht

 
### Hölzer

* Leimholzplatte Fichte 18mm 100%, F200, a=1mm
* Kiefer 15mm 100%, F200-F300, a=1mm je nach Dichte der Hölzer, bei Aststücken auch F200 zu wenig, markieren mit 50% und F3000 
 

### Holzverbundstoffe

#### OSB Platte

* 16mm F100-F200, a=1mm  Kanten deutlich verbrannt

#### Sperrholz

* Birke 5mm, 100%, F1500, a=10mm 
* Kiefer 6mm von Hornbach, 100% F300, a=10mm (Brandspuren, an manchen Stellen nicht ganz durch. aufgegeben. Vermutlich schlechter Leim)
* Pappel 6mm, 100% F900, a=5mm
* ????? 8mm, 100%, F120, a=5mm (F150 an machen Stellen nicht ganz durch)

#### HDF

 * 6mm, 100%, F800, a=10mm

#### MDF

 * 3mm, 100%, F1500, a=5mm lasert gerade so durch
 * 3mm, 100%, F1200, a=5mm, lasert sicher durch
 * 3mm, 50%, F1000, a=20mm, markieren lasert machmal an Umkehrpunkten leicht durch

#### Siebdruckplatte

 * 12mm, 100%, F250, 1. Durchgang F=10mm, 2. Durchgang F=1mm, sehr starke Verbrennungen nicht zu empfehlen
 * 12mm, 100%, F50, F=1mm, sehr starke Verbrennungen nicht zu empfehlen
 
#### Pappe und Papier

 * 1,5mm Finpappe, S100+F3000 gut durch, S20+F3000 zum markieren (für bessere Kantenqualität G64 Parameter und Speed ändern)

### Glas

 * garvieren und markieren möglich
 * Entspiegeltes Glas aus Scanner, F90, S100, a=10mm, starkes Plasma scheidet aber teilweise Glas durch, ein Riss läuft aber beim Schneiden unkontrolliert vom Startpunkt los
 * bis jetzt keine Parameter für nur anritzen zum Brechen, entweder unkontrollierbare Risse (zu viel Intensiät) oder kein brechen an der Schnittkante (zu wenig Intensität?) 

### Textilien

 * Dünner Baumwollstoff, schneiden, 30%, F1500, a=8mm,  Absaugung und Druckluft reduziert
 * Dünner Baumwollstoff, schneiden, 18% oder 19% (Einstellung sehr kritisch), F1500, a=8mm,  Absaugung und Druckluft reduziert

### Keramik und mineralische Stoffe

  * Porzellan unglasiert (Unterseite Teller),markieren 100%,F1500,a=5mm
  * Beton, markieren, a=7mm erzeugt dünnste Linie, 56%, F1000, a=7mm erzeugt sehr dünne feine Linien, etwas außer Focus und mehr Leistung erzeugen breite unregelmäßige Linien (ca. 0,5mm breit) 
  * Keramik von Leiterplatten- (nimmt zwar Energie auf, wird aber zersprengt auch bei minimalen Energieeintrag)

### Spezialmaterialien

#### GFK glasfaserverstärker Kunststoff (Platten)

 * GFK 2mm Glassfasermatte mit PA66, S100+F900, F=5mm, 4 bis 5 Durchgänge mit gleichem Focus, 3 Bar Durchluft über Komressor, Kantenqualtität mittel, *für eine entgültige Freigabe muss noch die Gesundheitsbeeinträchtigung genauer geprüft werden!* Dies hängt auch vom als Binder verwendetten Harz/Kunststoff ab
 * -GFK 2mm Glassfasermatte mit PA66, S100+F250, F=2mm, Fasern gehen durch, Material verschmiltzt jedoch wieder leicht. Teil lässt sich trotzdem trennen. Kanntenqualtität "schlecht"- 

#### CFK kohlefaserverstärkter Kunststoff (Platten)

 * -CFK 2mm Platten (Prepeg mit 50% PA66), S100+F1000, F=5mm, 3 Bar Durchluft über Komressor, 50 Durchgänge aber nur zu 80% durchgeschnitten, erwartete Kantenqualität schlecht- (weitere Tests nötigt)

#### Sandpapier und ähnliche

 * 3M Safty-Walk, F=8mm, S100, F1000, durch


### Gravieren und markieren von Metallen

 * kein direktes gravieren von Metallen möglich 
 * Gravieren mit Speziallack 1 Dose rund 100€
 * Gravieren mit "Auspufflack"
    * mit Lack einsprühen, nicht trocknen lassen
    * auf Lasersaur mit S100, F150, a=5mm einbrennen
    * nicht ausgehärteten Lack mit Alkohol (Spiritus) entfernen  
    * getestete Lacke Farbturm Hitzefest Sprühlack, schwarz hitzefest, (Hitzebeständig bis 650°C), Rühl Industrie_Baumarkprodukte Argentur GmbH 

## Mögliche aber ungetestete Materialien

Folgende Materialien wurden noch nicht getestet, sollten jedoch nach Erfahrungen von Anderen möglich sein

### Holzbasiert

 * Wellpappe
 * Holzfurnier
 * Balsaholz
 * Korkplatten
 * ABS

### Textilien aus Naturstoffen

Generell hohe Brandgefahr!

 * Leinen 
 * Jeansstoff
 * Leder
 * "Flece":http://wiki.fablab-muenchen.de/display/WIKI/Fleece+lasern+bzw.+gravieren 

### Kunststoffe

 * Mylar Folie (Siebdruck z.B. für Lötpaste)
 * POM Polyoxymethylen, Delrin, 
 * Kapton Folie, Polyimide 

### Spezial und Verbundmaterialien

 * Capa(TM) line (PU Schaum Verbund)
 * ausgehärteter Fliesenkleber (Flexkleber mit Polymeranteil), markieren, F750, S100, 5mm Focus (sichbar, weniger Speed für deutlichere Konturen)


### Spezielle Materialeigenschaften

 * verspiegeltes Acryl z.B. Ikea DRÖMMARE 160x500mm 4€    
 * Magnetmatten
 * Sandpapier von Rückseite
 * Schelllackplatten (Schalplatten von vor 1945), *jedoch keine Schallplatten nach 1945 aus Vinyl !*

## Noch nicht genauer untersuchte Materialien

Sollten prinzipiell mit CO2 Lasern bearbeitbar sein, es ist jedoch nicht geklärt ob giftige Gase entweichen oder die Materialien entflammen können   

 * Neopren, "Aachen":http://hci.rwth-aachen.de/lasercutter dagegen andere führen Neopren z.T. auf Listen 
 * PES Polyester
 * PE Polyethylen
 * PUR Polyurethan
 * verschiedene Gummiwerkstoffe
 * Kohlefaser Matten (nicht schon fertige Platten) 
 * Glassfasermatten
 * Graupappe "Aachen":http://hci.rwth-aachen.de/lasercutter dagegen  
 * Teflon (PTFE) "München dagegen":http://wiki.fablab-muenchen.de/pages/viewpage.action?pageId=1179992 
 
## Hoch problematische Materialien

Bei diesen Materialien ist bekannt, dass sie sehr große Probleme verursachen. Bevor sie probiert werden können, muss eine genaue Recherche sowie Tests mit kleinen Stücken erfolgen.  

 * Polystyrol, Polystyrene, Styropor Schaum (sehr feuergefährlich, ev. mit Opferplatten Oben und Unten )  
 * Silikonfolien (z.B. Backunterlagen) für Dichtungen (schmilzt ev. und verdreckt Laserbett, Opferplatte unterlegen?)
 * ABS (schmilzt, ev. Opferplatte unterlegen) 

## Nicht laserbare Materialien

 * Materialien welche bei der Zersetzung CO2 emittieren
 ** PC, Polycarbonat  
 * Metalle
 * Materialien welche Halogene wie Chor, Brom (Flammschutzmittel) und Fluor enthalten
 ** PVC, Vinyl
 ** PTFE, Teflon enthält Flur, erzeugt gesundheitsgefährliche Gase siehe https://en.wikipedia.org/wiki/Polymer_fume_fever

 * welche die maximale Dicke von etwa 20mm überschreiten 
 * leicht entzündlich sind
 ** Zelluloid (Filme vor 1950) aber auch Tischtennisbälle, Teile von Musikinstrumenten u.ä.
 * Giftige Gase emittieren
 ** "Bakelit":http://www.baubegriffe.com/Bausachverstandiger_Holzmann-Bauberatung/Blog/Eintrage/2011/10/11_122_Schadstoffe_die_unser_Leben_beeinflussen.html 

## Generelle Abhängigkeiten

### Allgemein

 * Bestimmte Materialien wie Sperrholz emittieren beim zersetzen CO2, die CO2 "Wolke" absorbiert die Laserleistung und es entsteht ein hell leuchtendes und sehr heißes Plasma welches die Oberfläche verbrennt. Dies sollte man vermeiden in dem man mit Druckluft die "Wolke" weg "pustet" .
 * der beim Verbrennungen entstehende Kohlenstoff "imprägniert" die Oberfläche und verhindert damit weitere Abtragungen
 * Verschiedene Materialien wie PMMA emtitieren Gase, welche im Schnittspalt wie eine Wellenleiter wirken und zum "selbstfokussieren" des Strahls führen. Dies führt dazu, das die optimale Fokusentfernung je nach Material unterschiedlich ist.    
 * Auf verschiedenen Stellen des Laserbetts hat der Laser vor der Linse einen unterschiedlichen Durchmesser, dadurch wird der Laser unterschiedlich fokussiert und die Schneidleistung ist unterschiedlich, bei großen Objekten vorher testen ob auch an allen Ecken das Material durchgeschnitten wird
 * Ist der Strahlengang des Lasers nicht richtig justiert sinkt die Schneidleistung z.T. extrem, dies betrifft schon kleine Änderungen z.B. am Laserkopf
 * Verschmutze Spiegel verringern die Schneidleistung
 * Auch von außen gleich aussehendes Material kann sich unterschiedlich verhalten. Verschiedene Sperrholzarten weichen z.T. extrem von den Schneidparametern ab

### Einfluss Druckluft 

 * Mit einem angepassten Luftzug kann man die CO2 Wolke verdünnt werden, so das weniger Plasma und damit Verbrennungen entstehen
 * Druckluft kühlt das Material und verhindert das Schmelzen
 * Druckluft facht entstandene "Verbrennungen" an. Stickstoff statt Luft könnte dies verbessern. 
 * Druckluft kann kleiner Objekte weg wehen
 * Pumpen von anderen Lasercuttern verwenden Pumpen mit  0,4 Bar, bei Tests an unserem Laser war ab etwa 2 Bar keine weitere Verbesserung zu sehen
 
## Recherchen von Materialien für Spezialanwendungen

### Elastomere für Dichtungen

  * normaler Gummi je nach Laserleistung nur bis etwa 0,5-3mm schneidbar
  * sinnvolle Dicke meist im Bereich 0,5mm..5mm

#### Suchbegriffe

 * seal, gasket,O-ring

#### Typen von Elastomeren

#####  "Gummi" schwarz (rubber), SBR, BUNA-S

 * Dichtungsgummi 2mm v=1% P=100% http://wiki.happylab.at/w/Laser_Cutter#Materialien
 * Gummi 1,6mm wird bei 40W nur halb durch geschnitten https://www.youtube.com/watch?v=BSzqBjXv2Ek 
 * Gummi schwarz 2mm v=100% P=20% (deckt sich nicht mit anderen Angaben) http://hci.rwth-aachen.de/lasercutter
 * Quellen
 ** 1/2/3mm http://www.modulor.de/Kunststoff-Gummi/Platten-Matten-Folien/Synthetische-Elastomere/Vollgummi-Dichtungsplatte-schwarz.html

##### Lasergummi

##### EPDM

 * gut schneidbar
 * bis etwa 120-150°C
 * nicht beständig gegen Mineralöl, Benzin
 * Quellen
 **  2x300x300 13,40€ https://www.fabstore.at/index.php?route=product/category&path=3_24 
 ** 0,6x1500xL 13,90€/m http://www.modulor.de/Kunststoff-Gummi/Platten-Matten-Folien/Synthetische-Elastomere/Dichtungsfolie-Gummi-schwarz.html

##### Silikon

 * gut schneidbar schmilzt jedoch leicht ->Schneidleistung reduzieren
 * bis etwa 180°C, flexibel auch bei tiefen Temperaturen
 * chemisch sehr beständig aber je nach Typ anfällig auf Mineralöl, Benzin
 * Silikon rot 2mm v=13% P=40% http://hci.rwth-aachen.de/lasercutter
 * Quellen
 ** http://www.modulor.de/Kunststoff-Gummi/Platten-Matten-Folien/Synthetische-Elastomere/Silikonplatte-opak-farbig.html
 ** http://www.modulor.de/Kunststoff-Gummi/Platten-Matten-Folien/Synthetische-Elastomere/Silikonplatte-transluzent-farblos.html

##### NBR, HNBR, BUNA-N

 * beständig gegen Mineralöl, Benzin
 * Quelle http://www.alibaba.com/showroom/laser-cut-nbr%252fnr-industry-rubber-sheet.html
 ** http://www.eurolaser.com/de/anwendungen/muster/dichtungsmaterial

##### Gummimatten aus Gummigranulat

Plasma vermeiden, schnell aber wiederholt schneiden
Die gleiche Stelle braucht sehr lange zum abkühlen

 * 8mm Matte, porröse Gummimatte aus Granulat, S100, F4000, Focus 12mm, 5x schneiden etwa 3mm, 20x schneiden etwa 6mm, durchschneiden schwirig
 * Fahrradschlauch, S100, F2000, Focus 8mm, gute Ergebnisse, schneiden von Dichungen und ähnliches möglich 
