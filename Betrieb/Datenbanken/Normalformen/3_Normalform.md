# Dritte Normalform

## Ziel

+ Damit die dritte Normalform erreicht werden kann, muss zunächst die zweite Normalform vorliegen
+ Bei der dritten Normalform sollen transitive Abhängigkeiten beseitigt werden
+ Eine transitive Abhängigkeit liegt dann vor, wenn ein Attribut bereits von einem Primärschlüssel abhängig ist, es sich jedoch innerhalb der Tabelle noch von einem zweiten Schlüssel abhängig macht

## Beispiel

+ Als Einstiegspunkt dient hierbei wieder die Tabelle aus der Zweiten Normalisierung
+ Auch hierbei gilt wieder, das die zweite Normalisierung bereits abgeschlossen sein muss, bevor wir mit der dritten beginnen
+ Bei der Zweiten Normalisierung haben wir diese Tabelle für die CD aufgestellt

|CD_ID|Albumtitel|Interpret|Gründungsjahr|Erscheinungsjahr|
|-|-|-|-|-|
|4711|Not That Kind|Anastacia|1999|2000|
|4711|Not That Kind|Anastacia|1999|2000|
|4711|Not That Kind|Anastacia|1999|2000|
|4712|Wish You Were Here|Pink Floyd|1965|1975|
|4713|Freak of Nature|Anastacia|1999|2001|

+ Wir haben bei dieser Tabelle den Primärschlüssel CD_ID, welcher in der Tabelle Lied als Fremdschlüssel auftritt
+ Sprich alle Attribute sind erst einmal von diesem Schlüssel abhängig und eindeutig identifizierbar
+ Jedoch gibt es hierbei noch eine zweite Abhängigkeit
+ Das Gründungsjahr der Band ist einzig und allein vom Interpreten abhängig, da die Gründung einer Band nur einmal stattfindet und danach nicht mehr
+ In unserer derzeitigen Darstellung ist das Erscheinungsjahr allerdings sowohl von der CD_ID transitiv, als auch vom Interpreten abhängig
+ Das Ziel der dritten Normalisierung ist es eben diese Abhängigkeit aufzulösen

+ Die Auflösung geschieht daher ähnlich wie bei der zweiten Normalisierung durch das erstellen einer neuen Tabelle
+ In dieser Tabelle stellen wir die Abhängigkeit zwischen dem Interpreten und dem Gründungsjahr dar

|Interpret|Gründungsjahr|
|-|-|
|Anastacia|1999|
|Pink Floyd|1965|

+ In dieser Tabelle dient uns der Interpret als Primärschlüssel und lässt uns das Gründungsjahr eindeutig identifizieren
+ Die CD Tabelle benötigt daher nur noch den Interpreten und kann diesen als Fremdschlüssel für die Neue Tabelle Künstler verwenden

|CD_ID|Albumtitel|Interpret|Gründungsjahr|Erscheinungsjahr|
|-|-|-|-|-|
|4711|Not That Kind|Anastacia|1999|2000|
|4711|Not That Kind|Anastacia|1999|2000|
|4711|Not That Kind|Anastacia|1999|2000|
|4712|Wish You Were Here|Pink Floyd|1965|1975|
|4713|Freak of Nature|Anastacia|1999|2001|

+ So sieht die neue CD Tabelle aus
+ Mit der Schaffung der Künstler Tabelle, haben wir die transitive Abhängigkeit des Erscheinungsjahrs von der CD_ID gelöst und auf die Abhängigkeit des Künstlers reduziert
+ Die dritte Normalform ist somit erreicht



## Quellen
+ [Wikipedia](https://de.wikipedia.org/wiki/Normalisierung_(Datenbank))