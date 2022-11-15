# Ip Adressen und Subnetzmasken

## Netzwerkadressierung

+ Ein Protokoll der Netzwerkschicht muss gewährleisten, dass jeder Knoten mit jedem anderen Knoten kommunizieren kann.
+ Damit ein Knoten eindeutig identifizierbar ist, wird die Ip Adresse verwendet.
+ Eine Ip-Adresse kennzeichnet ein Interface, wobei jedes benutzte Interface seine eigenen Ip Adresse besitzt.
+ Eine IPV4 Adresse besteht auf vier Bytes
+ Die Bytes werden in Dezimalzahlen umgewandelt und durch Punkte voneinander getrennt.
+ So zum Beispiel **11.88.3.100**
+ Eine IPV4 Adresse besteht aus einem Netzteil und einem Host Anteil
+ Hosts die sich im gleichen Netz befinden haben den gleichen Netzanteil, jedoch einen andren Host Anteil in ihrer Ip Adresse.
+ Die Höchste und die kleinste Host Adresse können nicht an einen Host vergeben werden, da die kleinste Adresse als Netzadresse und die grösste als -Broadcastadresse verwendet wird.

## Angabe des Netzanteils

1. Man hängt die Binäre Position des Netzanteils mit einem Slash an die Ip Adresse zb. **11.88.3.100/16**. Die 16 verweist auf das 16 bit.
2. Es wird eine Netzwerkmaske verwendet, welche in einem byte nur Einsen, oder Nullen verwendet.
Die Position wo nur Nullen sind gehören zum Host und die Stellen wo nur Einsen sind gehören zur Netzmaske.

## Host Formel
+ Die Host formell gibt an, wie viele host bei einer bestimmte subnetzmaske erlaubt sind
+ Die Formel lautet ***2^h-2***
+ ***h*** steht hierbei für die Anzahl der Nullen in der Subnetzmaske

Quelle: [Vernetzte IT-Systeme: 27](https://intranet.rbbk-dortmund.de/~heimann/buecher/vernetzte_it_systeme_a4/seite027.gif)

```
/*
Gibt aus der Anzahl der Nullen in
der Subnetzmaske die Möglichen Hosts an
*/
function hostFormel(zeroBits) {
  return Math.pow(2,zeroBits)-2;
}

function subnetzFormel(oneBits) {
  return Math.pow(2, oneBits);
}

// IP-Adressraum 192.168.0.0
// Subnetzmaske 255.255.255.0
// Binäre Maske 111111111 11111111 11111111 00000000 / 24 zu 8
console.log( "Hosts: ", hostFormel(9));

// Link: https://www.computerweekly.com/de/tipp/IP-Adressen-und-Subnetze-Wie-man-IPv4-Subnetzmasken-mit-der-Host-Formel-berechnet

```
