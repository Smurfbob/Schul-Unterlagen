# Algorythmen und Datenstrukturen

## Array
- Korrekte Aussagen über ein Array

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



