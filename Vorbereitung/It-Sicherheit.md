# Thematiken zur It Sicherheit


## Firewall und Intrusion Detection System

- **Firewall**
- - Dient dazu den unbefugten Zugriff in einem Netzwerk zu unterbinden
- - Die Firewall wird dementsprechend konfiguriert
- **Intrusion Detection System (IDS)**
- - Ist eine Soft, oder Hardware, welche das Ziel hat einen Angriff zu erkennen
- **Anmerkung**
- - Eine Firewall bzw ein IDS können das jeweils andere nicht ersetzten. Sprich eine Firewall kann nicht erkennen ob ein Angriff statt findet und ein IDS kann nicht den unbefugten Zugriff auf ein Netzwerk unterbinden

## Bewertung von Vertraulichkeit, Integrität und Verfügbarkeit von Hardware

|Kriterium|Router|Firewall|Arbeitsplatz-Pc mit Lan Verbindung|
|-|-|-|-|
|Vertraulichkeit|Die Übertragung von Kundendaten über das Internet hat einen sehr hohen Schutzbedarf, vor allem wenn auf Verschlüsselung verzichtet werden muss|Entsprechend der Wichtigkeit der Kundendaten ist auch die Vertraulichkeit der Firewall sehr Hoch|Da auf den Arbeitsrechnern mit den Kundendaten gearbeitet wird, ist die Vertraulichkeit sehr hoch|
|Integrität|Fehlerhafte Daten können relativ einfach erkannt werden|Fehlerhafte Daten können relativ einfach erkannt werden|Die Integrität ist stark davon abhängig, wie viele Mitarbeiter gleichzeitig mit den selben Daten arbeiten|
|Verfügbarkeit|Die Verfügbarkeit ist meist sehr wichtig, da je nach Unternehmensform viel mit den Kunden Kommuniziert werden muss|Die Verfügbarkeit ist sehr wichtig, sofern viele Daten vermittelt werden müssen|Die Verfügbarkeit der Arbeitsrechner ist sehr wichtig, da ein Ausfall dieser den Geschäftsprozess beeinträchtigen, oder sogar zum Stillstand bringen kann|

## Verschlüsselung von Daten

- **Symmetrische Verschlüsselung**
- - Bei der Symmetrischen Verschlüsselung verwenden sowohl der Sender, als auch der Empfänger die selben Schlüssel
- - Zum verschlüsseln und zum Entschlüsseln werden jeweils die gleichen Schlüssel verwendet
- - Das Verfahren ist so lange sicher, wie nur die beiden beteiligten die Schlüssel kennen

- **Asymmetrische Verschlüsselung**
- - Bei der Asymmetrischen Verschlüsselung besitzt jeder Beteiligten einen privaten und einen öffentlichen Schlüssel
- - Der private Schlüssel ist geheim und darf nur von der besitzenden Person gekannt werden
- - Der öffentliche Schlüssel wird an die Personen weiter gegeben, mit welchen die Daten ausgetauscht werden sollen
- - Das Verschlüsseln einer Datei erfolgt mit dem privaten Schlüssel. Mit den öffentlichen schlüsseln, kann festgelegt werden, wer die Datei entschlüsseln darf
- - Sofern eine Datei mit dem öffentlichen Schlüssel einer person verschlüsselt wurde, kann diese die Datei mit ihrem privaten Schlüssel wieder entschlüsseln


## Sicherung von Daten

- **Vollsicherung**
- - Bei einer Vollsicherung wird ein komplettes Abbild der Daten erstellt
- - Die Kann zum Beispiel eine Festplatte sein
- **Differenzielle Sicherung**
- - Bei der Differenziellen Sicherung liegt bereits eine Vollsicherung vor
- - Es wird ein Vergleich mit den Daten aus der Vollsicherung und den neuen Daten vorgenommen
- - Es werden anschließend nur die Daten in der Vollsicherung ersetzt, welche geändert wurden
- **Inkrementelle Sicherung**
- - Bei der Inkrementellen Sicherung wird bereits eine Vollsicherung und eine Differenzielle Sicherung benötigt
- - Es werden nur die Daten ersetzt, welche sich auf Basis der Vollsicherung, oder einer der Inkrementellen Sicherungen verändert haben