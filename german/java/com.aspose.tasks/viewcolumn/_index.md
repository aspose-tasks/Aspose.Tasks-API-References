---
title: "ViewColumn"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine Spalte in einer Projektansicht dar."
type: docs
weight: 344
url: /de/java/com.aspose.tasks/viewcolumn/
---

**Inheritance:**
java.lang.Object
```
public abstract class ViewColumn
```

Stellt eine Spalte in einer Projektansicht dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getField()](#getField--) | Ermittelt das Spaltenfeld. |
| [getName()](#getName--) | Ermittelt den Spaltennamen. |
| [getStringAlignment()](#getStringAlignment--) | Ermittelt die Ausrichtung des Textes (kann einer der Werte der [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)-Aufzählung sein). |
| [getTextStyleModificationCallback()](#getTextStyleModificationCallback--) | Ermittelt den Callback, der verwendet werden kann, um das Erscheinungsbild der Zellen der Spalte anzupassen. |
| [getWidth()](#getWidth--) | Ermittelt die Spaltenbreite. |
| [setField(int value)](#setField-int-) | Setzt das Spaltenfeld. |
| [setStringAlignment(int value)](#setStringAlignment-int-) | Legt die Ausrichtung des Textes fest (kann einer der Werte der [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)-Aufzählung sein). |
| [setTextStyleModificationCallback(ITextStyleModificationCallback value)](#setTextStyleModificationCallback-com.aspose.tasks.ITextStyleModificationCallback-) | Legt den Callback fest, der verwendet werden kann, um das Erscheinungsbild der Zellen der Spalte anzupassen. |
### getField() {#getField--}
```
public abstract int getField()
```


Ermittelt das Spaltenfeld. `Field`([getField()](../../com.aspose.tasks/viewcolumn\#getField--)/[setField(int)](../../com.aspose.tasks/viewcolumn\#setField-int-)).

**Returns:**
int – Spaltenfeld.
### getName() {#getName--}
```
public final String getName()
```


Ermittelt den Spaltennamen.

**Returns:**
java.lang.String – der Spaltenname.
### getStringAlignment() {#getStringAlignment--}
```
public final int getStringAlignment()
```


Ermittelt die Ausrichtung des Textes (kann einer der Werte der [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)-Aufzählung sein).

**Returns:**
int – Ausrichtung des Textes (kann einer der Werte der [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)-Aufzählung sein).
### getTextStyleModificationCallback() {#getTextStyleModificationCallback--}
```
public final ITextStyleModificationCallback getTextStyleModificationCallback()
```


Ermittelt den Callback, der verwendet werden kann, um das Erscheinungsbild der Zellen der Spalte anzupassen.

**Returns:**
[ITextStyleModificationCallback](../../com.aspose.tasks/itextstylemodificationcallback) - the callback which can be used to customize the appearance of the column's cells.
### getWidth() {#getWidth--}
```
public final int getWidth()
```


Ermittelt die Spaltenbreite.

**Returns:**
int – die Spaltenbreite.
### setField(int value) {#setField-int-}
```
public abstract void setField(int value)
```


Legt das Spaltenfeld fest. `Field`([getField()](../../com.aspose.tasks/viewcolumn\#getField--)/[setField(int)](../../com.aspose.tasks/viewcolumn\#setField-int-)).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | Spaltenfeld. |

### setStringAlignment(int value) {#setStringAlignment-int-}
```
public final void setStringAlignment(int value)
```


Legt die Ausrichtung des Textes fest (kann einer der Werte der [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)-Aufzählung sein).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | int | Ausrichtung des Textes (kann einer der Werte der [HorizontalStringAlignment](../../com.aspose/tasks/horizontalstringalignment)-Aufzählung sein). |

### setTextStyleModificationCallback(ITextStyleModificationCallback value) {#setTextStyleModificationCallback-com.aspose.tasks.ITextStyleModificationCallback-}
```
public final void setTextStyleModificationCallback(ITextStyleModificationCallback value)
```


Legt den Callback fest, der verwendet werden kann, um das Erscheinungsbild der Zellen der Spalte anzupassen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [ITextStyleModificationCallback](../../com.aspose.tasks/itextstylemodificationcallback) | Der Rückruf, der verwendet werden kann, um das Aussehen der Zellen der Spalte anzupassen. |

