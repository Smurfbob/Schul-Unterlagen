# Virtuelle Netze

## Übersicht 

+ Es gibt drei Möglichkeiten ein Virtuelle Maschine in ein Netzwerk einzubinden
1. Bridged Network: Direkte Verbindung zum LAN
2. NAT: Subnetz mit Host-Zugriff

## Bridged Network

+ Bei dem Bridget Network wird eine direkte Verbindung zum LAN aufgebaut.
+ Bei dieser Anbindung ist die VM aus der Sicht des Netzwerks nicht von einem Physischen Rechner zu unterscheiden
+ Diese Art der Verbindung wird of für Server verwendet
+ Der Virtuelle Netzwerkadapter wird hierbei mit dem Namen des Physischen Adapters konfiguriert

## NAT
+ Bei dieser Verbindung kann der Host mit den VMs über ein Netzwerk Daten austauschen und optional als Router fungieren
+ Bei der Option "Host-only" fällt die Router Funktion weg und es kann nur der Zugriff auf den Host gewährt werden

