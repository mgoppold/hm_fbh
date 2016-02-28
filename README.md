# hm_fbh
HomeMatic Script zur Steuerung einer Fussbodenheizung

##Installation


## Aufbau:

* TempRegler Typ 7xHM-TC-IT-WM-W-EU
* Switch     Typ 2xHM-LC-Sw4-DR

Stellmotoren stromlos geschlossen an HM-LC-Sw4-DR

Im Script sind die Seriennummern anzupassen. Diese werden aus
Performancegründen nicht über die Namen gesucht.

Die Räume werden mit 2 Buchstabigen Prefix gekennzeichnet
WZ,KU,FU,BZ,SZ,GZ,AZ

WZ .. Wohnzimmer
KU .. Küche
FU .. Flur
BZ .. Bad
...

Für das Logging wird CUxD benutzt.

##ToDo

- [ ] XX_Temp_Offset als 2 Variablen Sysvar mit
   - [x] 1. Wert Offset vor Soll aus
   - [ ] 2. Wert Offset unter Soll an
- [ ] debug Ausgaben auf einer einzigen Zeile zusammenbauen und am Ende ausgeben (Reduzierung der I/O)
- [ ] Zeiten messen die vergeht vom Einschalten bis erreichen der Solltemp.
  - [ ] Kann XX_Temp_Offset irgendwie berechnet werden?
- [x] SystemVar Arbeitstag_heute und Feiertag_heute nutzen um Wochenprogramm zu setzen 1 Arbeitstage 2 Urlaub/Feiertag ( -> eigenst. Programm)
- [x] itimeout = 1800 als Systemvar
- [x] idebug = 0,1,2,3 als Systemvar
- [x] sLogPrefix abhängig von osrc setzten
- [x] roffset pro Raum setzten (als Systemvar WZ_Temp_Offset)
