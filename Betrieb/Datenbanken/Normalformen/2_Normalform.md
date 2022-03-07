# Zweite Normalform

##  Ziel
+ Das Ziel der Zweiten Normalform ist es die Abhängigkeit der Attribute in neue Tabellen aufzulösen.
+ Hierbei werden Beziehung zwischen den Einzelnen Attributen verglichen
+ Das Ziel ist es Redundanzen zu vermeiden
+ Eine Redundanz ist das nicht notwendige Auftreten eines Attributes in einer Tabelle

## Beispiel

+ Die folgende Tabelle zeigt ein Beispiel, welches sich bereits in der ersten Normalform befindet, sprich alle Attribute sind Atomar und es gibt keine Auflistungen in einer Zelle
+ Das Beispiel listet Cds auf und die Dazugehörigen Attribute

|CD_ID|Albumtitel|Interpret|Gründungsjahr|Erscheinungsjahr|Track|Titel|
|-|-|-|-|-|-|-|
|4711|Not That Kind|Anastacia|1999|2000|1|Not That Kind|
|4711|Not That Kind|Anastacia|1999|2000|2|I’m Outta Love|
|4711|Not That Kind|Anastacia|1999|2000|3|Cowboys & Kisses|
|4712|Wish You Were Here|Pink Floyd|1965|1975|1|Shine On You Crazy Diamond|
|4713|Freak of Nature|Anastacia|1999|2001|1|Paid my Dues

+ Diese Tabelle befindet sich nicht in der zweiten Normalform, da nicht alle Attribute von einem Primärschlüssel, oder einer Gruppe von Primärschlüsseln, oder von keinem Primärschlüssel abhängig sind.
+ In diesem Beispiel können wir sehen, das die Attribute "Albumtitel", "Interpret", "Gründungsjahr" und "Erscheinungsjahr" von der CD_ID Abhängig sind.
+ Sprich sobald sich die CD_ID verändert, verändern sich auch diese Attribute
+ Andersherum sind die Attribute immer gleich, sobald die gegebenen CD_ID vorkommt.
Wir haben daher die Möglichkeit diese Attribute in eine zweite Tabelle auszulagern und diese ausschließlich von diesem Schlüssel abhängig zu machen
+ Die zwei entstehenden Tabellen sehen folgendermaßen aus


### CD Tabelle

+ Diese Tabelle stellt die CD dar
+ Der Primäre Schlüssel ist hierbei die CD_Id, über welche der Zugriff auf alle anderen Attribute erfolgt.

|CD_ID|Albumtitel|Interpret|Gründungsjahr|Erscheinungsjahr|
|-|-|-|-|-|
|4711|Not That Kind|Anastacia|1999|2000|
|4711|Not That Kind|Anastacia|1999|2000|
|4711|Not That Kind|Anastacia|1999|2000|
|4712|Wish You Were Here|Pink Floyd|1965|1975|
|4713|Freak of Nature|Anastacia|1999|2001|

### Lied Tabelle

+ Hier ist die Lied Tabelle dargestellt
+ Sie enthält zwei Schlüssel Attribute
+ Das erste ist die CD_ID
+ Sie stellt hierbei zudem einen Fremdschlüssel dar, da wir mit diesem werd die CD Tabelle nach anderen Attributen fragen können
+ Die CD_ID ist hierbei eindeutig, da alle Attribute in der CD Tabellen nur von der CD_ID abhängig sind (Daher auch die Aufteilung in eine zweite Tabelle)
+ Der Titel ist hierbei von den beiden Schlüsseln CD_ID und Track Abhängig und erst durch diese beiden eindeutig zu identifizieren

|CD_ID|Track|Titel|
|-|-|-|
|4711|1|Not That Kind|
|4711|2|I’m Outta Love|
|4711|3|Cowboys & Kisses|
|4712|1|Shine On You Crazy Diamond|
|4713|1|Paid my Dues


## Ergebnis

+ Durch diesen Vorgang haben wir aus einer Tabelle zwei neue geschaffen, in welchen die Attribute eindeutig von ihren Primären Schlüssel abhängig sind und somit eindeutig zu identifizieren sind.
+ Die CD_ID zum Beispiel kann immer klar die Attribute "Albumtitel", "Interpret", "Gründungsjahr" und "Erscheinungsjahr" ermitteln
+ Würde nun eine Tabelle zum Beispiel das Attribut Albumtitel benötigen, so kann stattdessen immer die CD_ID angegeben werden, da mit dieser der Albumtitel in der Tabelle CD immer eindeutig bestimmt werden kann
+ Wir sparen uns also einige Spalten und nutzen bei bedarf die CD_ID als Schlüssel für die Tabelle CD


## Quellen
+ [Wikipedia](https://de.wikipedia.org/wiki/Normalisierung_(Datenbank))