# IPv4

## Allgemein

+ Besteht aus vier Blöcken die auch als Oktett bezeichnet wird
+ Jeder Block ist ein Byte sprich acht Bit (Insgesamt 32 Bit)
+256 hoch vier Adressen sind möglich
+ Ein Byte kann einen Zahlenraum von 256 Zahlen Abdecken (0-255)

```
IPv4 Beispiel: 244.12.45.5
```


## Subnetzmaske (Host Netz Anteil) Ipv4

```
IPv4 Dezimal: 192.128,64.7 / 24

IPv4 Binär: 11000000.10000000.01000000.00000111
```

+ Die 24 am Ende der Dezimalen IPv4 stellt die Subnetzmaske dar
+ Sie sagt aus, das die ersten 24 Bits auf eins stehen

```
IPv4 Subnetz 24 Dezimal: 255.255.255.0
IPv4 Subnetz 24 Binär: 11111111.11111111.11111111.00000000
```

+ Um den Host und Netz Anteil zu erhalten werden die Bits der Subnetzmaske mit den Bits der IPv6 verglichen
+ Steht bei beiden eine eins, wird diese übernommen, sonst wird das Bit auf 0 gestellt

```
IPv4 Binär:                 11000000.10000000.01000000.00000111
IPv4 Subnetz 24 Binär:      11111111.11111111.11111111.00000000

IPv4 Netz Binär:      11000000.10000000.01000000.00000000
IPv4 Netz Dezimal:    192.128.64.0
```

+ Die Ersten drei Blöcke gehören zum Netz Anteil und der Letzte Block zum Host
+ Der Letzte Wert stellt immer die Broadcast Adresse dar
+ In diesem Falle ist es die 192.128.64.255, da 255 die Letzte zu vergebende position der Adresse ist.

## Quellen

[IPv4 Adresse einfach erklärt, ip und Subnetzmaske erklärt](https://www.youtube.com/watch?v=86ss1VVtcoA)