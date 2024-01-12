# Blockchain


## Definition
- Bei einer Blockhain handelt es sich um eine Art Datenbank, bei welcher die Speicherung dezentral erfolgt
- Eine wichtige Eigenschaft der Blockchain ist, das die einmal erstellten werte nicht mehr abgeändert werden können
- Die Blockchain speichert Informationen in Blöcken, welche Jeweils einen eigenen Hash aus ihrem Wert und einen Hash aus dem Block zuvor enthalten
- Durch die Verbindung dieser Blöcke entsteht eine Kette und alle Blöcke sind miteinander verbunden
- Sollte der Wert eines Blockes geändert werden, so würde der Hash nicht mehr mit dem des nächsten Blockes überein stimmen
- Dadurch können Änderungen in der Blockchain von den anderen Nutzern erkannte werden
- Da jeder Nutzer einer Blockhain eine Kopie aller Blocks besitzt, ist es kaum mehr möglich eine Änderung zu machen
- Jeder Neu erstellte Block wird von den anderen beteiligten geprüft, und erst nachdem mindestens die Hälfte diesen als Richtig markiert hat, wird dieser in die Blockchain mit aufgenommen

## Hashfunktion
- Eine Hashfunktion nimmt eine Zeichenkette von beliebiger Länge entgegen und verwandelt diese in eine Zeichenkette mit fester Länge.