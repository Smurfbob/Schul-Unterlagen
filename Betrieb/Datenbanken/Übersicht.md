# Datenbank Übersicht

## Was ist eine Datenbank

+ Bei einer Datenbank handelt es sich um eine Ansammlung von Entit
+ Meist wird eine Relationale Datenbank aufgebaut.
+ Datenbanken sind im entferntesten Sinne mit Excel Tabellen vergleichbar.
+ Ziel der Datenbank ist es die Attribute in sinnvolle Beziehungen zueinander zu bringen.

## Attribute
+ Attribute werden oben in die Spalten geschrieben
+ Die Zellen unter dieser Spalte enthalten Primitive Datentypen, welche die Exakte Ausprägung diese Attributes symbolisieren
+ Beispiel: Name => Peter

## Primär und Fremdschlüssel
+ Um Zugriff auf eine Tabelle zu erhalten wird ein Schlüssel (Key) erwartet
+ Ein Schlüssel ist entweder ein Primärschlüssel, oder ein Fremdschlüssel
+ Ein Primärschlüssel macht die Tabelle und ihre Attribute eindeutig
+ Ein Fremdschlüssel verweist auf eine zweite Tabelle und gewährt Zugriff auf diese.
+ In der Tabelle, auf die der Fremdschlüssel verweist, ist dieser wiederum ein Primärschlüssel

## Erste Normalform

+ Die erste Normalform hat das Ziel Auflistungen aufzulösen und Informationen in kleine Teile zu aufzuteilen

## Zweite Normalform

+ Die erste Normalform dient als Grundlage für die zweite Normalform und muss als erstes erreicht werden
+ Alle Attribute, die nicht als Schlüssel verwendet werden, sollen in eine Abhängigkeit zu einem Schlüssel, oder einer Schlüsselgruppe gestellt werden
+ Es kann auch sein, dass ein Attribut in keiner Abhängigkeit zu einem Schlüssel steht

## Dritte Normalform

+ Bei der dritten Normalform werden transitive Abhängigkeiten aufgelöst
+ Eine Transitive Abhängigkeit ist vorhanden, sobald ein Attribut von einem Primären Schlüssel abhängig ist, jedoch auch noch von einem Zweiten
+ Sofern dann die Möglichkeit besteht diese Abhängigkeit zu trennen und das Attribut nur noch von einem Abhängig zu machen, ist die dritte Normalisierung erreicht

## Quellen
+ [Wikipedia](https://de.wikipedia.org/wiki/Normalisierung_(Datenbank))