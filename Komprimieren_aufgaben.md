# Daten Komprimieren 

## 1. 

Dateisysteme haben auch eine Baumstruktur.

Ein binärer Baum hat bei jedem Knoten, immer höchstens 2 Kinder, dies ist bei nicht binären Bäumen nicht so, da gibt es meistens keine Begrenzung von Kindern.

#### 2.
B A N A N E

1 2 2 2 2 1


    6
   / \
  2   4
 /   / \
n   a   2
       / \
      b   e
![image](https://github.com/Rubenizz/114/assets/112400838/42683104-1ea9-445e-9490-4e1326420ecc)

## 3.
Mit 5 Bit kann man eine Linie von Pixeln im Bild darstellen. Es könnte 1 Bit oder kein Bit sein, da man einfach die Farbe angeben kann.

10100Gelb 1011Gelb, 10Schwarz, 111Gelb

10100Blau 1011Blau, 1Rot, 1Schwarz, 111Blau 100Blau, 10Rot, 1Schwarz, 10Blau, 101Rot, 1Schwarz,5Blau

1Blau

## 4. RLC:
RL-Code: 010100011110010010010010010010010010010110010110010010010010010010010010001 

```
010 100 011 110 010 010 010 010 010 010 010 010 010 110 010 110 010 010 010 010 010 010 010 010 001
 |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |
 2   4   3   6   2   2   2   2   2   2   2   2   2   6   2   6   2   2   2   2   2   2   2   2   1
 |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |
 W   S   W   S   W   S   W   S   W   S   W   S   W   S   W   S   W   S   W   S   W   S   W   S   W

WWSSSSWW
WSSSSSSW
WSSWWSSW
WSSWWSSW
WSSSSSSW
WSSSSSSW
WSSWWSSW
WSSWWSSW


  XXXX
 XXXXXX
 XX  XX
 XX  XX
 XXXXXX
 XXXXXX
 XX  XX
 XX  XX
```

Es wird ein 'A' dargestellt.

## 5.

### a. 

| Zeichenkette | Gefunden | Gespeichert | Eintrag | Nummer |
| ------------ | -------- | ----------- | ------- | ------ |
| banane       | b        | b           | ba      | 259    |
| anane        | a        | a           | an      | 256    |
| nane         | n        | 257         | na      | 257    |
| ane          | a        | 256         | ane     | 260    |
| ne           | n        | 257         | ne      | 261    |
| e            | e        | e           | -       | -      |

BANANE = b259260e

### b. 

| Zeichenkette  | Gefunden | Ausgabe | Eintrag | Nummer |
| ------------- | -------- | ------- | ------- | ------ |
| erdbe256kl260 | e        | e       | -       | -      |
| rdbe256kl260  | r        | r       | er      | 256    |
| dbe256kl260   | d        | d       | rd      | 257    |
| be256kl260    | b        | b       | db      | 258    |
| e256kl260     | e        | e       | be      | 259    |
| 256kl260      | e        | er      | ee      | 260    |
| kl260         | k        | k       | ek      | 261    |
| l260          | l        | l       | kl      | 262    |
| 260           | e        | ee      | le      | 263    |

erdbe256kl260 = erdbeerdklee


# 8.
## Andere Verfahren
 - Lempel-Ziv-Welch (LZW)
 - Deflate
 - Arithmetic Coding

### Daten, die verlustlos komprimiert werden sollten
- Textdateien
- Datenbanken
- Java Source Code

### Auswirkungen verlustbehafteter Komprimierung auf Texte und Quellcode
- Wörter verlust
- Daten verlust
- Unlesbarkeit
- Unausführbarkeit von Code
- Syntaxfehler

