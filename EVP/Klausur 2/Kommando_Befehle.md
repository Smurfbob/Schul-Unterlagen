# Auflistung der behandelten Linux und Windows Befehle

|Windows|Linux|Funktion|
|-|-|-|
help|man|Hilfe anzeigen|
|dir|Is|Verzeichnisinhalt anzeigen|
|dir /s| Is a-aIR|s.o. Mit allen Dateien in Unterordnern|
find|grep|Sucht nach einer Zeichenfolge|
|\\| |\\||Ausgabe in einen weiteren Befehl umleiten|
|>|>|Stdout in eine Datei schreiben (anhängen)|
|1>|1>|Stdout in eine Datei schreiben|
|2>|2>|Stderror in eine Datei schreiben|
|>>|>>|Stdout in eine Datei schreiben (anhängen)|
|set a = hello| a = hello|Die Variable mit dem Namen a auf hello setzen|
|echo %a%|echo $a|Den Inhalt einer Variable ausgeben|
|echo %1%|echo $1|Ausgabe des ersten Kommando-Zeilen-Argumentes|
|set|env|Anzeigen aller gesetzten Variablen|
|type|cat|Inhalt einer Textdatei anzeigen|
|more|more|Eine Textdatei seitenweise anzeigen|
|pause|read a|Ausführen einer Batch-Datei, bis eine Taste (bzw.Enter) gedrückt wird|
|copy|cp|Kopiert eine Datei|
|del|rm|Löschen von Dateien|
|rd|rm -R|Löschen von Verzeichnissen (und Dateien)|
|echo| echo| Eine Meldung auf dem Bildschirm ausgeben|
|exit| exit| Beendet den aktuellen Prozess (die Batch-Datei)|
|fc| diff| Vergleicht zwei Dateien und zeigt die Unterschiede.|
|ipconfig| ifconfig| Eigenschaften der Netzwerkadapter anzeigen (IP-Adresse)|
|mkdir|mkdir|Verzeichnis erstellen|
|move| mv| Verschieben einer Datei|
|rename| mv| Umbenennen einer Datei|
|net use| mount| Netzlaufwerke einbinden u.a.|
|nslookup| nslookup| DNS-Einstellungen überprüfen|
|ping|ping|Einen ICMP-Echo-Request schicken|
|telnet| telnet| Unverschlüsselte Konsole über das Netz aufbauen|
|route| route| IP-Routingtabelle anzeigen|
|shutdown| shutdown| Herunterfahren (Linux: shutdown -h now)|
|sort| sort| Sortiert eine Datei oder die Standardeingabe|
|tree| tree| Grafische Anzeige der Verzeichnisstruktur|
|sleep 1| sleep 1| Wartet eine Sekunde|
|call script2| ./script2| Aufruf eines weiteren Scriptes|
|edit| vi| Editor auf der Kommandozeile|
|start| /min &| Die Ausführung eines Prozesses in den Hintergrund schieben|