---
title: TableTextStyle
second_title: Aspose.Tasks for Java API Reference
description: Represents a text style in a view table.
type: docs
weight: 287
url: /java/com.aspose.tasks/tabletextstyle/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.TextStyle](../../com.aspose.tasks/textstyle)
```
public class TableTextStyle extends TextStyle
```

Represents a text style in a view table.
## Constructors

| Constructor | Description |
| --- | --- |
| [TableTextStyle(int rowUid)](#TableTextStyle-int-) | Initializes a new instance of the [TableTextStyle](../../com.aspose.tasks/tabletextstyle) class. |
| [TableTextStyle(int rowUid, FontDescriptor font)](#TableTextStyle-int-com.aspose.tasks.FontDescriptor-) | Initializes a new instance of the [TableTextStyle](../../com.aspose.tasks/tabletextstyle) class with the specified font. |
| [TableTextStyle(int rowUid, float fontSize, int fontStyle)](#TableTextStyle-int-float-int-) | Initializes a new instance of the [TableTextStyle](../../com.aspose.tasks/tabletextstyle) class with the specified font size and font style. |
| [TableTextStyle(int rowUid, int fontStyle)](#TableTextStyle-int-int-) | Initializes a new instance of the [TableTextStyle](../../com.aspose.tasks/tabletextstyle) class with the default font settings and the specified font style. |
## Methods

| Method | Description |
| --- | --- |
| [getField()](#getField--) | Gets a field the style is to be applied to. |
| [getItemType()](#getItemType--) | Returns text item type. |
| [getRowUid()](#getRowUid--) | Gets a row unique id. |
| [setField(int value)](#setField-int-) | Sets a field the style is to be applied to. |
### TableTextStyle(int rowUid) {#TableTextStyle-int-}
```
public TableTextStyle(int rowUid)
```


Initializes a new instance of the [TableTextStyle](../../com.aspose.tasks/tabletextstyle) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowUid | int | A specified row unique id. |

### TableTextStyle(int rowUid, FontDescriptor font) {#TableTextStyle-int-com.aspose.tasks.FontDescriptor-}
```
public TableTextStyle(int rowUid, FontDescriptor font)
```


Initializes a new instance of the [TableTextStyle](../../com.aspose.tasks/tabletextstyle) class with the specified font.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowUid | int | A specified row unique id. |
| font | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | A font on which a text style is based on. |

### TableTextStyle(int rowUid, float fontSize, int fontStyle) {#TableTextStyle-int-float-int-}
```
public TableTextStyle(int rowUid, float fontSize, int fontStyle)
```


Initializes a new instance of the [TableTextStyle](../../com.aspose.tasks/tabletextstyle) class with the specified font size and font style.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowUid | int | A specified row unique id. |
| fontSize | float | Size of a font on which a text style is based on. |
| fontStyle | int | Font style. |

### TableTextStyle(int rowUid, int fontStyle) {#TableTextStyle-int-int-}
```
public TableTextStyle(int rowUid, int fontStyle)
```


Initializes a new instance of the [TableTextStyle](../../com.aspose.tasks/tabletextstyle) class with the default font settings and the specified font style.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowUid | int | A specified row unique id. |
| fontStyle | int | Font style. |

### getField() {#getField--}
```
public final int getField()
```


Gets a field the style is to be applied to. `Field`([getField()](../../com.aspose.tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Returns:**
int - a field the style is to be applied to.
### getItemType() {#getItemType--}
```
public int getItemType()
```


Returns text item type.

**Returns:**
int - TextItemType enumerated type value.
### getRowUid() {#getRowUid--}
```
public final int getRowUid()
```


Gets a row unique id.

--------------------

Return -1 if the style is to be applied to all rows of a view.

**Returns:**
int - a row unique id.
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


Sets a field the style is to be applied to. `Field`([getField()](../../com.aspose.tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a field the style is to be applied to. |

