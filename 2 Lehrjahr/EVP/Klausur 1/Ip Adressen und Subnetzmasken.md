# Ip Adressen und Subnetzmasken
 
## Netzwerkadressierung

+ Ein Protokoll der Netzwerkschicht muss gewährleisten, dass jeder Knoten mit jedem anderen Knoten kommunizieren kann.
+ Damit ein Knoten eindeutig identifizierbar ist, wird die Ip Adresse verwendet.
+ Eine Ip-Adresse kennzeichnet ein Interface, wobei jedes benutzte Interface seine eigenen Ip Adresse besitzt.
+ Eine IPV4 Adresse besteht auf vier Bytes
+ Die Bytes werden in Dezimalzahlen umgewandelt und durch Punkte voneinander getrennt.
+ So zum Beispiel **11.88.3.100**
+ Eine IPV4 Adresse besteht aus einem Netzteil und einem Host Anteil
+ Hosts die sich im gleichen Netz befinden haben den gleichen Netzanteil, jedoch einen andren Host Anteil in ihrer Ip Adresse.
+ Die Höchste und die kleinste Host Adresse können nicht an einen Host vergeben werden, da die kleinste Adresse als Netzadresse und die grösste als -Broadcastadresse verwendet wird.

## Angabe des Netzanteils

1. Man hängt die Binäre Position des Netzanteils mit einem Slash an die Ip Adresse zb. **11.88.3.100/16**. Die 16 verweist auf das 16 bit.
2. Es wird eine Netzwerkmaske verwendet, welche in einem byte nur Einsen, oder Nullen verwendet.
Die Position wo nur Nullen sind gehören zum Host und die Stellen wo nur Einsen sind gehören zur Netzmaske.

## Host Formel
+ Die Host formell gibt an, wie viele host bei einer bestimmte subnetzmaske erlaubt sind
+ Die Formel lautet ***2^h-2***
+ ***h*** steht hierbei für die Anzahl der Nullen in der Subnetzmaske

## Subnetz Formel
+ Die Subnetzformel gibt an, wie viele Subnetze für eine Subnetzmaske vergeben werden können
+ Die Formel lautet **2^s**
+ ***s*** steht hierbei für die Anzahl der Einsen die zur Subnetzmaske hinzugefügt werden

## Öffentliche und Private Ip-Adressen
+ Öffentliche Ip-Adressen dienen zur Interaktion mit dem Internet
+ Private Ip-Adressen werden innerhalb eines lokalen Netzwerks verwendet
+ Private Ip-Adressen werden für die Kommunikation zwischen Geräten im selben Netz verwendet
+ Die öffentlichen Ip-Adressen fallen in den Rahmen

|Start|Ende|
|-|-|
|1.0.0.0|9.255.255.255|
|11.0.0.0|126.255.255.255|
|129.0.0.0|169.253.255.255|
|169.255.0.0|172.15.255.255|
|172.32.0.0|191.0.1.255|
|192.0.3.0|192.88.98.255|
|192.88.100.0|192.167.255.255|
|192.169.0.0|198.17.255.255|
|198.20.0.0|223.255.255.255|


## Quellen
+ [Vernetzte IT-Systeme: 27](https://intranet.rbbk-dortmund.de/~heimann/buecher/vernetzte_it_systeme_a4/seite027.gif)
+ [Computer Weekly.de](https://www.computerweekly.com/de/tipp/IP-Adressen-und-Subnetze-Wie-man-IPv4-Subnetzmasken-mit-der-Host-Formel-berechnet)
+ [Avg.com](https://www.avg.com/de/signal/public-vs-private-ip-address)


