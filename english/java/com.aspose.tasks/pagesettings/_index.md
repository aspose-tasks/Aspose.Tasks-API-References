---
title: PageSettings
second_title: Aspose.Tasks for Java API Reference
description: Represents printing settings for a page of project view.
type: docs
weight: 170
url: /java/com.aspose.tasks/pagesettings/
---

**Inheritance:**
java.lang.Object
```
public class PageSettings
```

Represents printing settings for a page of project view.
## Constructors

| Constructor | Description |
| --- | --- |
| [PageSettings()](#PageSettings--) | Initializes a new instance of the [PageSettings](../../com.aspose.tasks/pagesettings) class. |
## Methods

| Method | Description |
| --- | --- |
| [getAdjustToPercentOfNormalSize()](#getAdjustToPercentOfNormalSize--) | Gets a value indicating whether to adjust printing to the specified percentage ( PercentOfNormalSize ([getPercentOfNormalSize()](../../com.aspose.tasks/pagesettings\#getPercentOfNormalSize--)/[setPercentOfNormalSize(int)](../../com.aspose.tasks/pagesettings\#setPercentOfNormalSize-int-))) of normal size. |
| [getFirstPageNumber()](#getFirstPageNumber--) | Gets a first page number for printing. |
| [getPagesInHeight()](#getPagesInHeight--) | Gets a number of pages in height to be printed. |
| [getPagesInWidth()](#getPagesInWidth--) | Gets a number of pages in width to be printed. |
| [getPaperSize()](#getPaperSize--) | Gets a paper size. |
| [getPaperSizeId()](#getPaperSizeId--) | Gets an integer representing one of the PrinterPaperSize values or a custom page size id. |
| [getPercentOfNormalSize()](#getPercentOfNormalSize--) | Gets a percentage of normal size to adjust printing to. |
| [isPortrait()](#isPortrait--) | Gets a value indicating whether the page orientation is portrait; returns false if the page orientation is landscape. |
| [setAdjustToPercentOfNormalSize(boolean value)](#setAdjustToPercentOfNormalSize-boolean-) | Sets a value indicating whether to adjust printing to the specified percentage ( PercentOfNormalSize ([getPercentOfNormalSize()](../../com.aspose.tasks/pagesettings\#getPercentOfNormalSize--)/[setPercentOfNormalSize(int)](../../com.aspose.tasks/pagesettings\#setPercentOfNormalSize-int-))) of normal size. |
| [setFirstPageNumber(short value)](#setFirstPageNumber-short-) | Sets a first page number for printing. |
| [setPagesInHeight(int value)](#setPagesInHeight-int-) | Sets a number of pages in height to be printed. |
| [setPagesInWidth(int value)](#setPagesInWidth-int-) | Sets a number of pages in width to be printed. |
| [setPaperSize(int value)](#setPaperSize-int-) | Sets a paper size. |
| [setPaperSizeId(int value)](#setPaperSizeId-int-) | Sets an integer representing one of the PrinterPaperSize values or a custom page size id. |
| [setPercentOfNormalSize(int value)](#setPercentOfNormalSize-int-) | Sets a percentage of normal size to adjust printing to. |
| [setPortrait(boolean value)](#setPortrait-boolean-) | Sets a value indicating whether the page orientation is portrait; returns false if the page orientation is landscape. |
### PageSettings() {#PageSettings--}
```
public PageSettings()
```


Initializes a new instance of the [PageSettings](../../com.aspose.tasks/pagesettings) class. Represents printing settings for a page of project view.

### getAdjustToPercentOfNormalSize() {#getAdjustToPercentOfNormalSize--}
```
public final boolean getAdjustToPercentOfNormalSize()
```


Gets a value indicating whether to adjust printing to the specified percentage ( PercentOfNormalSize ([getPercentOfNormalSize()](../../com.aspose.tasks/pagesettings\#getPercentOfNormalSize--)/[setPercentOfNormalSize(int)](../../com.aspose.tasks/pagesettings\#setPercentOfNormalSize-int-))) of normal size.

--------------------

Is not effective when project is rendered in HTML format.

**Returns:**
boolean - a value indicating whether to adjust printing to the specified percentage ( PercentOfNormalSize ([getPercentOfNormalSize()](../../com.aspose.tasks/pagesettings\#getPercentOfNormalSize--)/[setPercentOfNormalSize(int)](../../com.aspose.tasks/pagesettings\#setPercentOfNormalSize-int-))) of normal size.
### getFirstPageNumber() {#getFirstPageNumber--}
```
public final short getFirstPageNumber()
```


Gets a first page number for printing.

**Returns:**
short - a first page number for printing.
### getPagesInHeight() {#getPagesInHeight--}
```
public final int getPagesInHeight()
```


Gets a number of pages in height to be printed.

**Returns:**
int - a number of pages in height to be printed.
### getPagesInWidth() {#getPagesInWidth--}
```
public final int getPagesInWidth()
```


Gets a number of pages in width to be printed.

**Returns:**
int - a number of pages in width to be printed.
### getPaperSize() {#getPaperSize--}
```
public final int getPaperSize()
```


Gets a paper size. Can be one of the values of the [PrinterPaperSize](../../com.aspose.tasks/printerpapersize) enumeration.

**Returns:**
int - a paper size.
### getPaperSizeId() {#getPaperSizeId--}
```
public final int getPaperSizeId()
```


Gets an integer representing one of the PrinterPaperSize values or a custom page size id. This value can be used to get PaperSize from OS settings ().

**Returns:**
int - an integer representing one of the PrinterPaperSize values or a custom page size id.
### getPercentOfNormalSize() {#getPercentOfNormalSize--}
```
public final int getPercentOfNormalSize()
```


Gets a percentage of normal size to adjust printing to.

**Returns:**
int - a percentage of normal size to adjust printing to.
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


Gets a value indicating whether the page orientation is portrait; returns false if the page orientation is landscape.

**Returns:**
boolean - a value indicating whether the page orientation is portrait; returns false if the page orientation is landscape.
### setAdjustToPercentOfNormalSize(boolean value) {#setAdjustToPercentOfNormalSize-boolean-}
```
public final void setAdjustToPercentOfNormalSize(boolean value)
```


Sets a value indicating whether to adjust printing to the specified percentage ( PercentOfNormalSize ([getPercentOfNormalSize()](../../com.aspose.tasks/pagesettings\#getPercentOfNormalSize--)/[setPercentOfNormalSize(int)](../../com.aspose.tasks/pagesettings\#setPercentOfNormalSize-int-))) of normal size.

--------------------

Is not effective when project is rendered in HTML format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to adjust printing to the specified percentage ( PercentOfNormalSize ([getPercentOfNormalSize()](../../com.aspose.tasks/pagesettings\#getPercentOfNormalSize--)/[setPercentOfNormalSize(int)](../../com.aspose.tasks/pagesettings\#setPercentOfNormalSize-int-))) of normal size. |

### setFirstPageNumber(short value) {#setFirstPageNumber-short-}
```
public final void setFirstPageNumber(short value)
```


Sets a first page number for printing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | short | a first page number for printing. |

### setPagesInHeight(int value) {#setPagesInHeight-int-}
```
public final void setPagesInHeight(int value)
```


Sets a number of pages in height to be printed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a number of pages in height to be printed. |

### setPagesInWidth(int value) {#setPagesInWidth-int-}
```
public final void setPagesInWidth(int value)
```


Sets a number of pages in width to be printed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a number of pages in width to be printed. |

### setPaperSize(int value) {#setPaperSize-int-}
```
public final void setPaperSize(int value)
```


Sets a paper size. Can be one of the values of the [PrinterPaperSize](../../com.aspose.tasks/printerpapersize) enumeration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a paper size. |

### setPaperSizeId(int value) {#setPaperSizeId-int-}
```
public final void setPaperSizeId(int value)
```


Sets an integer representing one of the PrinterPaperSize values or a custom page size id. This value can be used to get PaperSize from OS settings ().

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | an integer representing one of the PrinterPaperSize values or a custom page size id. |

### setPercentOfNormalSize(int value) {#setPercentOfNormalSize-int-}
```
public final void setPercentOfNormalSize(int value)
```


Sets a percentage of normal size to adjust printing to.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a percentage of normal size to adjust printing to. |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


Sets a value indicating whether the page orientation is portrait; returns false if the page orientation is landscape.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether the page orientation is portrait; returns false if the page orientation is landscape. |

