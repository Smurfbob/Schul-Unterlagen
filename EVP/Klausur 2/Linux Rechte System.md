# Linux Rechtesystem

## Was ist das Linux Rechtesystem
+ Das System ist in Nutzer und Gruppen unterteilt
+ Das System ist auf Windows nicht vorhanden
+ Das Rechtesystem ist auf allen Unix-Systemen gleich

## Nutzer

+ Der Nutzer ist für nur eine Person bestimmt
+ Jeder Nutzer hat einen Namen und erhält auch eine Identifikations-Nummer
+ Jeder Nutzer hat ein Home Verzeichnis, in welchen die persönlichen Daten gespeichert sind

## Gruppen

+ Nutzer können einer Gruppe zugehörig sein
+ Alle Nutzer, die einer Gruppe angehören, haben die selben Rechte, welche in dieser Gruppe definiert wurden
+ Normalerweise hat jeder Nutzer am Anfang bereits eine gleichnamige Gruppe
+ Auch die Gruppen besitzen eine Id und einen Namen

## Ordner und Dateien

+ Ordner und Dateien haben folgende Attribute
+ Jedes Element hat einen Besitzer
+ Jedes Element hat eine Gruppe

## Wichtige Befehle im Zusammenhang mit den Rechten

+ Die Wichtigsten Befehle für das Manipulieren von Rechten sind die folgenden

|Befehl|Funktion|
|-|-|
|chmod|Verändert die Zugriffsrechte auf ein Element|
|chown|Verändert den Besitzer, oder die Gruppe des Elements|
|chattr|Setzt, oder entfernt ein zusätzliches Attribut am Element|


## Übersicht über die Rechte

+ Die Rechte einer Datei werden bei der Auflistung dieser im Terminal sichtbar
+ Ein Beispielhafter Aufbau sieht zum Beispiel so aus
+ drwxr-x-w- 2 root jan 4096 Apr 15 09:11 dirname1
+ In dieser Auflistung sehen wir als erstes die Attribut der Datei "drwxr-x-w-"
+ Danach folgt der Nutzer, in diesem Fall "root"
+ Darauf folgt die Gruppe, in diesem Fall "jan"
+ Jetzt kommt noch die Größe der Datei in Bytes "4096"

## Attribut Zeichenkette

+ Die Attribut-Zeichenkette, in unserem Fall beispielhaft "drwxr-x---" gibt an, wer was mit der Datei machen darf und um welchen Typ es sich handelt
+ Der Aufbau erfolgt nach dem Schema 1+3+3+3, sprich es folgt erst ein Zeichen und danach folgen 3*3 Zeichen

### Erstes Zeichen

+ Das erste Zeichen gibt Aufschluss über den Typen der Datei
+ Es gelten folgende Zeichen
+ d: Ordner
+ b: Blockorientiertes Gerät
+ c: Zeichenorientiertes Gerät
+ f: Pipeline
+ s: Socketorientiertes Gerät
+ -: Normale Datei

### Dreier Block Zeichen

+ Die nächsten drei Blöcke sind alle nach dem selben Muster aufgebaut
+ Diese Blöcke definieren Rechte
+ Es gibt die folgenden Symbole
+ r: Leserechte
+ w: Schreibrechte
+ x: Ausführungsrechte
+ -: Rechte nicht gewährt
+ Die Position des Blocks gibt einen Bezug an
+ Der Erste Block bezieht sich auf den Besitzer
+ Der zweite Block bezieht sich auf die Gruppe
+ Der letzte Block bezieht sich auf die Rechte aller Nutzer

## Zugriffsrechte in Oktalzahlen

+ Anstelle der Symbole r,w,x, welche für das Verteilen der Rechte verwendet werden, kann man auch Oktalzahlen verwenden
+ 4: Leserecht
+ 2: Schreibrecht
+ 1: Ausführbar

## Übersicht

+ Rechte lassen sich durch die Addition der Zahlen miteinander kombinieren
+ Das Recht Ausführbar hat zum Beispiel den Wert 1 und das Recht lesbar hat den Wert 5
+ Sobald man diese Werte miteinander addiert, sprich den Wert 6 verwendet, hat man eine Datei, die sowohl lesbar, als auch ausführbar ist.
+ Die Tabelle stellt eine Übersicht, über die möglichen Kombinationen der Rechte dar

|Rechte|Zahl|Buchstaben|
|-|-|-|
|Keine Rechte|0|---|
|Ausführbar|1|--x|
|Schreibbar|2|-w-|
|Lesbar|4|r--|
|Ausführbar und Schreibbar|3|-wx|
|Ausführbar und Lesbar|5|r-x|
|Schreibbar und Lesbar|6|rw-|
|Lesbar, Schreibbar und Ausführbar|7|rwx|

## Quellen
+ [Jan Karres](https://jankarres.de/2015/04/debian-linux-zugriffsrechte-system-erklaert/)
