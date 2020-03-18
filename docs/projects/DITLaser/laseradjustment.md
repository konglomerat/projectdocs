# Laserstrahljustierung

## Hinweise

  * Thermopapier verwenden um Strahlprofil abzubilden 
  * http://www.pulslaser.de/index.php?datei=Allgemeines/optik/optik.htm&datei2=navigation/left_allgemein.htm
  * Zur Einstellung der Linse und den Fehler dabei siehe die Erklärung unter

    * http://www.buildlog.net/blog/2013/05/why-are-my-laser-cut-edges-not-straight/
    * Dies erklärt auch den Fehler mit den schrägen Kanten welche wir an den fuer den Laser auf dem Epiloglaser gefertigten Teilen gesehen haben 

   
## Dimensionierung Strahlengang 

  * Der Lasersaur hat einen sehr einfachen Strahlengang mit einem fixen und zwei beweglichen Spiegel welche um jeweils 90° ablenken. Eine Aufweitung des Strahl findet nicht statt. 
  * Links zum Strahlengang des Lasersaur http://www.lasersaur.com/manual/optics_setup  
  * Auf der Webseite wurden bis jetzt keine Hinweise zur Berechnung der Aufweitung des Strahlengangs gefunden
  * Ziele und Hinweise bei der Dimensionierung
  * Laserstrahl

    * Der aus dem Laser austretende Strahl hat einen bestimmten Durchmesser. Der Stahl ist außerhalb nicht 0 sondern die Intensität von der Mitte zum Rand folgt in etwa einer Gaussverteilung.
    * Der Laserstrahl ist häufig etwas elliptisch, ein typischer Wert ist 20% Abweichung von der Kreisform
    * Der austretende Laserstrahl ist nicht exakt parallel sonder weitet sich mit der Zeit auf (Divergenz)  
    * Da die Spiegel die Leistungsdichte des Laserstahls aushalten müssen, sollte wegen diesem Punkt der Stahl so weit aufgeweitet wie möglich sein
    * Da die Spiegel und Linsen nur einen Maximalen Durchmesser haben, sollte der Stahl nicht stärker als dieser Durchmesser ausgeweitet sein, da der Anteil der Energie welche außerhalb liegt verloren ist.    
    * Da der Strahl mit zusätzlicher Entfernung ausgeweitet ist die maximale Länge des Strahlengangs gegrenzt
    * Auch die minimale Länge des Strahlengang ist begrenzt. das heißt die Entfernung Laser zu Linse darf nicht beliebig kurz sein. Ein Ansatz zur Erklärung ist im EVO 100 Datenblatt
    * Meist ist bei den Chianlasern jedoch kein Datenblatt zu finden, so das außer Außenabmessungen und Laserleistung auch kein Wert garantiert wird und alle Berechnung nur mit angenommenen Werten durchgeführt werden können
    * Ohne entsprechende Strahlqualität lässt sich die Laserleistung nicht durch Fokussierung mit der Linse in Schnitttiefe umsetzten. 
    * Weiterhin sind in den Foren genügend Klagen zu lesen, das die angegebene Laserleistung nicht erreicht wird. 
    * 
