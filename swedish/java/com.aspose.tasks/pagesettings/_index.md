---
title: "PageSettings"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar utskriftsinställningar för en sida i projektvyn."
type: docs
weight: 181
url: /sv/java/com.aspose.tasks/pagesettings/
---

**Inheritance:**
java.lang.Object
```
public class PageSettings
```

Representerar utskriftsinställningar för en sida i projektvyn.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [PageSettings()](#PageSettings--) | Initierar en ny instans av klassen [PageSettings](../../com.aspose.tasks/pagesettings). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getAdjustToPercentOfNormalSize()](#getAdjustToPercentOfNormalSize--) | Hämtar ett värde som indikerar om utskriften ska justeras till den angivna procentsatsen (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) av normal storlek. |
| [getFirstPageNumber()](#getFirstPageNumber--) | Hämtar ett första sidnummer för utskrift. |
| [getPagesInHeight()](#getPagesInHeight--) | Hämtar ett antal sidor i höjd som ska skrivas ut. |
| [getPagesInWidth()](#getPagesInWidth--) | Hämtar ett antal sidor i bredd som ska skrivas ut. |
| [getPaperSize()](#getPaperSize--) | Hämtar en pappersstorlek. |
| [getPaperSizeId()](#getPaperSizeId--) | Hämtar ett heltal som representerar ett av värdena i PrinterPaperSize eller ett anpassat sidstorleks‑ID. |
| [getPercentOfNormalSize()](#getPercentOfNormalSize--) | Hämtar en procentsats av normal storlek att justera utskriften till. |
| [isPortrait()](#isPortrait--) | Hämtar ett värde som indikerar om sidorienteringen är stående; returnerar false om sidorienteringen är liggande. |
| [setAdjustToPercentOfNormalSize(boolean value)](#setAdjustToPercentOfNormalSize-boolean-) | Ställer in ett värde som indikerar om utskriften ska justeras till den angivna procentsatsen (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) av normal storlek. |
| [setFirstPageNumber(short value)](#setFirstPageNumber-short-) | Ställer in ett första sidnummer för utskrift. |
| [setPagesInHeight(int value)](#setPagesInHeight-int-) | Ställer in ett antal sidor i höjd som ska skrivas ut. |
| [setPagesInWidth(int value)](#setPagesInWidth-int-) | Ställer in ett antal sidor i bredd som ska skrivas ut. |
| [setPaperSize(int value)](#setPaperSize-int-) | Ställer in en pappersstorlek. |
| [setPaperSizeId(int value)](#setPaperSizeId-int-) | Ställer in ett heltal som representerar ett av värdena i PrinterPaperSize eller ett anpassat sidstorleks‑ID. |
| [setPercentOfNormalSize(int value)](#setPercentOfNormalSize-int-) | Ställer in en procentsats av normal storlek att justera utskriften till. |
| [setPortrait(boolean value)](#setPortrait-boolean-) | Ställer in ett värde som indikerar om sidorienteringen är stående; returnerar false om sidorienteringen är liggande. |
### PageSettings() {#PageSettings--}
```
public PageSettings()
```


Initierar en ny instans av klassen [PageSettings](../../com.aspose.tasks/pagesettings) . Representerar utskriftsinställningar för en sida i projektvyn.

### getAdjustToPercentOfNormalSize() {#getAdjustToPercentOfNormalSize--}
```
public final boolean getAdjustToPercentOfNormalSize()
```


Hämtar ett värde som indikerar om utskriften ska justeras till den angivna procentsatsen (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) av normal storlek.

--------------------

Har ingen effekt när projektet renderas i HTML-format.

**Returns:**
boolean - ett värde som indikerar om utskriften ska justeras till den angivna procentsatsen (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) av normal storlek.
### getFirstPageNumber() {#getFirstPageNumber--}
```
public final short getFirstPageNumber()
```


Hämtar ett första sidnummer för utskrift.

**Returns:**
short - ett första sidnummer för utskrift.
### getPagesInHeight() {#getPagesInHeight--}
```
public final int getPagesInHeight()
```


Hämtar ett antal sidor i höjd som ska skrivas ut.

**Returns:**
int - ett antal sidor i höjd som ska skrivas ut.
### getPagesInWidth() {#getPagesInWidth--}
```
public final int getPagesInWidth()
```


Hämtar ett antal sidor i bredd som ska skrivas ut.

**Returns:**
int - ett antal sidor i bredd som ska skrivas ut.
### getPaperSize() {#getPaperSize--}
```
public final int getPaperSize()
```


Hämtar en pappersstorlek. Kan vara ett av värdena i uppräkningen [PrinterPaperSize](../../com.aspose.tasks/printerpapersize).

**Returns:**
int - en pappersstorlek.
### getPaperSizeId() {#getPaperSizeId--}
```
public final int getPaperSizeId()
```


Hämtar ett heltal som representerar ett av värdena i PrinterPaperSize eller ett anpassat sidstorleks‑ID. Detta värde kan användas för att hämta PaperSize från OS‑inställningarna ().

**Returns:**
int - ett heltal som representerar ett av PrinterPaperSize-värdena eller ett anpassat sidstorleks-ID.
### getPercentOfNormalSize() {#getPercentOfNormalSize--}
```
public final int getPercentOfNormalSize()
```


Hämtar en procentsats av normal storlek att justera utskriften till.

**Returns:**
int - en procentsats av normal storlek att justera utskrift till.
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


Hämtar ett värde som indikerar om sidorienteringen är stående; returnerar false om sidorienteringen är liggande.

--------------------

Gäller vid rendering när SaveOptions.getPageSize() == PageSize.DefinedInView.

**Returns:**
boolean - ett värde som indikerar om sidorienteringen är stående; returnerar false om sidorienteringen är liggande.
### setAdjustToPercentOfNormalSize(boolean value) {#setAdjustToPercentOfNormalSize-boolean-}
```
public final void setAdjustToPercentOfNormalSize(boolean value)
```


Ställer in ett värde som indikerar om utskriften ska justeras till den angivna procentsatsen (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) av normal storlek.

--------------------

Har ingen effekt när projektet renderas i HTML-format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | boolean | ett värde som indikerar om utskriften ska justeras till den angivna procentsatsen (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose.tasks/pagesettings\#setPercentOfNormalSize-int-))) av normal storlek. |

### setFirstPageNumber(short value) {#setFirstPageNumber-short-}
```
public final void setFirstPageNumber(short value)
```


Ställer in ett första sidnummer för utskrift.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | short | ett första sidnummer för utskrift. |

### setPagesInHeight(int value) {#setPagesInHeight-int-}
```
public final void setPagesInHeight(int value)
```


Ställer in ett antal sidor i höjd som ska skrivas ut.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett antal sidor i höjd som ska skrivas ut. |

### setPagesInWidth(int value) {#setPagesInWidth-int-}
```
public final void setPagesInWidth(int value)
```


Ställer in ett antal sidor i bredd som ska skrivas ut.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett antal sidor i bredd som ska skrivas ut. |

### setPaperSize(int value) {#setPaperSize-int-}
```
public final void setPaperSize(int value)
```


Ställer in en papperstorlek. Kan vara ett av värdena i uppräkningen [PrinterPaperSize](../../com.aspose.tasks/printerpapersize).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | en papperstorlek. |

### setPaperSizeId(int value) {#setPaperSizeId-int-}
```
public final void setPaperSizeId(int value)
```


Ställer in ett heltal som representerar ett av PrinterPaperSize-värdena eller ett anpassat sidstorleks-ID. Detta värde kan användas för att hämta PaperSize från OS-inställningarna ().

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett heltal som representerar ett av PrinterPaperSize-värdena eller ett anpassat sidstorleks-ID. |

### setPercentOfNormalSize(int value) {#setPercentOfNormalSize-int-}
```
public final void setPercentOfNormalSize(int value)
```


Ställer in en procentsats av normal storlek att justera utskriften till.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | en procentsats av normal storlek att justera utskrift till. |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


Ställer in ett värde som indikerar om sidorienteringen är stående; returnerar false om sidorienteringen är liggande.

--------------------

Gäller vid rendering när SaveOptions.getPageSize() == PageSize.DefinedInView.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om sidorienteringen är stående; returnerar false om sidorienteringen är liggande. |

