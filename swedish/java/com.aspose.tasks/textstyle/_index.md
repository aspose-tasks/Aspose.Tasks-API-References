---
title: "TextStyle"
second_title: "Aspose.Tasks for Java API-referens"
description: "Ändra den visuella stilen på texten för ett objekt i projektsvyn."
type: docs
weight: 315
url: /sv/java/com.aspose.tasks/textstyle/
---

**Inheritance:**
java.lang.Object
```
public class TextStyle
```

Ändra den visuella stilen på texten för ett objekt i projektsvyn.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [TextStyle()](#TextStyle--) | Initierar en ny instans av klassen [TextStyle](../../com.aspose.tasks/textstyle) med standardinställningar. |
| [TextStyle(float fontSize, int fontStyle)](#TextStyle-float-int-) | Initierar en ny instans av klassen [TextStyle](../../com.aspose.tasks/textstyle) med standardtypsnittet och angiven teckenstorlek och stil. |
| [TextStyle(int fontStyle)](#TextStyle-int-) | Initierar en ny instans av klassen [TextStyle](../../com.aspose.tasks/textstyle) med standardtypsnittet och angiven typsnittsstil. |
| [TextStyle(FontDescriptor font)](#TextStyle-com.aspose.tasks.FontDescriptor-) | Initierar en ny instans av klassen [TextStyle](../../com.aspose.tasks/textstyle) med angivna typsnittsinställningar. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getBackgroundColor()](#getBackgroundColor--) | Hämtar bakgrundsfärg för textstilen. |
| [getBackgroundPattern()](#getBackgroundPattern--) | Hämtar bakgrundsmönster för textstilen. |
| [getColor()](#getColor--) | Hämtar färgen på texten. |
| [getFont()](#getFont--) | Hämtar teckensnittet för textstilen. |
| [getItemType()](#getItemType--) | Hämtar [TextItemType](../../com.aspose/tasks/textitemtype) för textstilen. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | Ställer in bakgrundsfärgen för textstilen. |
| [setBackgroundPattern(int value)](#setBackgroundPattern-int-) | Ställer in bakgrundsmönstret för textstilen. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Ställer in färgen på texten. |
| [setFont(FontDescriptor value)](#setFont-com.aspose.tasks.FontDescriptor-) | Ställer in teckensnittet för textstilen. |
| [setItemType(int value)](#setItemType-int-) | Ställer in [TextItemType](../../com.aspose/tasks/textitemtype) för textstilen. |
### TextStyle() {#TextStyle--}
```
public TextStyle()
```


Initierar en ny instans av klassen [TextStyle](../../com.aspose.tasks/textstyle) med standardinställningar.

### TextStyle(float fontSize, int fontStyle) {#TextStyle-float-int-}
```
public TextStyle(float fontSize, int fontStyle)
```


Initierar en ny instans av klassen [TextStyle](../../com.aspose.tasks/textstyle) med standardtypsnittet och angiven teckenstorlek och stil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fontSize | float | Storlek på teckensnittet för TextStyle. |
| fontStyle | int | Stil på teckensnittet för TextStyle. |

### TextStyle(int fontStyle) {#TextStyle-int-}
```
public TextStyle(int fontStyle)
```


Initierar en ny instans av klassen [TextStyle](../../com.aspose.tasks/textstyle) med standardtypsnittet och angiven typsnittsstil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fontStyle | int | Stil på teckensnittet att tillämpa på standardteckensnittet. |

### TextStyle(FontDescriptor font) {#TextStyle-com.aspose.tasks.FontDescriptor-}
```
public TextStyle(FontDescriptor font)
```


Initierar en ny instans av klassen [TextStyle](../../com.aspose.tasks/textstyle) med angivna typsnittsinställningar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| font | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | Teckensnitt för TextStyle. |

### getBackgroundColor() {#getBackgroundColor--}
```
public final Color getBackgroundColor()
```


Hämtar bakgrundsfärgen för textstilen. `Color`([getBackgroundColor()](../../com.aspose/tasks/textstyle\#getBackgroundColor--)/[setBackgroundColor(java.awt.Color)](../../com.aspose/tasks/textstyle\#setBackgroundColor-java.awt.Color-)).

**Returns:**
java.awt.Color - bakgrundsfärgen för textstilen.
### getBackgroundPattern() {#getBackgroundPattern--}
```
public final int getBackgroundPattern()
```


Hämtar bakgrundsmönstret för textstilen. `BackgroundPattern`([getBackgroundPattern()](../../com.aspose/tasks/textstyle\#getBackgroundPattern--)/[setBackgroundPattern(int)](../../com.aspose/tasks/textstyle\#setBackgroundPattern-int-)).

**Returns:**
int - bakgrundsmönster för textstilen.
### getColor() {#getColor--}
```
public final Color getColor()
```


Hämtar färgen på texten.

**Returns:**
java.awt.Color - färg på texten.
### getFont() {#getFont--}
```
public final FontDescriptor getFont()
```


Hämtar teckensnittet för textstilen.

**Returns:**
[FontDescriptor](../../com.aspose.tasks/fontdescriptor) - font of the text style.
### getItemType() {#getItemType--}
```
public int getItemType()
```


Hämtar [TextItemType](../../com.aspose/tasks/textitemtype) för textstilen.

**Returns:**
int - [TextItemType](../../com.aspose/tasks/textitemtype) för textstilen.
### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public final void setBackgroundColor(Color value)
```


Ställer in bakgrundsfärgen för textstilen. `Color`([getBackgroundColor()](../../com.aspose/tasks/textstyle\#getBackgroundColor--)/[setBackgroundColor(java.awt.Color)](../../com.aspose/tasks/textstyle\#setBackgroundColor-java.awt.Color-)).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.awt.Color | bakgrundsfärgen för textstilen. |

### setBackgroundPattern(int value) {#setBackgroundPattern-int-}
```
public final void setBackgroundPattern(int value)
```


Ställer in bakgrundsmönstret för textstilen. `BackgroundPattern`([getBackgroundPattern()](../../com.aspose/tasks/textstyle\#getBackgroundPattern--)/[setBackgroundPattern(int)](../../com.aspose/tasks/textstyle\#setBackgroundPattern-int-)).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | bakgrundsmönster för textstilen. |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public final void setColor(Color value)
```


Ställer in färgen på texten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.awt.Color | färg på texten. |

### setFont(FontDescriptor value) {#setFont-com.aspose.tasks.FontDescriptor-}
```
public final void setFont(FontDescriptor value)
```


Ställer in teckensnittet för textstilen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | teckensnitt för textstilen. |

### setItemType(int value) {#setItemType-int-}
```
public void setItemType(int value)
```


Ställer in [TextItemType](../../com.aspose/tasks/textitemtype) för textstilen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | int | [TextItemType](../../com.aspose.tasks/textitemtype) för textstilen. |

