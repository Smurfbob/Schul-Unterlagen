# Wichtige Begriffe zum Merken

|Begriff|Erklärung|
|-|-|
|Cluster Server|-|
|Backups|Eine Kopie von Daten, welche regelmäßig aktualisiert wird und zur Verwendung kommt, falls die Daten, welche derzeit in Benutzung sind verloren gehen|
|USV (Notstromversorgung)  |Wird verwendet um im Falle von einem Stromausfall alle Geräte sicher herunter zu fahren|
|Offline USV (VFD - Voltage and Frequency Dependent)|Sind einfach und kostengünstig. Kann für einfache Geräte verwendet werden. Leitet den Strom im Normalbetrieb einfach weiter und schaltet bei einem Ausfall auf die Batterie um. Es dauert um die 10ms bis die Umschaltung erfolgt ist|
|Netzinterkive USV (VI - Voltage Independent)|Ist schneller als die Offline USV und schaltet mit 4ms auf die Batterie um. Besitzt einen Bidirektionalen Wechselrichter. Dieser begrenzt auch im Normalbetrieb die Höhe der Spannung. Dadurch können Spannungschwankungen abgefangen werde. Ist im mittleren Preisegment|
|Online USV (VI - Voltage and Frequency Independent)|Die Online USV hat keine Umschaltzeit. Sie gleicht konstant die Versorgung aus und ist für Kritische Systeme sinvoll. Sie ist im vergleich zu den anderen USV Variante sehr teuer|
|Raid 0|Bei einem Raid 0 werden die Daten gleichmäßig auf zwei Platten verteilt. Dies dient der Ausweitung des Speichers|
|Raid 1|Es werden zwei Platten verwendet und die Daten werden gespiegelt, sofern eine der Platten ausfällt, dient die andere als Backup|
|Raid 5|Bei Raid 5 werden mindestens drei Platten verwendet. Die Daten werden auf drei Platten verteilt und mit Prüfsummen gesichert. Sofern eine der drei Platten ausfällt, so lässt sich der Inhalt durch die verbleibenden zwei platten wieder herstellen|
|Raid 6|Arbeitet wie Raid 5 jedoch werden vier Platten verwendet und es können zwei Platten ausfallen und die anderen können die Daten wieder herstellen|
|Paritätsinformationen|Damit werden die Prüfsummen auf einem Raid gemeint, aus welchen sich die Daten bei einem Ausfall wieder herstellen lassen|
|Neronales Netz|Neuronale Netze arbeiten nach dem Vorbild des menschlichen Gehirns und durch Nachahmung erlernt. Hierbei werden künstliche Neuronen miteinander vernetzt und mit bestimmten Daten trainiert|
|Hardware Schnittstelle|Schnittstelle zwischen physischen Systemen in der Computertechnik|
|Netwerkschnittstelle|Schnittstelle zwischen Komponenten der Netzwerktechnik|
|Softwareschnittstelle|Schnittstellen zwischen Anwendungen, zum Betriebssystem oder in der Programmierung zur Vereinbarung von Funktionen oder Methoden|
|Benutzerschnittstelle|Schnittstell zwischen Mennsch und Gerät meist der Computer|
|Software Ergonomie|Bedeutet so vie wie optimale wechselseitige Anpassung zwischen dem Menschen und seinen Arbeitsbedingungen. Die Software soll also auf den Menschen zugeschnitten sein|
|Arbeitsstättenverordnung|Tisch und Stuhl muss verstellbar sein. Bildschirm soll einstälbar sein und darf nicht Flackern. Schrift soll auch verstellbar sein. Die Tastatur muss eine vom Bildschirm getrennte Einheit sein. Genug Licht am Arbeitsplatz. Blickrichtung soll parallel zum Fenster sein. Nach 50 Minuten sollte ein Pause von 5 bis 10 Minuten Stattfinden|
|San (Storage Area Network)|Ein SAN ist ein Netzwerk von Speichergeräten, au fdie von mehreren Teilnehmern zugegriffen werden kann und die gemeinsam genutzten Speicherplatz bereitstellen. Das SAN wird so dargestellt, als währe es ein lokales speicher Medium. Anzahl der Platten kann erhöht werden.|
|Ethernet|-|
|NAS (Network Attached Storage)|Ein NAS ist ein Speicher, welcher in einen Netzwerk ein IP bekommt und über Ethernet und IP Kommunizieren. Es stellt seinen Zugang also über ein Netz bereit. Die Anzahl der Platten kann meist nicht erhöht werden|
|Rack Server|Ein Rack Server wird in ein meist 19 Zoll breites Rack eingebaut. Rack Server können übereinander eingebaut werden|
|Blade-Server|Ein Blade Server ist ein ComputerSystem, welches allgemeine Funktionen wie Lüftung und Stromversorgung aus einem Chassis bekommt. In das Chassis können mehre Blades(Computer) eingebunden werden|
|Chassis|Eine Art Hülle die Funktionen wie Lüftung und Stromversorgung bereit stellt. In dieses können Computer (Blades) eingebaut werden|
|Service Level Agreement|Reguliert widerkehrende Dienstleistungen bei einem Produkt. Es wird zum Beispiel Leistungsumfang, Reaktionszeit und Schnelligkeit der Verarbeitung geregelt|
|Level 1 Support|Ist die Erste Stelle, an welche sich der Kunde für eine Problemlösung wendet|
|Level 2 Support|Ist die Zweite Stelle an die sich der Kunde wendet. Diese wird als erste Eskalationstufe bezeichnet und Personen mit Fachwissen sind vor Ort|
|Level 3 Support|Ist die zweite Eskalationsstufe und es handelt sich um Spezialisten vor Ort|
|API|Ist eine Software Schnittstelle und stellt Interaktionen mit einer Software Komponente bereit|
|REST|Steht für Representational State Transfer und wird bei der Kommunikation zwischen verteilten Systemen eingesetzt. Es ist zustandslos, was bedeuted, das jede Anfrage für sich Vollständig ist und alle nötigen Informationen enthält|
|SOAP|Steht für Simple OBject Access Protocol und verwendet Xml für die Übertragung von Daten. Kann SMPT oder HTTP als Protocol verwenden. Es definiert strenge Regeln für den Datenaustausch|
|CORBA|Steht für Common Object Request Broker Architecture und arbeitet Objekt orientiert|
| Scrum | Agiles Framework für die Entwicklung von Software und anderen Produkten, das auf kurzen, iterativen Entwicklungszyklen basiert. |
| Kanban | Agiles Framework für die Verwaltung von Arbeitsprozessen, das sich auf die Visualisierung von Arbeit und die kontinuierliche Verbesserung konzentriert. |
| Produktionsprozess | Abfolge von Schritten, die zur Herstellung eines Produkts oder einer Dienstleistung erforderlich sind. |
| Arbeitsabläufe | Abfolge von Aktivitäten, die zur Erfüllung einer Aufgabe oder eines Ziels erforderlich sind. |
| Agile | Ansatz für die Entwicklung von Software und anderen Produkten, der sich auf die Flexibilität und Anpassungsfähigkeit an sich ändernde Anforderungen konzentriert. |
| Softwareentwicklungsmodell | Rahmenwerk für die Entwicklung von Software, das die Struktur, die Abläufe und die Artefakte der Entwicklung definiert. |
| Projektplanung | Prozess der Definition der Ziele, des Umfangs, des Zeitplans, des Budgets und der Ressourcen eines Projekts. |
| Zeitplanung | Prozess der Festlegung der Termine für die einzelnen Aufgaben eines Projekts. |
| Projektphasen | Abfolge von aufeinanderfolgenden Abschnitten, in die ein Projekt unterteilt ist. |
| Netzplan | Diagramm, das die Beziehungen zwischen den einzelnen Aufgaben eines Projekts darstellt. |
| Gantt-Diagramm | Diagramm, das die geplanten Termine für die einzelnen Aufgaben eines Projekts darstellt. |
| Projektmanagement | Fachgebiet, das sich mit der Planung, Steuerung und Kontrolle von Projekten befasst. |
| Magisches Dreieck | Modell, das die drei grundlegenden Zielkonflikte des Projektmanagements darstellt: **Zeit**, **Kosten** und **Qualität**. |
| DIN EN ISO 9921 | Norm für die Begriffe und Definitionen im Projektmanagement. |
| DIN 69901 | Norm für die Projektmanagement-Prozesse. |
| PMBOK | A Guide to the Project Management Body of Knowledge, ein Standardwerk für das Projektmanagement. |
| SOAP | Simple Object Access Protocol, ein Protokoll zur Kommunikation zwischen Anwendungen. |
| IPMA | International Project Management Association, eine internationale Vereinigung von Projektmanagern. |
| REST | Representational State Transfer, ein Architekturstil für verteilte Systeme. |
| PRINCE2 | PRojects IN Controlled Environments, ein Framework für das Projektmanagement. |
| ISAPI | Internet Server Application Programming Interface, eine API für die Entwicklung von Web-Anwendungen. |
| Vorbereitung | Phase des Projektmanagements, in der die Grundlagen für das Projekt gelegt werden. |
| Durchführung | Phase des Projektmanagements, in der die geplanten Aktivitäten durchgeführt werden. |
| Abschluss | Phase des Projektmanagements, in der das Projekt abgeschlossen und die Ergebnisse evaluiert werden. |
| Rollen und Verantwortlichkeiten | Zuordnung von Aufgaben und Verantwortungen an die einzelnen Beteiligten eines Projekts. |
| Kommunikation | Austausch von Informationen zwischen den Beteiligten eines Projekts. |
| Risikomanagement | Prozess zur Identifizierung, Bewertung und Behandlung von Risiken, die das Projekt beeinflussen können. |
| Change Management | Prozess zur Steuerung von Änderungen am Projektumfang, am Zeitplan oder am Budget. |
| Qualitätsmanagement | Prozess zur Sicherstellung der Einhaltung der Qualitätsstandards für das Projekt. |
| Kostenmanagement | Prozess zur Planung, Steuerung und Kontrolle der Kosten eines Projekts. |
| Ressourcenmanagement | Prozess zur Planung, Steuerung und Kontrolle der Ressourcen eines Projekts. |
| Terminmanagement | Prozess zur Planung, Steuerung und Kontrolle der Termine eines Projekts. |
| Auftraggeber | Person oder Organisation, die das Projekt in Auftrag gibt. |
| Projektmanager | Person, die für die Leitung und Steuerung eines Projekts verantwortlich ist. |
| Teammitglieder | Personen, die an der Durchführung des Projekts beteiligt sind. |
