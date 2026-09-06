---
title: "TableTextStyle"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en textstil i en vytabell."
type: docs
weight: 288
url: /sv/java/com.aspose.tasks/tabletextstyle/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.TextStyle](../../com.aspose.tasks/textstyle)
```
public class TableTextStyle extends TextStyle
```

Representerar en textstil i en vytabell.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [TableTextStyle(int rowUid)](#TableTextStyle-int-) | Initierar en ny instans av klassen [TableTextStyle](../../com.aspose.tasks/tabletextstyle). |
| [TableTextStyle(int rowUid, FontDescriptor font)](#TableTextStyle-int-com.aspose.tasks.FontDescriptor-) | Initierar en ny instans av klassen [TableTextStyle](../../com.aspose.tasks/tabletextstyle) med det angivna teckensnittet. |
| [TableTextStyle(int rowUid, float fontSize, int fontStyle)](#TableTextStyle-int-float-int-) | Initierar en ny instans av klassen [TableTextStyle](../../com.aspose.tasks/tabletextstyle) med den angivna teckenstorleken och teckenstilen. |
| [TableTextStyle(int rowUid, int fontStyle)](#TableTextStyle-int-int-) | Initierar en ny instans av klassen [TableTextStyle](../../com.aspose/tasks/tabletextstyle) med standardteckensnittinställningarna och den angivna teckensnittsstilen. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getField()](#getField--) | Hämtar ett fält som stilen ska tillämpas på. |
| [getItemType()](#getItemType--) | Returnerar textobjekttyp. |
| [getRowUid()](#getRowUid--) | Hämtar ett rad‑unikt ID. |
| [setField(int value)](#setField-int-) | Ställer in ett fält som stilen ska tillämpas på. |
### TableTextStyle(int rowUid) {#TableTextStyle-int-}
```
public TableTextStyle(int rowUid)
```


Initierar en ny instans av klassen [TableTextStyle](../../com.aspose.tasks/tabletextstyle).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowUid | int | Ett specificerat rad‑unikt ID. |

### TableTextStyle(int rowUid, FontDescriptor font) {#TableTextStyle-int-com.aspose.tasks.FontDescriptor-}
```
public TableTextStyle(int rowUid, FontDescriptor font)
```


Initierar en ny instans av klassen [TableTextStyle](../../com.aspose.tasks/tabletextstyle) med det angivna teckensnittet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowUid | int | Ett specificerat rad‑unikt ID. |
| font | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | Ett teckensnitt som en textstil är baserad på. |

### TableTextStyle(int rowUid, float fontSize, int fontStyle) {#TableTextStyle-int-float-int-}
```
public TableTextStyle(int rowUid, float fontSize, int fontStyle)
```


Initierar en ny instans av klassen [TableTextStyle](../../com.aspose.tasks/tabletextstyle) med den angivna teckenstorleken och teckenstilen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowUid | int | Ett specificerat rad‑unikt ID. |
| fontSize | float | Storlek på ett teckensnitt som en textstil är baserad på. |
| fontStyle | int | Teckensnittsstil. |

### TableTextStyle(int rowUid, int fontStyle) {#TableTextStyle-int-int-}
```
public TableTextStyle(int rowUid, int fontStyle)
```


Initierar en ny instans av klassen [TableTextStyle](../../com.aspose/tasks/tabletextstyle) med standardteckensnittinställningarna och den angivna teckensnittsstilen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowUid | int | Ett specificerat rad‑unikt ID. |
| fontStyle | int | Teckensnittsstil. |

### getField() {#getField--}
```
public final int getField()
```


Hämtar ett fält som stilen ska tillämpas på. `Field`([getField()](../../com.aspose.tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Returns:**
int - ett fält som stilen ska tillämpas på.
### getItemType() {#getItemType--}
```
public int getItemType()
```


Returnerar textobjekttyp.

**Returns:**
int - TextItemType enumererad typvärde.
### getRowUid() {#getRowUid--}
```
public final int getRowUid()
```


Hämtar ett rad‑unikt ID.

--------------------

Returnera -1 om stilen ska tillämpas på alla rader i en vy.

**Returns:**
int - ett rad‑unikt ID.
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


Ställer in ett fält som stilen ska tillämpas på. `Field`([getField()](../../com.aspose.tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett fält som stilen ska tillämpas på. |

