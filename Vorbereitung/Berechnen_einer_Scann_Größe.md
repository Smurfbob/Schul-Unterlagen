# Berechnen einer Scann Größe

## Was wird für die Berechnung benötigt

- Es wird die Auflösung benötigt. Die Auflösung wird in der Einheit **dpi (dots per Inch)** angegeben
- Die Auflösung gibt an, wie viele Bildpunkte auf 2,54cm erfasst werden sollen
- Da die Auflösung aber in **Inch** angeben wird, muss bekannt sein, das ein **Inch** 2,54 **cm** entspricht
- Die Farbtiefe entspricht **16bit**
- - Es soll die Größe des Scans in **Mb** berechnet werden

## DPI PPI

- **DPI**
- - DPI bezieht sich auf die Zahl der gedruckten Punkte pro Zoll eines mit einem Drucker gedruckten Bildes
- **PPI**
- - PPI bezieht sich auf die Zahl der Pixel pro Zoll eines auf einem Computermonitor angezeigten Bildes.


## Beispiel

- **Angaben**
- Es wird eine DinA4 Seite eingescannt.
- Eine DIN A4 Seite ist besitzt die Maße 21 x 29,7 cm
- Es wird mit einer Auflösung von 600 ppi gescannt, sprich 600 dots pro inch
- Und es liegt eine Farbtiefe von 16 bit vor
- Es soll errechnet werden, wie groß die Datei am Ende ist

**Berechnung**

1. Die gegebenen Maße von 21 x 29,7 müssen in Inches umgewandelt werden
- - $Inch = {cm \over 2,54}$
- - $cm_v = {21 \over 2,54} = 8,27Inch$
- - $cm_h = {29,7 \over 2,54} = 11,7Inch$
- - - 
2. Als nächstes müssen die Pixel pro Bildseite errechnet werden. Dafür wird der **ppi** Wert mit den Werten der Inches Multipliziert. Um die gesamte Anzahl aller Bildpunkte zu erhalten müssen diese Werte noch multipliziert werden
- - $dots_v = 8,27 * 600 = 4.962$
- - $dots_h = 11,7 * 600 = 7.020$
- - $dots_g = dots_v*dots_h = 34.580.520$
- Die Gesamtzahl aller Bildpunkte entspricht also $34.580.520$
- - - 
3. Wir kennen die Anzahl der gesamten Bildpunkte jetzt wird jeder dieser Bildpunkte mit einer bestimmten Farbtiefe gescannt. In diesem Fall sind es **16bit**. Daher muss jetzt muss jetzt der Wert aller Punkte mal 16 gerechnet werden.
- - $bits_g = 16 * dots_g = 553.288.320$
- Die Anzahl aller bist beträgt also $553.288.320$
- - -
4. Abschließen muss das Ergebnis noch auf das gewünschte Größenformat umgerechnet werden. In diesem Fall werden Mb gewünscht.
- - Formel ${bit \over 10^6 * 8}$
- Abschließend kommt man auf 69,16 Mb als Ergebnis

