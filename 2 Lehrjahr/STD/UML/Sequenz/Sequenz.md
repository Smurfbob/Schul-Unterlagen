# Sequenz Diagramm

- Bei einem Sequenzdiagramm werden Interaktionen zwischen einer Gruppe von Objekten abgebildet und es gibt eine Reihenfolge an
- Wird teils auch als Ereignisdiagramm bezeichnet
- Wird zum Beispiel verwendet, um zu verstehen, welche Anforderungen eine neues System stellt

## Symbole

|Name|Beschreibung|Symbol|
|----|------------|------|
|Objekt Symbol|Stellt eine Klasse bzw. ein Objekt dar. Es sollte jedoch keine Attribute enthalten|![Empty](./image/Objekt.PNG)|
|Aktivitätsbalken|Die Länge des Balkens soll die Dauer zum abschließen einer Aufgabe darstellen|![Empty](./image/Aktivit%C3%A4ts-Balken.PNG)|
|Akteur-Symbol|Stellt eine Person dar, welche mit dem System interagiert|![Empty](./image/Nutzer.PNG)|
|Paket|Soll interaktive Elemente darstellen|![Empty](./image/Paket.PNG)|
|Lebenslinie|Stellt einen Zeitverlauf dar und zeigt auf, was in diesem Verlauf mit dem Objekt passiert|![Empty](./image/Lebenslinie.PNG)|
|Optionsschleife|Stellt dinge dar, welche unter einer bestimmte voraussetzung eintreten|![Empty](./image/Optionsschleife.PNG)|
|Alternativen|Stellt eine Auswahl von Elementen dar, welche sich in der Regel gegenseitig ausschließen|![Empty](./image/Alternative.PNG)|

## Nachrichten

|Name|Beschreibung|Symbol|
|----|------------|------|
|Synchrone Nachricht|Der Absender muss auf die Antwort der Nachricht warten|![Empty](./image/Synchron.PNG)|
|Asynchrone Nachricht|Der Absender muss nicht auf die Antwort warten|![Empty](./image/Asynchron.PNG)|
|Asynchrone Antwort Nachricht|Gibt eine Antwort auf eine Asynchrone Anfrage|![Empty](./image/Asynchrone-Antwort.PNG)|
|Asynchrone Nachrichten Erstellung|Eine Solche Nachricht erstellt eine neues Objekt|![Empty](./image/Asynchrone-Nachrichten-Erstellung.PNG)|
|Antwort Nachricht|Stellen Antworten auf Anrufe dar|![Empty](./image/Antwort.PNG)|
|Löschnachricht|Eine Solche Nachricht zerstört ein Objekt|![Empty](./image/L%C3%B6sch-Nachricht.PNG)|

## Beispiel

- In diesem Beispiel geht es um den Besuch in einem Krankenhaus
- Wir haben die Akteure **Patient**, **Doctor**, **Operation**, **Test** und **Patient Database**
- Zu beginn können wir sehen, das der **Doctor** die Aktionen **Perform Checkup** und **Prescribe Meds** am Patienten ausführt ausführt
- Dies wird durch ``Synchrone Nachrichten`` dargestellt
- Der Patient gibt ein **Feedback** an den **Doctor** und verwendet dafür ``Antwort Nachrichten``
- Danach führt der Arzt die Aktion **Prescribe Test** aus und erhält **keine** Antwort vom Patienten
---
- Der Patient versendet nun eine Nachricht an den Akteur **Test** und erhält später die Antwort **Return Report**
- Danach gibt der **Patient** die Nachricht **Review Report** an den Arzt, welcher darauf die Nachricht **Update Patient info** an den Akteur **Patient Database** versendet
---
- Nach einer Pause versendet der **Doctor** die Nachricht **Prescribe Meds** und etwas später noch die Nachricht **Prescribe Operation** an den **Patient**
- Dieser sendet darauf die Nachricht **Undergo Operation** an den Akteur **Operation**
- Während der Operation verschreibt der **Doctor** mehr Tests und führt danach die Operation durch
- Zum Abschluss wird ein Update auf die Patienten Datenbank durchgeführt.
---

![Empty](./image/Example.PNG)


## Quellen

[Lucidchart](https://www.lucidchart.com/pages/de/uml-sequenzdiagramme)