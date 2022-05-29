# Arbeiten mit Virtuellen Maschinen

## Analyse der Hardware der Virtuellen Maschine

+ Der Nutzer sollte als root agieren
+ Um sich Informationen über die Hardware zu verschaffen können folgende Befehle verwendet werden

|Befehl|Funktion|
|-|-|
|lspci -v|Gibt Informationen zu allen PCI-Bussen und Systemen im Gerät aus|
|lsusb -v|Gibt alle USB Geräte aus, die mit dem Rechner verbunden sind|
|cat /proc/cpuinfo|Gibt den Inhalt der Datei cpuinfo aus|
|ip a|Zeigt die ip Adresse an|

## Anlegung eines Festplattenplatzes für eine Virtuelle Maschine

+ Der Speicher kann in einer Datei auf dem Originalen Betriebssystem angelegt werden
+ Der Speicher kann direkt auf der Festplatte durch eine Partition festgelegt werden (Hoher aufwand)

## Anlegen eines Virtuellen Laufwerkes auf einem FAT23 System

+ Beim anlegen eines virtuellen Laufwerks muss beachtet werden, dass diese nur 4 GByte große Dateien unterstützt
+ Größere Festplatten müssen unterteilt werden

## Kritischste Ressource bei mehreren Gast Betriebssystemen

+ Der Arbeitsspeicher(RAM) ist am wichtigsten

## Hardware in der Virtuellen Maschine

+ Der Virtuellen Maschine wird die Hardware nur vorgespielt
+ Dies macht es leichter die Virtuelle Maschine auf ein anderes System zu verlagern
+ Die Virtuelle Maschine besitzt zudem eine eigene MAC-Adresse

## Virtuelle Netzwerk-Verbindungen

|Art|Funktion|
|-|-|
|Host-Only|Eigenes Netzwerk zwischen Host und Guest|
|Bridged|Host und Guest hängen beide an einem virtuellen Switch. Der Guest bekommt eine IP-Adresse vom DHCP-Server des Klassenraums|
|NAT|Der Guest bekommt eine private IP-Adresse vom Host zugewiesen. Der Host setzt dann nach außen hin diese private IP-Adresse auf seine eigene um|