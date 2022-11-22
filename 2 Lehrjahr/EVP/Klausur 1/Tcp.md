# TCP

+ TCP ist ein Transport Protokoll, bei welchem immer sicher gestellt wird, das am Ende alle Informationen übertragen wurden.
+ TCP ist in der Lage verschiedenen Netzwerke mit unterschiedlichen Größen miteinander zu verbinden.

## Voraussetzungen

+ Tcp benötigt in seinen Konfigurationen folgende Wert
1. Eine Ip-Adresse
2. Eine Subnetzmaske
3. Ein Standardgateway


## Flags
+ Um sicherzustellen das alle Daten am Ende auch richtig übertragen wurden, werden flags verwendet
+ Flags sind bestimmte Signale, mit welchen der Client und der Server sich gegenseitig Informationen über ihren Stand austauschen
+ Es gibt die folgenden Flags

1. **SYN**
2. **ACK**
3. **FIN**


## Ablauf einer TCP Verbindung

### Aufbau der Verbindung
1. Der Client sendet eine **SYN** Flag an den Server
2. Der Server muss diese Flag mit einer **ACK** bestätigen und ebenfalls eine **SYN** Flag versenden
3. Der Client muss wiederum mit einer **ACK** Flag antworten. Danach kann die Verbindung hergestellt werden

### Transport von Daten
1. Der Server wird jetzt sein erstes Datenpaket an den Client Senden
2. Der Client muss den Erhalt eines Paketes bestätigen
3. Dieser Vorgang wird so lange wiederholt, bis die Daten übertragen wurden

### Abbau der Verbindung
1. Eine der Beiden Seiten versendet ein **FIN** Flag
2. Die gegenseite muss dies mit einer **ACK** Flag beantworten und ebenfalls eine **FIN** Flag senden
3. Sobald die Verbindung abgebaut ist, wird dafür noch einmal eine letzte **ACK** Flag versendet

### Paket Verlust

+ Alle Daten-Pakete werden mit einer Sequenz-Nummer versehen
+ Anhand dieser Sequenz-Nummern kann der Client feststellen, ob ihm ein Datenpaket fehlt
+ Der Client teilt dem Server mit, welche Pakete er erhalten hat
+ Sofern die Bestätigung für ein Bestimmtes Paket zu lange ausbleibt, sendet der Server dieses Paket erneut los






