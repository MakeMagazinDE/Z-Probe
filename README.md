![GitHub Logo](http://www.heise.de/make/icons/make_logo.png)

Maker Media GmbH und c't, Heise Zeitschriften Verlag

***

# Z-Probe
Z-Längentaster für CNC-Maschinen, kapazitiv

Die Schaltung kann mit +5V oder +12V bis +24V versorgt werden. Bei 5-V-Versorgung ist JP3 zu überbrücken. Höhere Betriebsspannungen als 24V sind möglich, wenn man R7..R9 durch den Wert 2k2 ersetzt.

Die Empfindlichkeit wird von C1 bestimmt - kleinere Werte ergeben höhere Empfindlichkeit. LED1 leuchtet bei Berührung der Schaltfläche auf (Berührung zum Test mit dem Finger). Sobald die (parasitäre) Kapazität an der Schaltfläche größer wird als C1, spricht die Schaltung an. Bei durchgehender Massefläche auf der Rückseite (doppelseitige Platine) ist die Kapazität der Elektrode nach Masse von sich aus schon recht hoch. C1 sollte dann mit 22p bemessen werden. 

Üblicherweise sollte JP1 für eine negative Logik (Ausgang schaltet bei Berührung nach Masse) überbrückt sein. Sollte die CNC-Steuerung eine positive Logik (Ausgang normal auf Masse, bei Berührung offen bzw. "high") verlangen, ist stattdessen JP2 zu überbrücken.

Layout für doppelseitige Platine als Gerber- und PDF-Dateien. Informationen für Selbstätzer: Rückseite vollständig Kupfer als Massefläche, zwei Durchkontaktierungen aus Kupferdraht nötig. Ggf. zwei Bohrungen für Steckverbinder auf Rückseite freikratzen.

Z-Probe-Eingang bei der aktuellen Version der GRBL-JOG-Firmware ist Pin 5 (PB4, SPI SS) des ATmega644. Dieser Eingang ist an PL7 (ISP) Pin 3 zugänglich. Für erhöhte Störsicherheit sollte ein Pull-up-Widerstand 4k7 nach +5V und ggf. ein Eingangsfilter wie an den anderen Schalter-Eingängen vorgesehen werden. Eine überarbeitete GRBL-JOG-Platine ist in Planung.

Bitte beachten Sie den Artikel in Make: 1/2016.

Carsten Meyer, Redaktion Make:
