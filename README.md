# Z-Probe
Z-Längentaster für CNC-Maschinen, kapazitiv

Empfindlichkeit wird von C1 bestimmt - kleinere Werte ergeben größere Empfindlichkeit. LED1 leuchtet bei Berührung der Schaltfläche auf (Berührung zum Test mit dem Finger). 

Die Schaltung kann mit +5V oder +12V bis +24V versorgt werden. Bei 5-V-Versorgung ist JP3 zu überbrücken. Höhere Betriebsspannungen sind möglich, wenn man R7..R9 durch den Wert 2k2 ersetzt.

Üblicherweise sollte JP1 für eine negative Logik (Ausgang schaltet bei Berührung nach Masse) überbrückt sein. Sollte die CNC-Steuerung eine positive Logik (Ausgang normal auf Masse, bei Berührung offen bzw. "high") verlangen, ist stattdessen JP2 zu überbrücken.

Bitte beachten Sie den Artikel in Make: 1/2016.

Carsten Meyer
