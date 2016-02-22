![GitHub Logo](http://www.heise.de/make/icons/make_logo.png)

Maker Media GmbH und c't, Heise Zeitschriften Verlag

***

# Z-Probe
Z-Längentaster für CNC-Maschinen, kapazitiv

Empfindlichkeit wird von C1 bestimmt - kleinere Werte ergeben größere Empfindlichkeit. LED1 leuchtet bei Berührung der Schaltfläche auf (Berührung zum Test mit dem Finger). 

Die Schaltung kann mit +5V oder +12V bis +24V versorgt werden. Bei 5-V-Versorgung ist JP3 zu überbrücken. Höhere Betriebsspannungen sind möglich, wenn man R7..R9 durch den Wert 2k2 ersetzt.

Üblicherweise sollte JP1 für eine negative Logik (Ausgang schaltet bei Berührung nach Masse) überbrückt sein. Sollte die CNC-Steuerung eine positive Logik (Ausgang normal auf Masse, bei Berührung offen bzw. "high") verlangen, ist stattdessen JP2 zu überbrücken.

Layout für doppelseitige Platine als Gerber- und PDF.Dateien. Infprmationen für Selberätzer: Rückseite vollständig Kupfer als Massefläche, zwei Durchkontaktierungen aus Kupferdraht nötig. Bohrungen für Steckverbinder ggf. auf Rückseite freikratzen.

Z-Probe-Eingang bei der aktuellen Version der GRBL-JOG-Firmware ist Pin 5 (PB4, SPI SS) des ATmega644. Dieser Eingang ist an PL7 (ISP) Pin 3 zugänglich. Für erhöhte Störsicherheit sollte ein Pull-up-Widerstand 4k7 nach +5V und ggf. ein Eingangsfilter wie an den anderen Schalter-Eingängen vorgesehen werden. Eine überarbeitete GRBL-JOG-Platine ist in Planung.

Bitte beachten Sie den Artikel in Make: 1/2016.

Carsten Meyer, Redaktion Make:
