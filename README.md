# hm_fbh
HomeMatic Script zur Steuerung einer Fussbodenheizung

Aufbau:
TempRegler Typ 7xHM-TC-IT-WM-W-EU
Switch     Typ 2xHM-LC-Sw4-DR

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


