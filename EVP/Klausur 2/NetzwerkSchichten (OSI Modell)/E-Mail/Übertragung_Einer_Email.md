# Übertragung einer E-Mail im OSI Modell

## Schritt sieben

+ Der siebte Schritt erfolgt auf der Anwendungsschicht
+ Hierbei gibt der Nutzer den Gewünschten Text in die E-Mail ein

## Schritt sechs

+ Der sechste Schritt findet auf der Darstellungsschicht statt
+ Hierbei wird die E-Mail in ein unabhängiges Daten-Format umgewandelt
+ Dies ist notwendig, damit die E-Mail auf jedem System lesbar ist
+ Zudem kommt es zu einer Verschlüsselung und Komprimierung der E-Mail

## Schritt fünf

+ Im fünften Schritt erstellt die Sitzungsschicht eine art Checkpoint
+ Dieser ist notwendig, damit bei einem Abbruch der Verbindung nicht alle 
Informationen erneut gesendet werden müssen

## Schritt vier

+ Im vierten Schritt geht es um die Transportschicht
+ Die Transportschicht ist dafür verantwortlich die Dateien in kleine Pakete zu unterteilen und diese zu versenden
+ Es gibt hierbei zwei Wichtige Protokolle einmal TCP und UDP
+ TCP stellt immer sicher, das alle Pakete die versendet werden auch garantiert ankommen
+ Sollte ein Paket fehlen, wird dieses nochmals gesendet
+ UDP stellt dies nicht sicher und es kann zu einem Paket Verlust kommen
+ Im unserem Beispiel mit der E-Mail wird daher TCP verwendet, da dieses sicher stellt, das die E-Mail auch vollständig ankommt
+ UDP wird hingegen meist für das Streamen, oder telefonieren verwendet, da dort ein verlorenes Paket nicht so schlimm ist

## Schritt drei

+ Im dritten Schritt befinden wir uns in der Netzwerkschicht
+ Hier wird der Empfänger der E-Mail ermittelt
+ Dies geschieht über eine IP-Adresse
+ Dadurch wird sichergestellt, das auch wirklich der Richtige die E-Mail bekommt und die Transportschicht, weiß dadurch, wohin sie die Pakete versenden muss

## Schritt zwei

+ Im zweiten Schritt kommt die Sicherungsschicht zum Tragen
+ Ihre Aufgabe ist es die Geschwindigkeit der Übertragung zu überwachen, damit nicht zu viele und nicht zu wenige Daten gesendet werden
+ Zudem werden Prüfsummen erstellt mit welchen die Pakete (Frames) auf ihre Richtigkeit geprüft werden können

## Schritt eins

+ Der erste Schritt findet in der Bitübertragungsschicht statt und wandelt die Pakete in ein passendes Signal um

![Empty](Bilder/E-Mail_%C3%9Cbertragen.png)