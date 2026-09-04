---
title: "TableTextStyle"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt einen Textstil in einer Ansichtstabelle dar."
type: docs
weight: 288
url: /de/java/com.aspose.tasks/tabletextstyle/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.TextStyle](../../com.aspose.tasks/textstyle)
```
public class TableTextStyle extends TextStyle
```

Stellt einen Textstil in einer Ansichtstabelle dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [TableTextStyle(int rowUid)](#TableTextStyle-int-) | Initialisiert eine neue Instanz der Klasse [TableTextStyle](../../com.aspose.tasks/tabletextstyle). |
| [TableTextStyle(int rowUid, FontDescriptor font)](#TableTextStyle-int-com.aspose.tasks.FontDescriptor-) | Initialisiert eine neue Instanz der Klasse [TableTextStyle](../../com.aspose.tasks/tabletextstyle) mit der angegebenen Schriftart. |
| [TableTextStyle(int rowUid, float fontSize, int fontStyle)](#TableTextStyle-int-float-int-) | Initialisiert eine neue Instanz der Klasse [TableTextStyle](../../com.aspose.tasks/tabletextstyle) mit der angegebenen Schriftgröße und Schriftstil. |
| [TableTextStyle(int rowUid, int fontStyle)](#TableTextStyle-int-int-) | Initialisiert eine neue Instanz der Klasse [TableTextStyle](../../com.aspose.tasks/tabletextstyle) mit den Standard-Schrifteinstellungen und dem angegebenen Schriftstil. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getField()](#getField--) | Liest ein Feld, auf das der Stil angewendet wird. |
| [getItemType()](#getItemType--) | Gibt den Text-Elementtyp zurück. |
| [getRowUid()](#getRowUid--) | Liest die eindeutige ID einer Zeile. |
| [setField(int value)](#setField-int-) | Setzt ein Feld, auf das der Stil angewendet wird. |
### TableTextStyle(int rowUid) {#TableTextStyle-int-}
```
public TableTextStyle(int rowUid)
```


Initialisiert eine neue Instanz der Klasse [TableTextStyle](../../com.aspose.tasks/tabletextstyle).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowUid | int | Eine angegebene eindeutige Zeilen-ID. |

### TableTextStyle(int rowUid, FontDescriptor font) {#TableTextStyle-int-com.aspose.tasks.FontDescriptor-}
```
public TableTextStyle(int rowUid, FontDescriptor font)
```


Initialisiert eine neue Instanz der Klasse [TableTextStyle](../../com.aspose.tasks/tabletextstyle) mit der angegebenen Schriftart.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowUid | int | Eine angegebene eindeutige Zeilen-ID. |
| font | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | Eine Schriftart, auf der ein Textstil basiert. |

### TableTextStyle(int rowUid, float fontSize, int fontStyle) {#TableTextStyle-int-float-int-}
```
public TableTextStyle(int rowUid, float fontSize, int fontStyle)
```


Initialisiert eine neue Instanz der Klasse [TableTextStyle](../../com.aspose.tasks/tabletextstyle) mit der angegebenen Schriftgröße und Schriftstil.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowUid | int | Eine angegebene eindeutige Zeilen-ID. |
| fontSize | float | Größe einer Schriftart, auf der ein Textstil basiert. |
| fontStyle | int | Schriftstil. |

### TableTextStyle(int rowUid, int fontStyle) {#TableTextStyle-int-int-}
```
public TableTextStyle(int rowUid, int fontStyle)
```


Initialisiert eine neue Instanz der Klasse [TableTextStyle](../../com.aspose.tasks/tabletextstyle) mit den Standard-Schrifteinstellungen und dem angegebenen Schriftstil.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowUid | int | Eine angegebene eindeutige Zeilen-ID. |
| fontStyle | int | Schriftstil. |

### getField() {#getField--}
```
public final int getField()
```


Liest ein Feld, auf das der Stil angewendet wird. `Field`([getField()](../../com.aspose.tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Returns:**
int - ein Feld, auf das der Stil angewendet wird.
### getItemType() {#getItemType--}
```
public int getItemType()
```


Gibt den Text-Elementtyp zurück.

**Returns:**
int - enumerierter Typwert von TextItemType.
### getRowUid() {#getRowUid--}
```
public final int getRowUid()
```


Liest die eindeutige ID einer Zeile.

--------------------

Gibt -1 zurück, wenn der Stil auf alle Zeilen einer Ansicht angewendet werden soll.

**Returns:**
int - eine eindeutige Zeilen-ID.
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


Setzt ein Feld, auf das der Stil angewendet wird. `Field`([getField()](../../com.aspose.tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | ein Feld, auf das der Stil angewendet wird. |

