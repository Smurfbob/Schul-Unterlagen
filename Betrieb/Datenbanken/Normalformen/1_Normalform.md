# Erste Normalform

## Ziel

+ Die erste Normalform zeichnet sich durch zwei Eigenschaften aus
+ Die Eigenschaften nennen sich Atomare und Wiederholungsfrei
+ Das Ziel ist es also die Daten so aufzubereiten, dass jedes Attribut nur eine Spalte bekommt und nicht mehrfache Informationen in einer Zelle stehen.

## Beispiel

### Atomare Attribute
+ Ein Attribut gilt dann als Atomar, sofern es sich nicht in kleinere Attribute aufspalten lässt
+ Nehmen wir als Beispiel die folgende Tabelle

|Name|Adresse|
|-|-|
|Peter Müller|August Straße, 6, PLZ: 3456, Ort: Berlin|

+ Das Attribut Name verstößt hierbei gegen die Atomare regel
+ Das Attribut Name kann nämlich noch in Vor und Nachname gespalten werden.
+ Berichtigt sieht die Tabelle daher so aus

|Vorname|Nachnahme|Adresse|
|-|-|-|
|Peter |Müller|August Straße, 6, PLZ: 3456, Ort: Berlin|

+ Die Tabelle ist allerdings immer noch nicht in der ersten Normalform, da die Adresse noch aus einer Auflistung besteht

### Auflistung

|Vorname|Nachnahme|Adresse|
|-|-|-|
|Peter |Müller|August Straße 6, PLZ: 3456, Ort: Berlin|

+ Wir behalten die Tabelle aus dem oberen Beispiel bei und sehen, das die Adresse aus den Attributen "Straße", "PLZ", "Haus-Nummer" und "Ort" aufgebaut ist
+ Die einzelnen Werte sind hierbei meist durch ein Komma getrennt und daher anders als bei dem Atomaren Attribut leicht zu erkennen
+ Die Attribute müssen daher noch in eine eigene Spalte unterteilt werden

|Vorname|Nachnahme|Straße|Nummer|PLZ|Ort|
|-|-|-|-|-|-|
|Peter |Müller|August|6|3456|Berlin|

+ Nach dieser Unterteilung befindet sich die Tabelle in der ersten Normalform
+ Die erste Normalform ist der Ausgangspunkt für die zweite Normalform und muss immer als erstes durchgeführt werden.

## Quellen
+ [Wikipedia](https://de.wikipedia.org/wiki/Normalisierung_(Datenbank))