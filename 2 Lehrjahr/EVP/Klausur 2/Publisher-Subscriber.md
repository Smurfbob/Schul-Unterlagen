# Publisher Subscriber Prinzip

- Bei dem Publisher Subscriber Prinzip handelt es sich um ein Verfahren in welchem Informationen ausgetauscht werden
- Es wird mit einem Rollenprinzip gearbeitet, bei welchem einer der Beteiligten einen Publisher darstellt,
welcher eine beliebige Anzahl von Subscribern versorgen kann
- Zudem gibt es einen Broker, welcher als Vermittlungsinstanz dient
- Die Aufgabe des Brokers ist es hierbei die Nachrichten vom Publisher entgegen zu nehmen und an die Subscriber zu verteilen
- Meist wird mit sogenannten **Topics** gearbeitet. Ein subscriber abonniert ein bestimmtes Topic und kann danach Nachrichten
erhalten, welche mit diesem Topic versendet wurden.
- Dieses Verfahren erfolgt über das **MQTT** Protokoll

## Filterung

- Die Informationen können unterschiedlich gefiltert werden
- Einmal besteht die Möglichkeit dies über die Topics zu machen, welche vom Publisher festgelegt werden
- Die andere Möglichkeit ist dies über den Inhalt der Nachricht zu machen. Hierbei bestimmt der Subscriber, wie dieser Inhalt aufgebaut sein muss, damit dieser für den Subscriber in Frage kommt

## Quellen

- [It-Wissen](https://www.itwissen.info/Publish-Subscribe-Modell-publish-subscribe.html)
