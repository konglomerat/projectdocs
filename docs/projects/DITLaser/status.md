# Status Übersicht

Hier findet ihr unseren persönlichen Lasersaur Bauplan, der sich an der offiziellen Anleitung  ( http://labs.nortd.com/lasersaur/manual ) von nortd lab orientiert, aber inzwischen nicht mehr ganz so kleine Modifizierungen besitzt. Das heißt unser persönlicher Bauplan entsteht mit mit dem Aufbau des DIT:LASERS und dient gleichzeitig als Übersicht des aktuellen Baustandes.

!!! warning "Laser aktuell in Testphase!"

## Zu beschaffende Posten

Siehe [Zu beschaffender Posten](supply.md)

### Material was gekauft wurde aber noch nicht abgerechnet

  * 150€ Rechnungen für PC Platten
  * 200€ für Kompressor
  * 7,50€ Schrauben 100 Stück M4x8 Linsenkopf 

## Status quo

Zustand komplett bis auf die ToDo

### Prio 1a (notwendig für Probebetrieb)

 * *S* Senkung der G0 Geschwindigkeit im LinuxCNC Config von 30000 mm/min auf 3000 mm/min
 * *M* Gehäuse geschlossen, Metallplatten hinter direkten Strahlengang 
 * *E* Laser darf bei "PC Aus" nicht an gehen
 * *D* Dokumentation für Betrieb
 * *E* Lüfter für SM Treiber
 * *E* Sicherheitsschaltung überprüfen
 
### Prio 1b (für Probebetrieb schnellstmöglich nachrüsten)

 * *M* Abluft bleibt dauerhaft am Fenster (zumindest im Sommer)
 * *S* Trajectory Control im Visicut
 * *E* Betriebsminutenzähler
 * *D* Wartungsplan und Dokumentation Wartung
 * *R* neuer Kompressor sollte ein ähnlicher Typ wie beim Zinq sein
 * *D* FAQ und Materialsammlung für potentielle Nutzer

### Prio 1c (für langfristigen Betrieb)

 * *D* Kontakt mit anderen Lasersaur Nutzern zum Erfahrungsaustausch
 * *E* nach GND Verbindung beim Parallelport, Test Maximalgeschwindigkeit, 
 * *M* Spannvorrichtungen für die Zahnriemen bauen, nach neueren besseren (breiteren) Zahnriemen recherieren (ev die vom aktuellen Lasersaurstand) und Umlenkrollen auch durch Zahnriehmenräder ersetzen 
 * *M* Laserbett anheben und neu justieren
 ** Das Wabengitter sollte etwa 0,5mm-1mm unter der Obefläche enden.
 ** Die rechte obere Ecke des Wabengitters (Anschlag für Platten, sollte genau auf dem Nullpunkt liegen!)
 ** Größe des Laserbereichs optimieren), Schleppkette schlägt manchmal an nachträglich eingebauten Halter für die Stangen an
 * *M* Schleppkette der X-Achse zu steif und wird manchmal nach innen gedrückt,
 ** aktuell arbeiten die Schrittmotoren im Halbschrittbetrieb, werden die Stufen bei µ-Schritt besser? , wegen der begrenzten Geschwindigkeit des Parallelport reduziert dies jedoch die max. Geschwindigkeit  
 * *M* Laserkopf immer noch nicht lotrecht
 * *E* Notaus während Fahrt zerstört SM Treiber? 
 * *E*, *S* Wenn in Linux CNC Pause gedrückt wird, halten die Achsen an aber der Laser (Spindel) bleibt an, das ist für eine Fräse ok aber beim Laser besteht Brandgefahr
 * *E*, *S* Je nachdem ob eine Position von links oder rechts Angefahren wird, kommt es zu einer Abweichung in y-Richtung. Es werden jedoch keine Schritte verloren 
 * *D* Dokumentation 
   * Justagevorgang
   * Materialsammlung
   * Sicherheitshinweise
   * Bedienung 
 * *D* Beschluss Nutzungskonzept
 * *R*, *E* Maschinensicherheit, Laserschutzbeauftragter, Zulassung
 * *R* Klärung der rechtlichen Grundlagen und Risiken für "Normalbetrieb"
 * *D* Lasergala für "offizielle" Einweihung und Übergang zum Normalbetrieb



### Prio 2 (Upgrades im Normalbetrieb)

 * *S* Test Trajectory control, Linux CNC arbeitet als Fräse, Kurven werden in Geraden zerlegt, bei jeder Gerade wird von v=0 beschleunigt und am Ende wieder auf v=0 abgebremst. danach folgt die nächste Gerade. Während dessen ist der Laser aber mit konstanter PWM an, dies führt zu Verbrennungen am Anfang und Ende von jeder Gerade. Dies für zu einem "Perlenketteneffekt" also einer sehr rauen Oberfläche. Wählt man in VisiCut eine niedrige dpi Zahl sind die Geraden lang bei höheren dpi Zahlen kurz. Um dies zu beheben müsste man entweder per Zusatzschaltung die Momentangeschwindigkeit messen und darauf die Laser PWM anpassen oder eine ander Steuerung wählen welche mit konstanter Geschwindigkeit fährt. In Ecken von kleinen Winkel bleibt das Problem mit den Verbrennungen in diesem Fall aber bestehen.
 * *E* Freischaltung, Abrechnungseinrichtung
 * *E* Neue SM Elektronik [[Update Elektronik]] und  Umstellung Ansteuersoftware  ?
 * *S* Gravieren, es gibt schon andere Gruppen die das gravieren für den Lasersaur umgesetzt haben. Die Implementierung setzt ev. neue SM Elektronik voraus da die Geschwindigkeit sonst ev. zu niedrig ist. 
 * *M* *E* Motofocus (Z-Achse), Karlsruhe will auch eine bauen http://wiki.fablab-karlsruhe.de/doku.php?id=projekte:uebersicht
 * *E* Kühlung Überwachungsschaltung, Gehäuse
 * *H* Filterung
 * *H* Untertisch zum Lagern von Material[[wiki:projekte:bauen:dokumentation:bauplan:untertisch|Status]]
 * *E* Ausstattung der Achsen mit Indexmessstreifen z.B. aus alten A3 Druckern um zumindest in einem kleinen Bereich, die Position genau messen und das Umkehrspiel durch die Dehnung der Zahnriemen ausgleichen zu können. Ziel ist eine Erhöhung der Präzision. Dies setzt ein Einlesen der Daten in eine schnelle Verarbeitungseinheit (schneller µC oder FPGA) voraus. Das gesamte Projekt sollte so angelegt sein, das die Ergebnisse auch für andere Maschinen (Fräse) zu verwenden sind.
 * *M* Passstifte in Rahmen des Laserbetts, welche es Erlauben Platten umzudrehen und noch einmal von der anderen Seite mit gespiegelten Daten zu lasern, damit sollte sich die maximale Dicke deutlich verbessern lassen

### Legende

* *D* okumentation
* *E* lektronik
* *H* olz
* *M* echanik/ *M* etall 
* Internet *R* echerche
* *S* oftware

