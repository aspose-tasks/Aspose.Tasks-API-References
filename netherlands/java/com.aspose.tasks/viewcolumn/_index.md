---
title: "ViewColumn"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een kolom in een projectweergave voor."
type: docs
weight: 344
url: /nl/java/com.aspose.tasks/viewcolumn/
---

**Inheritance:**
java.lang.Object
```
public abstract class ViewColumn
```

Stelt een kolom in een projectweergave voor.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getField()](#getField--) | Haalt het kolomveld op. |
| [getName()](#getName--) | Haalt de kolomnaam op. |
| [getStringAlignment()](#getStringAlignment--) | Haalt de uitlijning van de tekst op (kan een van de waarden van de enumeratie [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) zijn). |
| [getTextStyleModificationCallback()](#getTextStyleModificationCallback--) | Haalt de callback op die kan worden gebruikt om het uiterlijk van de cellen van de kolom aan te passen. |
| [getWidth()](#getWidth--) | Haalt de kolombreedte op. |
| [setField(int value)](#setField-int-) | Stelt kolomveld in. |
| [setStringAlignment(int value)](#setStringAlignment-int-) | Stelt de uitlijning van de tekst in (kan een van de waarden van de [HorizontalStringAlignment](../../com.aspose/tasks/horizontalstringalignment) enumeratie zijn). |
| [setTextStyleModificationCallback(ITextStyleModificationCallback value)](#setTextStyleModificationCallback-com.aspose.tasks.ITextStyleModificationCallback-) | Stelt de callback in die kan worden gebruikt om het uiterlijk van de cellen van de kolom aan te passen. |
### getField() {#getField--}
```
public abstract int getField()
```


Haalt kolomveld op. `Field`([getField()](../../com.aspose.tasks/viewcolumn\#getField--)/[setField(int)](../../com.aspose.tasks/viewcolumn\#setField-int-)).

**Returns:**
int - kolomveld.
### getName() {#getName--}
```
public final String getName()
```


Haalt de kolomnaam op.

**Returns:**
java.lang.String - de kolomnaam.
### getStringAlignment() {#getStringAlignment--}
```
public final int getStringAlignment()
```


Haalt de uitlijning van de tekst op (kan een van de waarden van de enumeratie [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) zijn).

**Returns:**
int - uitlijning van de tekst (kan een van de waarden van de [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) enumeratie zijn).
### getTextStyleModificationCallback() {#getTextStyleModificationCallback--}
```
public final ITextStyleModificationCallback getTextStyleModificationCallback()
```


Haalt de callback op die kan worden gebruikt om het uiterlijk van de cellen van de kolom aan te passen.

**Returns:**
[ITextStyleModificationCallback](../../com.aspose.tasks/itextstylemodificationcallback) - the callback which can be used to customize the appearance of the column's cells.
### getWidth() {#getWidth--}
```
public final int getWidth()
```


Haalt de kolombreedte op.

**Returns:**
int - de kolombreedte.
### setField(int value) {#setField-int-}
```
public abstract void setField(int value)
```


Stelt kolomveld in. `Field`([getField()](../../com.aspose.tasks/viewcolumn\#getField--)/[setField(int)](../../com.aspose.tasks/viewcolumn\#setField-int-)).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | kolomveld. |

### setStringAlignment(int value) {#setStringAlignment-int-}
```
public final void setStringAlignment(int value)
```


Stelt de uitlijning van de tekst in (kan een van de waarden van de [HorizontalStringAlignment](../../com.aspose/tasks/horizontalstringalignment) enumeratie zijn).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | int | uitlijning van de tekst (kan een van de waarden van de [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) enumeratie zijn). |

### setTextStyleModificationCallback(ITextStyleModificationCallback value) {#setTextStyleModificationCallback-com.aspose.tasks.ITextStyleModificationCallback-}
```
public final void setTextStyleModificationCallback(ITextStyleModificationCallback value)
```


Stelt de callback in die kan worden gebruikt om het uiterlijk van de cellen van de kolom aan te passen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [ITextStyleModificationCallback](../../com.aspose.tasks/itextstylemodificationcallback) | de callback die kan worden gebruikt om het uiterlijk van de cellen van de kolom aan te passen. |

