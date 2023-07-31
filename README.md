# ss_v2
Soldering Station v2 Projekt

Das Soldering Station v2 Projekt basiert auf dem SolderingStation Projekt: https://github.com/ConnyCola/SolderingStation.
Da dieses Projekt nun schon einige Jahre alt ist und mir ein paar kleine Tweeks wie USB-C input oder User-Buttons fehlen, ist dies somit die inoffizielle Fortsetzung.
Der Code basiert maßgebend auf dem des Originalprojekts. 
Hinzugefügt wurde:
- User-Buttons Funktionen (speichern, abrufen und löschen von selbst festgelegten Temperaturwerten)
- Automatisches Standby, wenn PWM über gewisse Zeit einen Wert nicht überschreitet
- Menü, um obriges einzustellen

Die Schaltung basiert ebenfalls auf dem Originalprojekt, wobei hier einige Änderungen vorgenommen wurden:
- Der uC (Atmega328p) wird direkt integriert.
- Es werden drei programmierbare Nutzer-Buttons hinzufügt, z.B. für voreingestellte Temperaturen oder Standby.
- Über einen Pin kann mit einem Federkontakt der Lötkolben automatisch in den Standy gesetzt werden, wenn er in die Halterung gelegt wird.
- Es gibt nun eine AVR-ISP-Schnittstelle zur Programmierung.
- Der OpAmp wurde durch ein günstigeres Modell ersetzt.
- Es gibt neben dem bisherigen Rundstecker auch einen USB-C Anschluss, der Power Delivery (USB-PD) unterstützt.
- Ein Kippschalter wird eingesetzt, um zwischen Rundstecker und USB-C zu schalten um somit reverse-current zu verhindern.

ToDo:
Der gesamte Programmierteil sowie ein Prüfen der Schaltung.
