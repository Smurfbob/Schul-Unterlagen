# OSI Modell

## Funktion

+ Es gliedert komplexe Vorgänge in einzelne Schritte (eigentlich: Schichten). Jeder dieser Schichten wird eine bestimmte Aufgabe zugeschrieben und sie werden übereinandergestellt – so wird garantiert, dass die Kommunikation zwischen PCs und ähnlichen Endgeräten herstellerunabhängig und -übergreifend funktioniert.
+ Das Modell wird sehr häufig als Referenz herangezogen, wenn es darum geht, Abläufe einer Kommunikation oder Nachrichtenübermittlung exemplarisch darzustellen.
+ OSI steht für Open Systems Interconnection, also ein „offenes“ System für Kommunikationsverbindungen und Vernetzung.

## Aufbau des OSI Modells
+ Das OSI Modell gliedert sich in sieben Schichten.
+ Jede dieser Schichten hat eine explizite Aufgabe im Bezug auf das Senden und Empfangen von bestimmten Daten.
+ Jeder Nutzer, der an einer Kommunikation beteiligt ist, besitzt diese sieben Schichten auf seinem Gerät.
+ Die Schichten arbeiten eng miteinander zusammen und liefern Daten an die nächste, oder empfangen welche von der vorherigen Schicht.

## Aufbau der Schichten

+ Es gibt sieben Schichten im OSI Modell, welche auch als Layer bezeichnet werden.
+ Merkspruch: "Please Do Not Throw Salami Pizza Away"

### 1 Physical Layer / Bitübertragungsschicht
+ Umwandlung der erhaltenen Bits in ein zum Medium passenden Signal, abschließend die physikalische Übertragung
+ Hierbei kommen elektrische und mechanische Funktionen zum Einsatz.
+ Die Übertragung kann leitungsgebunden, oder auf leitungslosen Wege verlaufen

#### Protokolle
+ Ethernet
+ Token
+ Ring
+ FDDI
+ V.110
+ X.25
+ Frame Relay
+ V.90
+ V.34
+ V.24

### 2 Data-Link-Layer / Sicherungsschicht
+ Segmentierung der Pakete in sogenannte Frames und Hinzufügen von Prüfsummen
+ Die Bits aus der ersten Schicht werden in Blöcke unterteilt (Frames)
+ Diese Frames bekommen eine Prüfsumme, über welche der Empfänger die Richtigkeit dieser Frames bestimmen kann
+ Der Empfänger kann zudem den Sender anweisen, mit welcher Geschwindigkeit dieser seine Informationen sendet.

#### Protokolle
+ LLC/MAC
+ X.75
+ V.120
+ ARP
+ HDLC
+ PPP

### 3 Network-Layer / Netzwerkschicht
+ Routing der Datenpakete zum nächsten Kommunikationsknotenpunkt

#### Protokolle
+ IP -> Ist für die Korrekte Adressierung zuständig
+ IPX
+ ICMP
+ T.70
+ T.90
+ X.25
+ IPV6
+ NetBEUI
 
### 4 Transport-Layer / Transportschicht
+ Teilt Daten einer Anwendung zu

#### Protokolle
+ TCP -> Stellt die Verbindung zwischen Application und Transport her
+ UDP
+ SPX
+ NetBEUI

### 5 Session-Layer / Sitzungsschicht
+ Steuerung der Verbindungen und des Datenaustauschs

#### Protokolle
+ FTP
+ HTTP
+ SMTP
+ NNTP
+ NetBIOS -> Stellt unter Windows die Verbindung zur Transportschicht her
+ TFTP

### 6 Presentation Layer / Darstellungsschicht
+ Systemabhängige Daten werden in ein unabhängiges Format umgewandelt

#### Protokolle
+ Telnet
+ FTP
+ HTTP
+ SMTP
+ NNTP

### 7 Application-Layer / Anwendungsschicht
+ Liefert Funktionen für Anwendungen sowie die Dateneingabe und Ausgabe

#### Kommunikation in der Anwendungsschicht
+ In der Anwendungsschicht dient die Url als Identifikation für einen Computer
+ Diese Url wird dann zu einer IP-Adresse umgewandelt
+ Zur Ermittlung einer IP-Adresse durch eine Url wird ein DNS verwendet

#### Protokolle
+ Telnet
+ FTP
+ HTTP
+ SMTP
+ NNTP

## Anwendungsschichten
+ Unter die Anwendungsschichten fallen die Schichten fünf, sechs und Sieben.
+ Auf diese Schichten haben Anwendungen und Programme direkten Zugriff.

## Vorteile des OSI Modells
+ Kann gut als Standartmodell verwendet werden
+ Die Betriebssysteme spielen eine untergeordnete Rolle
+ Es unterstützt sowohl verbindungslose, als auch verbindungsorientierte Dienste
+ Es ist in der Lage sich an viele Protokolle anzupassen



## Quellen

Aufbau des OSI Modells: [Myrasecurity.com](https://www.myrasecurity.com/de/osi-modell/)

Schichten Funktion: [Ip-insider.de](https://www.ip-insider.de/was-ist-das-osi-modell-a-605831/)
