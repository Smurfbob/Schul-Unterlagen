# For Schleife

## Was ist eine for Schleife
+ Die for Schleife hat das Ziel einen Vorgang mehrfach aufzuführen
+ Die Anzahl der Durchläufe ist meist an eine feste Größe gebunden, im Gegensatz zur while Schleife
+ Die gebundene Größe kann zum Beispiel der Inhalt eines Verzeichnisses sein, oder eine vom
Nutzer gegebene Größe

## Aufbau einer for Schleife unter Linux
+ Der Aufbau einer Schleife in Batch lässt sich so darstellen
+ "for Bereich; do Anweisung; done"
+ Der begriff for markiert den Anfang der Anweisung
+ Der Bereich gibt die Größe an, an welche die for Schleife gebunden ist, unter Batch ist dies meist ein Verzeichnis
+ nach dem do folgt die Anweisung, welche in Abhängigkeit von der Größe des Bereichs x mal ausgeführt wird
+ Das done markiert das Ende der for Schleife

### Beispiele
+ Das folgende Beispiel gibt den String "Hallo Welt: $i" aus
+ $i ist hierbei eine Laufvariable, die am Anfang auf 0 gesetzt wird und bis auf neun ansteigt
``` Batch
for ((i=0;i<=10;i++)); do echo Hallo Welt: $i; done
```

## Aufbau einer for Schleife unter Windows
+ Die for Schleife in Windows ist etwas anders aufgebaut

``` Batch
@echo off
for %%i IN (Das ist ein Text) do (
    echo %i
)
```
+ Das Ergebnis dieser Schleife ist eine Ausgabe der Worte Das, ist, ein, Text
