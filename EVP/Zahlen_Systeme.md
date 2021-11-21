# Zahlen Systeme

## Dual Zahlen

+ Im dualen Zahlen-System wird einen Dezimalzahl nur mit einsen und und Nullen dargestellt.

+ Hierbei wird mit zwei als Basis gearbeitet, welche immer weiter potenziert wird. Sprich  2 hoch 0, 2 hoch 1, 2 hoch 3 etc.

+ Um eine Dezimalzahl in eine Dualzahl zu konvertieren, wird die Dezimalzahl, solange sie größer als 0 ist immer wieder durch zwei geteilt.
Gibt es einen Rest, wird eine eins hinzugefügt, gibt es keinen Rest, wird eine 0 hinzugefügt.
Am ende wird die Zahl noch invertiert.

## Hexadezimal Zahlen

+ Hexendezimalzahlen arbeiten mit der Basis 16 und greifen auf eine Erweiterung der Zahlen zurück sprich ab der 10 wird bis zur 15 mit den ersten Buchstabe des Alphabets weiter gerechnet.

+ Um eine Dezimalzahl in eine Hexadezimal-Zahl zu konvertieren, wird die Dezimalzahl solange durch 16 dividiert, bis dies 0 ergibt. Die reste von jedem teilergebnis wird mit 16 multipliziert und separat niedergeschrieben. 10 bis 15 hierbei natürlich als Buchstaben. Am ende werden die niedergeschrieben Zahlen noch invertiert.

### Negative Dualzahlen

+ Eine negative Dualzahl wird durch ein Zweierkomplement dargestellt. Hierbei werden alle positionen der Dualzahl invertiert (Aus 1 wird 0 und andersherum).

+ Diese Dualzahl wird als Einerkomplement bezeichnet, um jetzt noch ein Zweierkomplement zu bekommen, wird zu dieser Dualzahl eine 1 addiert.

## Allgemein für die Zahlensysteme

+ Um eine Zahl aus einem Zahlensystem in eine Dezimalzahl zu konvertieren, wird der Wert jeder Position mit einer potenz des jeweiligen Zahlensystems multipliziert und am Ende aufsummiert.

## Binäre Addition

+ Bei der binären Addition werden zwei Dualzahlen miteinander addiert.

+ Hierbei wird ähnlich der schriftlichen Addition von Dezimalzahlen jede Dualzahl untereinander geschrieben und jede Ziffer einzeln addiert und gegebenenfalls ein Übertrag auf die nächste Position weiter gegeben.

### Bei der Addition der einzelnen Ziffern gelten folgende Regeln.

|Fall|Ergebnis|Übertrag|
|-|-|-|
|0+0|0|0|
|1+0|1|0|
|0+1|1|0|
|1+1|0|1|
|1+1+1|1|1|

## BCD Zahlen

+ Bei einer BCD Zahl wird jede einzelne Ziffer einer Dezimalzahl als einzelne Dualzahl dargestellt.

+ Beispiel: 356 => 3-5-6 => 0111-0101-0110

### Rechnen mit BCD Zahlen

+ Beim Addieren von BCD Zahlen wie bei der Binären Addition jede Ziffer einzeln miteinander addiert. Auch hierbei gilt die Tabelle.

+ Besonders hierbei ist aber dass für den Fall, dass eine BCD Ziffer größer als 9 ist, diese mit dem wert 0110 => 6 addiert wird und der Übertrag auf die anderen BCD Zahlen erfolgt. Sofern am ende eine Übertrag bleibt, so muss dieser gegebenenfalls mit Nullen aufgefüllt werden.

+ Wichtig zu wissen ist hierbei auch, dass der Wert 0000 => 0 als größer als 9 gewertet wird und daher auch mit 0110 addiert werden muss.