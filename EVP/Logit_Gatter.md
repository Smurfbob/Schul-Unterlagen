# Logit Gatter

## Und gatter (And)

### Tabelle

|A|B|Y|
|-|-|-|
|0|0|0|
|0|1|0|
|1|0|0|
|1|1|1|

## Oder gatter (Or)

### Tabelle

|A|B|Y|
|-|-|-|
|0|0|0|
|0|1|1|
|1|0|1|
|1|1|1|

## Nicht gatter (Not)

### Tabelle

|A|Y|
|-|-|
|0|1|
|1|0|

## Nicht und Gatter (Nand)

### Tabelle

|A|B|Y|
|-|-|-|
|0|0|1|
|0|1|1|
|1|0|1|
|1|1|0|

## Nicht Oder gatter (Nor)

### Tabelle

|A|B|Y|
|-|-|-|
|0|0|1|
|0|1|0|
|1|0|0|
|1|1|0|

## Exclusives Oder (Xor)

### Tabelle

|A|B|Y|
|-|-|-|
|0|0|0|
|0|1|1|
|1|0|1|
|1|1|0|

### Formel

( !( A && B ) ) && (A || B)


## Exclusives nicht Oder (NXor)

### Tabelle

|A|B|Y|
|-|-|-|
|0|0|1|
|0|1|0|
|1|0|0|
|1|1|1|