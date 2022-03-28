# SQL Übersicht

## Informationen

+ Kommandos werden sollten immer groß geschrieben werden

## Kommandos

|Kommandos|Funktion|
|-|-|
|CREATE TABLE "Name" ();|Erstellt eine Tabelle mit dem Namen "Name"|
|id INT|Gibt der Variable "id" den Datentypen INT|
|id PRIMARY KEY|Setzt die Variable id als Primär Schlüssel|
|SELECT * FROM table_name|Gibt die Werte in der Tabelle aus|
|SELECT column_name FROM table_name|Gibt eine Spalte aus einer Tabelle aus|
|SELECT column_name FROM table_name WHERE Vergleichswert > number|Gibt alle Zeilen aus, bei welchen die column_name Werte der zugehörigen aussage "Vergleichswert > number" entsprechen|
|INSERT INTO table_name (column1, column2, column3) VALUES (value1, value2, value3)|Fügt der Tabelle "table_name" die gegebenen Werte in die geforderte Spalte ein|
|DROP TABLE table_name|Löscht die Tabelle mit dem Namen table_name|
|SERIAL|Fügt dem Wert automatisch eine Id als Integer ein|
|SELECT * FROM table_name WHERE columnName = 'value';|Gibt die Reihe aus, in welcher der Wert aus der Spalte "columnName" dem Wert "value" gleicht|
|Klammern: ''|Werden verwendet um String werte zu markieren|
|Klammern: ""|Werden verwendet um Key Worte für Namen verwendbar zu machen|


## Datentypen

|Datentypen|Beschreibung|
|-|-|
|INT|Eine Zahl ohne Komma Werte|
|VARCHAR(N)|Speichert einen String der Größe N|
|DECIMAL(M,N)|Eine Zahl mit Komma Werten. N steht für die Größe der Zahl vor dem Komma und N steht für die Größe der Zahl nach dem Komma|
|BLOB|Steht für "Binary Large Object" und speichert ein größeres Objekt|
|DATE|Speichert ein Datum|
|TIMESTAMP|Stellt einen Zeitstempel dar, welcher einen Zeitpunkt dokumentiert|