# Aggregation

+ Bei einer Aggregation handelt es sich um Methoden, welche auf die Spalten angewendet werden
+ In diesem Beispiel wird die Aggregation "COUNT" verwendet, welche auf die Namen der Tabelle Person angewendet werden

``` SQL
SELECT COUNT(name) FROM person;
```


## Beispiel Aggregationen

|Aggregation|Wirkung|
|-|-|
|COUNT|Zählt die Anzahl der Werte in einer Spalte (Null wird nicht mit gezählt)|
|MAX|Gibt den Größten Wert in der Spalte aus|
|MIN|Gibt den kleinsten Wert in der Spalte aus|
|AVG|Gibt den Durchschnittswert in der Spalte aus|
|SUM|Gibt die Summe aller Werte in der Spalte aus|

## Having

+ Sofern man eine Aggregation einschränken möchte, so ist dies nicht über WHERE möglich, sondern muss über HAVING erfolgen

## Gruppierungen

+ Bei einer Gruppierung werden die Ergebnisse eines SELECT in Gruppen unterteilt, um sich eine bessere Übersicht zu verschaffen