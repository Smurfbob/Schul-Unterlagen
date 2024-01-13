# Raid

- **Funktion**
- - Bei **RAID** wird versucht durch die Nutzung von mehreren Festplatten entweder die Speicherkapazität eines Rechners zu erhöhen, oder sicherzustellen, dass bei dem Verlust einer Festplatte nicht alle Daten verloren gehen, da sie auf einer anderen Platte zwischengespeichert werden.

- **Beispiele**

|Typ|Aufbau|Ziel|
|-|-|-|
|RAID 0|Bei RAID 0 werden mindestens zwei Festplatten zusammen geschaltet und die Daten werden auf alle Festplatten verteilt. Jedoch gehen bei RAID 0 alle Daten verloren, sobald eine der genutzten Festplatten ausfällt. Dies geschieht da die Daten auf alle Festplatten verteilt werden und nach dem Ausfall einer Festplatte nicht mehr zusammen geführt werden können|Das Ziel ist es, die Speicherkapazität zu erhöhen, da mehrere Festplatten zu einer zusammen geschaltet werden. Es kann auch zu einer schnelleren Speicherung kommen, da auf mehrere Festplatten gleichzeitig geschrieben wird.|
|RAID 1|Bei RAID 1 werden die gespeicherten Daten 1 zu 1 auf beide Festplatten gespiegelt. Es werden auch hierbei mindestens zwei Festplatten benötigt|Durch das Spiegeln der Daten ist es möglich, trotz des Ausfalls einer Festplatte keine Daten zu verlieren, da diese sich noch exakt auf einer anderen Festplatte befinden|
|RAID 5|Bei RAID 5 werden mindestens drei Festplatten benötigt. Wie bei RAID 0 werden auf alle Festplatten die Daten verteilt, jedoch werden auch Prüfsummen erstellt.|Durch das Erstellen von Prüfsummen ist es möglich, beim Ausfall einer Festplatte die verlorenen Daten erneut zu errechnen. Dieses System gilt als sehr sicher, ist aber relativ langsam|
|RAID 6|Raid 6 Benötigt mindestens vier Festplatten und Arbeitet wie RAID 5, jedoch werden zwei Arten von Prüfsummen erstellt|Dadurch können bei vier Festplatten zwei ausfallen und die Daten lassen sich durch die Prüfsummen weiterhin errechnen|
|RAID 10|RAID 10 Kombiniert RAID 0 und RAID 1 und benötigt mindestens vier Festplatten. Die Daten werden auf zwei Festplatten aufgeteilt und auf den anderen zwei Festplatten noch einmal gespiegelt|RAID 10 ist Schnell und kann beim Ausfall einer Festplatte noch alle Daten wieder herstellen, jedoch muss in viele Festplatten investiert werden|



## Berechnung der Kapazität

### Raid 5
- Bei einem Raid 5 wird die Kapazität durch die die Speichergröße der kleinsten Platte multipliziert mit der Anzahl der verwendeten Platten minus die Größe der kleinsten Platte Berechnet.
    - (kleinstePlatte * AnzahlPlatten) - kleinstePlatte