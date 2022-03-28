# SQL Join

## Datensatz

+ Für die Folgenden Beispiele werden diese Tabellen verwendet

### Person
|Id|Name|age|
|-|-|-|
|1|Peter|33|
|2|John|24|
|3|Manuel|12|
|4|Bodo|55|

### Beruf

|Id|Name|Tätigkeit|
|-|-|-|
|1|Lehrer|Unterrichten|
|2|Optiker|Kunden Betreuung|
|3|Schüler|Lernt|
|4|Kaufmann|Verkauft Produkte|

## Join

+ Bei einem Join werden mehrere Tabellen zu einer neuen Tabelle zusammengefasst
+ Die Neue Tabelle wird nicht gespeichert und dient nur zur Ansicht für den Nutzer
+ Join lässt sich in verschiedene Typen gliedern


## Cross Join

+ Der Cross Join verbindet mehrere Tabellen miteinander zu einer Tabelle
+ Hierbei werden alle Kombinationen für die gegebenen Tabellen dargestellt

``` SQL
SELECT * person CROSS JOIN beruf
```

+ Alternativ funktioniert auch dieser Befehl

``` SQL
SELECT * FROM person,beruf WHERE person.id = beruf.id
```

### Ausgabe

|Id|Name|Age|Id|Name|Tätigkeit|
|-|-|-|-|-|-|
|1|Peter|33|1|Lehrer|Unterricht|
|1|Peter|33|2|Optiker|Kunden Betreuung|
|1|Peter|33|3|Schüler|Lernt|
|1|Peter|33|4|Kaufmann|Verkaufte Produkte|
|2|John|24|1|Lehrer|Unterricht|
|2|John|24|2|Optiker|Kunden Betreuung|
|2|John|24|3|Schüler|Lernt|
|2|John|24|4|Kaufmann|Verkaufte Produkte|
|3|Manuel|12|1|Lehrer|Unterricht|
|3|Manuel|12|2|Optiker|Kunden Betreuung|
|3|Manuel|12|3|Schüler|Lernt|
|3|Manuel|12|4|Kaufmann|Verkaufte Produkte|
|4|Bodo|55|1|Lehrer|Unterricht|
|4|Bodo|55|2|Optiker|Kunden Betreuung|
|4|Bodo|55|3|Schüler|Lernt|
|4|Bodo|55|4|Kaufmann|Verkaufte Produkte|


## Inner Join

+ Bei einem Inner Join werden nur die Spalten ausgegeben, bei welchen die Werte übereinstimmen
+ Dies wird durch eine Angabe von Parametern erreicht
+ In diesem Beispiel werden nur die Werte ausgegeben, bei welchen die id der Person mit der Id des Berufes übereinstimmen
+ Das "ON" markiert den Bereich für die Parameter Übergaben
+ Das "ON" kann als eine art Filter verstanden werden
+ Die Werte der Inner Join Ausgabe tauchen dementsprechend auch in der Cross Join Ausgabe auf

``` SQL
SELECT * FROM person JOIN beruf ON person.id = beruf.id;
```

### Ausgabe

|Id|Name|Age|Id|Name|Tätigkeit|
|-|-|-|-|-|-|
|1|Peter|33|1|Lehrer|Unterricht|
|2|John|24|2|Optiker|Kunden Betreuung|
|3|Manuel|12|3|Schüler|Lernt|
|4|Bodo|55|4|Kaufmann|Verkaufte Produkte|

## Natural Join

+ Beim Natural Join werden automatisch spalten verglichen, die den selben Namen tragen
+ Es werden daher auch keine Spalten doppelt angezeigt

``` SQL
SELECT * FROM person NATURAL JOIN beruf;
```