# DHCP Server

## Übersicht

+ DHCP ermöglicht es Clients ohne ein manuelle Konfiguration in ein bestehendes Netz einzubinden
+ Informationen wie die Ip-Adresse, die Netzmaske, das Gateway, oder der Name des DNS Servers werden automatisch vergeben

## Server
+ Der DHCP Server selbst besitzt Informationen über den zu vergebenen Adresspool, die Subnetzmaske, die lokale DNS-Domain, oder das GateAway

## Möglichkeiten der Nutzung

### Statische Zuordnung

+ Bei der statischen Zuordnung werden die Ip-Adressen bestimmten MAC-Adressen fest zugeordnet.
+ Einer der Nachteile hierbei ist, das das Netz nicht mehr erweitert werden kann

### Automatische Zuordnung

+ Im DHCP Server wird ein Bereich von Ip-Adressen definiert
+ Die Ip Adressen werden automatisch auf die MAC-Adressen verteilt und in einer Tabelle fest gehalten
+ Eine einmal zugeteilte Ip-Adresse bleibt immer mit der MAC-Adresse verbunden
+ Sobald der gesamte Adressbereich vergeben ist, können keine weiteren Clients dem Netzwerk beitreten

### Dynamische Zuordnung

+ Bei der Dynamischen Zuordnung werden die Ip-Adressen wie bei der Automatischen Zuordnung vergeben, werden jedoch nur für einen gewissen Zeitraum verliehen
+ Der Client muss sich in einem gewissen Zeitraum zurück melden, sofern dieser die Ip-Adresse behalten möchte
+ Macht der Client dies nicht wird die Ip wieder frei und kann an jemand anderen weiter gegeben werden