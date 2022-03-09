# Container Visualisierung

## Was ist Container Visualisierung

+ Bei der Container Visualisierung handelt es sich um ein Konzept, bei welchem interne Funktionen eines Betriebsystems dafür genutzt werden anwendungen isoliert voneinander auf dem selben Host-System zu betreiben
+ Der Container ist hierbei vergleichbar mit einer Virtuellen Maschine
+ Anders als bei einer virtuellen Maschine muss jedoch hierbei kein vollständiges Betriebsystem installiert werden
+ Es wird stadtessen auf den Kernel des Hosts zugegriffen und dessen Betriebsystem genutzt

## Docker
+ Lange zeit war das Konzept der Visualisierung nicht nutzerfreundlich und gerade in der Anfangszeit für die Rechner zu resourcen aufwendig
+ Dies änderte sich im Jahre 2013 mit der Einführung von Dockern

## Vorteile

+ Die Container sind deutlich kleiner als eine virtuelle Maschine und können schneller gestarted und gestoppt werden
+ Die Container lassen sich auf den meisten Betriebsystemen einrichten

## Hypervisoren

+ Der Hypervisor, welcher auch als Virtual-Machine-Monitor bezeichnet wird ist eine Schicht, die die Kommunikation von zwei Betriebsystemen ermöglicht.
+ Eines der Betriebsysteme ist meist direkt auf der Hardware Installiert, das andere ist isoliert und als Virtueles Betriebsystem gespeichert
+ Dadurch ist es möglich mehrere Gastbetriebsysteme auf einem Rechner zu betreiben

### Typ 1
+ Der erste Typ wird auch als Bare-Metal-Hypervisor bezeichnet
+ Der erste Typ bietet eine bessere Performance und birgt eine höhere Flexibilität
+ Der Grund dafür liegt in einer dünnen Schicht zwischen der Hardware und der Virtuellen Maschine
+ Meist haben rechner mit Typ eins nur eine bestimmte Aufgabe

### Typ 2
+ Der zweite Typ erstellt Umgebungen für Virtuelle Maschinen und koordiniert Aufrufe auf die CPU, den Arbeitspeicher, die Festplatte, das Netzwerk und andere Resourcen.
+ Der erste Typ im gegensatz, hat direkten Zugriff auf diese Resourcen
+ Die Virtuelle Maschine kennt den Hypervisor meist nicht und kommuniziert nur indirekt mit diesem
+ 



## Nachteile

+ Risiken können dadurch entstehen, das Container ihren zuständigkeitsbereich verlassen und Änderungen am Kernel vornehmen
+ Zudem werden die Container nicht automatisch geupdated und müssen manuel und einzeln aktualisiert werden
+ Durch die Regulierung des Typs zwei ist es leichter mehrere Virtuellen Maschinen zu betreiben, da diese durch den Hypervisor verwaltet werden und keinen direkten Zugriff auf die Hardware haben


## Quellen

+ [Gridscale](https://gridscale.io/community/glossar/was-ist-containervirtualisierung/)
+ [Hypervisor: Wikipedia](https://de.wikipedia.org/wiki/Hypervisor)
+ [Hypervisor Typ 1](https://www.computerweekly.com/de/tipp/Vergleich-zwischen-Typ-1-und-Typ-2-Den-richtigen-Hypervisor-auswaehlen)
+ [Hypervisor Typ 2](https://www.computerweekly.com/de/definition/Typ-2-Hypervisor-Hosted-Hypervisor)
