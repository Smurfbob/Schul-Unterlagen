# OSI Modell

## Funktion

+ Es gliedert komplexe Vorgänge in einzelne Schritte (eigentlich: Schichten). Jeder dieser Schichten wird eine bestimmte Aufgabe zugeschrieben und sie werden übereinandergestellt – so wird garantiert, dass die Kommunikation zwischen PCs und ähnlichen Endgeräten herstellerunabhängig und -übergreifend funktioniert.
+ Das Modell wird sehr häufig als Referenz herangezogen, wenn es darum geht, Abläufe einer Kommunikation oder Nachrichtenübermittlung exemplarisch darzustellen.
+ OSI steht für Open Systems Interconnection, also ein „offenes“ System für Kommunikationsverbindungen und Vernetzung.

## Aufbau des OSI Modells
+ Das OSI Modell gliedert sich in sieben Schichten.
+ Jede dieser Schichten hat eine explizite Aufgabe im Bezug auf das Senden und Empfangen von bestimmten Daten.
+ Jeder Nutzer, der an einer Kommunikation beteiligt ist, besitzt diese sieben Schichten auf seinem Gerät.
+ Die Schichten arbeiten eng miteinander zusammen und liefern Daten an die nächste, oder empfangen welche von der vorhärigen Schicht.

## Aufbau der Schichten

+ Es gibt sieben Schichten im OSI Modell, welche auch als Layer bezeichnet werden.
+ Merkspruch: "Please Do Not Throw Salami Pizza Away"

### 1 Physical Layer / Bitübertragungsschicht
+ Umwandlung der erhaltenen Bits in ein zum Medium passenden Signal, abschließend die physikalische Übertragung 

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
+ Segementierung der Pakete in sogenannte Frames und Hinzufügen von Prüfsummen

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
+ IP
+ IPX
+ ICMP
+ T.70
+ T.90
+ X.25
+ IPV6
+ NetBEUI
 
### 4 Transport-Layer / Transportschicht
+ Einer Anwendung werden Datenpakete zugeordnet

#### Protokolle
+ TCP
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
+ NetBIOS
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

#### Kommunikation in der Anwendungschicht
+ In der Anwendungschicht dient die Url als Identifikation für einen Computer
+ Diese Url wird dann zu einer IP-Adresse umgewandelt
+ Zur ermittlung einer IP-Adresse durch eine Url wird ein DNS verwendet

#### Protokolle
+ Telnet
+ FTP
+ HTTP
+ SMTP
+ NNTP

## Anwendungschichten
+ Unter die Anwendungschichten fallen die Schichten fünf, sechs und Sieben.
+ Auf diese Schichten haben Anwendungen und Programme direten Zugriff.
+ 

## Quellen

Aufbau des OSI Modells: [Myrasecurity.com](https://www.myrasecurity.com/de/osi-modell/)
