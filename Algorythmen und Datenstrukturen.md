# Algorythmen und Datenstrukturen

## Array

- Bei einem Array wird ein bestimmter Speicherblock mit einer festenGröße reserviert

- Das Vergrößern eines Arrays ist teuer, da ein größeres Array angelegt und alle Daten kopiert werden müssen.

- Auf das Array wird mit einem Index zugegriffen

- Der Aufwand für das Iterieren ist von der Größe Abhängig

- Benötigt einen zusammenhängenden Bereich im Speicher

## Liste Einfach Verkettet

- Wenn ich ein Element aus einer einfach verketteten Liste lösche, muss die Referenz auf das nächste Element "umgebogen" werden. Bei einer zweifach verketteten Liste muss zusätzlich auch die Referenz auf das vorherige Element "umgebogen" werden.

- Wenn ich auf ein Element einer einfach verketteten Liste zugreifen möchte, muss ich immer beim ersten Element (first) anfangen und so lange zum nächsten Element (next) springen, bis ich bei meinem gewünschten Element angekommen bin.

- Der Aufwand für das Iterieren ist von der Größe Abhängig

- Der Aufwand für das Einfügen eines Elements am Endei einer einfach verketteten Liste unter der Annahme, dass diese folgenden Methoden zur Verfügung stehen first(), next() ist bei beliebigen Element immer gleich.

- Besteht aus Knoten die miteinander verbunden sind

## Queues

- Hat die Operationen Enqueue und Dequeue
- Eine Deque hat die Operationen
|Operation|Ergebnis|
|Push|Fügt das Element an das linke Ende der Liste|
|Put|Fügt das Element an das rechte Ende der Liste|
|Get|Nimmt vom rechten Ende der Liste|
|Pop|Nimt vom linken Ende der Liste|

- Sie kombiniert die Eigenschaften einer Queue und eines Stacks

### FIFO
- First in First Out
- Elemente werden oben/hinten angehängt und von unten/vorne wieder weggenommen

## Stack

- Hat die Operationen Push und Pop

### LIFO

- Last in First Out
- Elemente werden oben/hinten angehängt und von oben/hinten wieder weggenommen

## Schleifen / Iteratoren
- Beim Iterieren über eine Sammlung mit einer Foreach Schleife dürfen keine Elemente hinzugefügt oder entfernt werden.
- Bei einer ForEach-Schleife habe ich keine separate Zählvariable
- Mit ForEach-Schleifen kann über alle Elemente einer Collection iteriert werden.
- Laut Hpi sind ForEach Schleifen langsamer als for Schleifen
- Um sich zwischen den Elementen eines Iterators zu bewegen können die Methoden next() und previous() verwendet werden

## Compare To
- Wir können herausfinden ob zwei Elemente gleich sind
- Die Standardt Method von equals die aus Object kommt prüft nur ob es sich um das selbe Projekt handelt
- Es sollte nur Objekte miteinander verglichen werden, welche vom gleichen Datentypen sind
- Sofern ein equals() überschrieben wird, sollte auch das hashCode() überschrieben werden
- Die hashCode() methode sollte alle Attribute enthalten, welche für den Vergleich relevant sind
- Der umgekehrte compareTo() wert sollte immer negative bzw Positiv zum vorherigen Wert sein.
- Ob zwei Objecte nach der Methode equals() gleich sind hängt von der Implementation von equals() ab
- Weil das Object selbst ein equals() implementiert kann jedes Object miteinander verglichen werden
- Zwei gleiche Objecte müssen den gleichen Hascode haben
- Sollte nicht die Objectidentität für den Hashcode verwendet werden, muss die Methode überschrieben werden

## Suchen in Listen

### Lineare Suche
- Es mutss nur im schlimmsten Fall jedes Element der Liste betrachtet werden.
- 

### Binäre Suche

- Es muss eine sortierte Liste vorliegen
- Mit jedem such Schritt kann die anzahl der Betroffenen Elemente halbiert werden
- Es wird das prinzip divide and Conquer angewendet
- In einer sortierten liste lassen sich leichter bestimmte Werte finden

## Such Algorythmen

### Bubble Sort
- Wir vergleichen benachbarte Elemente und tauschen diese, wenn siein der falschen Reihenfolge sind. Das wiederholen wir so lange, bis die Liste sortiert ist.
- Bubblesort nutzt zwei ineinander verschachtelte Schleifen
- Nach dem ersten Durchlauf der äußeren Schliefe ist mindestens ein Element an der richtigen Position.
