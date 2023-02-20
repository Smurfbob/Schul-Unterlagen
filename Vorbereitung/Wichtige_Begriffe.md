# Stichpunkte

## Verordnungen

- DIN VDE 100-410
- - Ist die wichtigste Norm für die Errichtung elektrischer Niederspannungsanlagen. Sie beschreibt die Schutzmaßnahmen gegen den elektrischen Schlag.

|Schutzmaßnahme|Beschreibung|
|-|-|
|Basisschutz|Dieser Schutz verhindert das direkte Berühren von spannungsführenden Leitungen oder Teilen des Systems. Das kann durch Isolierung oder Abdeckung oder auch Absperrungen erreicht werden|
|Fehlerschutz|Wenn es durch Fehler zu einer Spannung an Teilen (beispielsweise Gehäuseteilen) kommt, die normalerweise nicht unter Spannung stehen, so verhindert dieser Schutz durch Abschalten gefährliche Spannungen bei einer Berührung|
|Zusatzschutz|Dieser Schutz wird in der Regel mit Fehlerstrom-Schutzschaltern erreicht und dient als weitere Stufe des Schutzes|

## Virtualisierung


- **Was ist ein Snapshot**
- - Ist ein Abbild einer virtuellen Maschine
- - Hierbei werden die Daten eines Virtuellen Computers gesichert
- - Snapshots können während des Betriebs erstellt werden und der Nutzer kann immer wieder auf diese zurück gehen


### Server Virtualisierung
|Vorteile|Nachteile|
|-|-|
|Bessere Auslastung von Systemressourcen|Fällt der physische Server aus, sind alle virtuellen Maschinen betroffen|
|Weniger physischer Server notwendig|Geteilte Ressourcen wie Arbeitsspeicher können überlasten|
|Geringere Bereitstellungszeit für neue Server|-|
|Einfache Wartung|-|


### Anbieter von Virtualisierungen

|Anbieter|Beschreibung|
|-|-|
|Microsoft Hyper-V|Virtualisierungslösung, die meist bei Windows Server Systemen eingesetzt wird, aber auch unter Windows 10 verwendet werden kann|
|VMWare Hypervisor (ESXI)|Sehr weit verbreiteter Bare-Metal-Hypervisor. In einer Basisversion kostenfrei nutzbar, allerdings greifen hier viele Einschränkungen wie die Anzahl der unterstützen Prozessoren oder fehlende Features wie Live Migration|
|Oracle Virtualbox|Open Source Hosted Hypervisor, der au einer Vielzahl an Host-Betriebssystemen verfügbar ist|
|KVM|Kernel-based Virtual Machine ist eine Virtualisierungssoftware, die unter Linux verfügbar ist|
|Citrix Hypervisor|Wurde aus dem Open Source XenServer-Projekt entwickelt. In der kostenlosen Version ist nur ein eingeschränkter Funktionsumfang vorhanden. Die Lizenzierung erfolgt meist pro CPU-Sockel|


## Protokolle

- **publish-subscribe Protokoll**
- - Beim publish subscribe Protokoll gibt es einen Sender und eine unbeschränkte Anzahl an Empfängern
- - Sobald der Sender, meist ein Server, eine Nachricht ausgibt, wird dies allen offenen Empfängern zugestellt

- **Request-Response Protokoll**
- Beim Request Response Protokoll gibt es einen Client und einen Server
- Der Client stellt eine Anfrage an den Server und der Server soll diese beantworten
- Die Verbindung bleibt so lange offen, bis die Übertragung übermittelt ist, oder ein Zeitfenster ausgelaufen ist
