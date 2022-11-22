# UDP

## Nutzen

+ UDP ist ein Protokoll, welches auf der vierten Schicht des OSI Modells (Transportschicht) Verwendung findet
+ Die Aufgabe von UDP ist es Daten zwischen zwei im Netzwerk verbundenen Knoten zu übertragen
+ Anders als TCP verwendet UDP keine Flags, mit welchen Server und Client sicher stellen, dass alle Daten-Pakete richtig übertragen wurden
+ Bei UDP wird ein fehlerhaftes, oder verloren gegangenes Paket nicht ersetzt
+ Daher eignet sich UDP vor allem für Übertragungen, welche nicht auf eine 100 prozentige Richtigkeit der Pakete angewiesen sind
+ UDP kann daher zum Beispiel für das Übertragen eines Live-Steams verwendet werden