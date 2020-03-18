# DY13

Das Lasernetzteil ist relativ dürftig Beschrieben "z.B. hier":http://www.recilaser.com/en/productInfo/fc9181e93b448cac013b44fba49f0f2a.htm

h2. Ansteuerung

Eigene Versuche haben folgendes ergeben:

* Anschluß 1 (5V) ist der 5V-Ausgang der für die Steuerung des Netzteils verwendet werden kann.
* Anschluß 5 (G) ist Masse.
* Anschluß 4 (WP) muss mit Masse (5) verbunden werden. Nur dann schaltet ein internes Relays das Netzteil ein.
* Anschluß 6 (IN) steuert den Ausgangsstrom der Hochspannungsquelle von 0 bis 28 mA durch eine Steuerspannung von 0 bis 5 V. Dazu kann ein Potentionmeter verwendet werden.
* Die Anschlüsse 2 (TH) uns 3 (TL) arbeiten wie folgt:
<pre>
  TH  TL  Power
  LO  LO  100%
  LO  HI  10%
  HI  LO  100%
  HI  HI  100%
</pre>

Für die Ansteuerung mittels PWM bei einer Frequenz von < 20 kHz muß die PWM für den Anschluß 6 (IN) in eine Gleichspannung umgewandelt werden.
Ab 20 kHz glättet die Laserröhre selbst die PWM. Diese Frequenz ist aber mittels LinuxCNC nicht einstellbar.

Ich habe zwei in Frage kommende Schaltungen entprechend simuliert (siehe die angehängende Dateien).


## PWM

* [PWM_FILTER_01.pdf](attachments/PWM_FILTER_01.pdf)
* [PWM_FILTER_02.pdf](attachments/PWM_FILTER_02.pdf)