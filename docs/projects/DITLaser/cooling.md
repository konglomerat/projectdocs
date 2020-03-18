# Kühlung

* "Links zur Laserröhre 100W Modell":http://www.cncoletech.cn/Laser%20tuber%20long%20life.html .
* "Specs der Kühler die von den Herstellern unserer Laserröhre mitgeliefert werden":http://www.teyuchiller.com/Products/ChillerCW5000800Wcoo.html 0,015K/W

Die Laserröhre hat eine elektrische Leistung 672W=24.000V*28mA. Davon sollen etwa 100W als Laserstrahlung abgegeben werden. Es sind als 572W=672W-100W zu kühlen.
Im Datenblatt des Kühler aus der Lasersaur BOM sind 65 W/K bzw. 0,0153 K/W angegeben. Die Temperaturerhöhung ist also etwa T=572W*0,0153K/W=9K. Der maximale Durchfluss des Kühlers ist mit 15l/min angegeben.
Mit dieser Berechnung könnte also auch mit Wasseruhr, Stoppuhr und zwei Thermometern den Wirkungsgrad des Lasers messen und damit auf die Ausgangsleistung schließen. 

h1. Ideen zum Aufbau 

Mögliche gut verfügbare Wasser-Luft Wärmetauscher wären Autokühler oder Radiatoren von der Rückseite von Kühlschränken.
Auto Kühler haben ohne Lüfter ab 0,1K/W (kleiner ist besser) aber mit Lüfter haben selbst kleine Autokühler 0,018 K/W. Ein mittelgroßer Autokühler mit Lüfter ist also genauso gut wie das Aggregat aus der BOM. Für den Selbstbau braucht man also einen Autokühler aus einem Auto, Wasserpumpe, Temperaturreglung mit PWM des Lüfters und Notabschaltung bei Übertemperatur.

Links zu anderen Ideen

 * http://www.electricstuff.co.uk/lasercutter.html verwendet einen etwas größeren Heizungswärmetauscher aus einem Auto, dafür aber nur einen Lüfter
 * Wasserkühlung für PC (Overclocking Bedarf)


h1. Realisierter Eigenbau Kühler

h2. Grundaufbau 

Grundlage ist der Heizungswärmetauscher (Wasser->Luft) aus einem Wartburg, da dieser vorhanden war. Dieser war undicht und wurde gelötet. 
Um die Übertragungsfähigkeit zu erhöhen wurden auf dem Wärmetauscher 3 Stück 120mm PC Lüfter angebracht. Damit wird die gesamte Fläche des Kühlers abgedeckt.
Eine im Wasser Vorratsbehälter eingetauchte Aquariumspumpe sorgt für die Umwälzung des Wassers. Es wurden im Durchlauf durch die Laserröhre etwa 12l/min gemessen

h2. Test und Bemessung Kühlleistung

Zum Test der Kühlung wurde das Wasser statt mit dem Laser mit einem 1100W Tauchsieder erhitzt. 
Nach etwa 30min ergab sich ein thermisches Gleichgewicht mit einer Wassertemperatur von 42°C was 24K Temperaturerhöhung gegen die 18° Umgebungstemperatur ergibt. Der Kühler hat also rund 24K/1100W=0,022 K/W.
Bei maximal 572W des Lasers ergibt sich eine Temperaturerhöhung von 572W*0,022K/W=13K. Die Spec. der Laserröhre fordert maximal 40°C. Die Umgebungstemperatur bei Dauerbetrieb darf daher maximal 27°C sein. Wenn man den Kühler mit 6 statt 3 Lüftern betreibt (unten noch 3 Lüfter welche saugen statt blasen) sinkt der Wert noch mal auf rund 0,015K/W. Dies entspricht der passend zur Laserröhre angebotenen COLE TECH Kühlung mit auch 0,015K/W.

h2. Hinweise zur Kühlung 

  * Bei den Laserröhren aus Glas sind die Kühlwasseranschlüsse einer der Schwachpunkte, die häufig abbrechen. Es ist also wichtig die Schläuche möglichst ohne Kraft und nur einmal aufzuschieben und danach immer nur am anderen Ende abzuziehen. Auch ev. Schlauchschellen sollten dort sehr vorsichtig festgezogen werden. 
  * Wenn man die Laserröhre zum Beispiel für einen Transport ausbaut sollten nur kurze Schlauchstücke an der Röhre verbleiben um keine großen Kräfte durch die Masse der Schläuche auszuüben. Um dies zu realisieren und auch um mögliche Kräfte abzufangen, sollte man an der Befestigung der Laserröhre je ein kurzes Rohrstück für Vorlauf und Rücklauf unterbringen, so das man von den Rohrstücken mit möglichst kurzen Schläuche zu den Anschlüssen der Laserröhre kommt. Für diese kurzen Stücke wären hochflexible Silikonschläuche mit mittlerer Wandstärke sinnvoll.

h2. Ideen zur Überwachungsschaltung

*Ist aktuell noch nicht realisiert.*

Für die Notabschaltung der Laserröhre bei Überhitzung des Kühlwassers wurde ein kleiner Bimetallschalter aus einem Akkupack herausgesucht. Der Schaltet bei 45°C von ZU auf AUF und soll in Reihe zum Ansteuersignal des Lasers geschleift werden. Das Kühlwasser des Lasers soll laut Spec. max. 40°C sein. Unklar ist jedoch ob sich dies auf Einlass oder Auslass bezieht. Die Notabschaltung am Wasserauslass der Röhre bei 45°C sollte aber ganz gut dazu passen. Ein Schalter im Bereich 35-40°C wäre besser. 
Da diese Lösung rein mechanisch arbeitet, sollte nach einem Test mit einer Heißluftpistole auf den Sensor diese Schaltung auch nicht versagen.
Kritischer ist die Überprüfung ob die Pumpe läuft. Wenn die Pumpe nicht läuft, wird auch das warme Wasser nicht zum Bimetallschalter gepumpt und er löst nicht aus. Es gibt einen größeren rein visuell anzeigenden Durchflussmesser. Diesen können man mit einem Magneten auf dem Flügelrad und einem Hallsensor (Aus Lüfter oder Fahrradtacho) umbauen.
Per µC könnte dann eine genau Temperaturmessung mit 2-stufiger Warnung und Abschaltung und eine Durchflussmessung zum Überwachung der Pumpe gebaut werden. 
Zusätzlich stellt sich die Frage ob noch eine zusätzlich "robuste" diskrete Überwachung der Durchmessmenge ohne µC aufgebaut werden soll. Möglich wäre ein einstellbarer, retriggerbarer Monoflop.

h2. Fazit

Wir haben eine dauerhafte, einfache Lösung für den Kühler welcher noch die Überwachungsfunktionen und das Gehäuse fehlen. Ein direkter Nachbau ist schwierig, da die Grundlage ein nicht mehr hergestellten Ersatzteil eines DDR Autos ist. Ein Motorrad oder kleiner Autokühler zusammen mit etwa 3 guten 120mm Lüftern sollte ausreichende Kühlung für einen Laser mit 100W optischer Ausgangsleistung ergeben.

h2. ToDo

 * Überwachung der Wassertemperatur und abschalten des Lasers wenn die Temperatur über der zulässigen Maximaltemperatur der Laserröhre von 40°C liegt
 * Überwachung der Durchflussmenge (Pumpenausfall) und abschalten des Lasers bei ungenügender Durchflussmenge.   
 * Optional Anzeige von aktueller Wassertemperatur und Durchflussmenge
 * Gehäuse für Iteration der Kühlung unter dem Tisch

