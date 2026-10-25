---
title: "PageSettings"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt afdrukinstellingen voor een pagina van de projectweergave voor."
type: docs
weight: 181
url: /nl/java/com.aspose.tasks/pagesettings/
---

**Inheritance:**
java.lang.Object
```
public class PageSettings
```

Stelt afdrukinstellingen voor een pagina van de projectweergave voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [PageSettings()](#PageSettings--) | Initialiseert een nieuw exemplaar van de [PageSettings](../../com.aspose.tasks/pagesettings) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getAdjustToPercentOfNormalSize()](#getAdjustToPercentOfNormalSize--) | Haalt een waarde op die aangeeft of het afdrukken moet worden aangepast naar het opgegeven percentage (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) van de normale grootte. |
| [getFirstPageNumber()](#getFirstPageNumber--) | Haalt het eerste paginanummer op voor afdrukken. |
| [getPagesInHeight()](#getPagesInHeight--) | Haalt een aantal pagina's in hoogte op die moeten worden afgedrukt. |
| [getPagesInWidth()](#getPagesInWidth--) | Haalt een aantal pagina's in breedte op die moeten worden afgedrukt. |
| [getPaperSize()](#getPaperSize--) | Haalt een papierformaat op. |
| [getPaperSizeId()](#getPaperSizeId--) | Haalt een geheel getal op dat een van de PrinterPaperSize-waarden of een aangepast paginagrootte-id vertegenwoordigt. |
| [getPercentOfNormalSize()](#getPercentOfNormalSize--) | Haalt een percentage van de normale grootte op om het afdrukken aan te passen. |
| [isPortrait()](#isPortrait--) | Haalt een waarde op die aangeeft of de paginarichting portret is; retourneert false als de paginarichting landschap is. |
| [setAdjustToPercentOfNormalSize(boolean value)](#setAdjustToPercentOfNormalSize-boolean-) | Stelt een waarde in die aangeeft of het afdrukken moet worden aangepast naar het opgegeven percentage (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) van de normale grootte. |
| [setFirstPageNumber(short value)](#setFirstPageNumber-short-) | Stelt het eerste paginanummer in voor afdrukken. |
| [setPagesInHeight(int value)](#setPagesInHeight-int-) | Stelt een aantal pagina's in hoogte in die moeten worden afgedrukt. |
| [setPagesInWidth(int value)](#setPagesInWidth-int-) | Stelt een aantal pagina's in breedte in die moeten worden afgedrukt. |
| [setPaperSize(int value)](#setPaperSize-int-) | Stelt een papierformaat in. |
| [setPaperSizeId(int value)](#setPaperSizeId-int-) | Stelt een geheel getal in dat een van de PrinterPaperSize-waarden of een aangepast paginagrootte-id vertegenwoordigt. |
| [setPercentOfNormalSize(int value)](#setPercentOfNormalSize-int-) | Stelt een percentage van de normale grootte in om het afdrukken aan te passen. |
| [setPortrait(boolean value)](#setPortrait-boolean-) | Stelt een waarde in die aangeeft of de paginarichting portret is; retourneert false als de paginarichting landschap is. |
### PageSettings() {#PageSettings--}
```
public PageSettings()
```


Initialiseert een nieuwe instantie van de [PageSettings](../../com.aspose/tasks/pagesettings) klasse. Vertegenwoordigt afdrukinstellingen voor een pagina van de projectweergave.

### getAdjustToPercentOfNormalSize() {#getAdjustToPercentOfNormalSize--}
```
public final boolean getAdjustToPercentOfNormalSize()
```


Haalt een waarde op die aangeeft of het afdrukken moet worden aangepast naar het opgegeven percentage (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) van de normale grootte.

--------------------

Is niet effectief wanneer het project wordt gerenderd in HTML-indeling.

**Returns:**
boolean - een waarde die aangeeft of het afdrukken moet worden aangepast naar het opgegeven percentage (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) van de normale grootte.
### getFirstPageNumber() {#getFirstPageNumber--}
```
public final short getFirstPageNumber()
```


Haalt het eerste paginanummer op voor afdrukken.

**Returns:**
short - een eerste paginanummer voor afdrukken.
### getPagesInHeight() {#getPagesInHeight--}
```
public final int getPagesInHeight()
```


Haalt een aantal pagina's in hoogte op die moeten worden afgedrukt.

**Returns:**
int - een aantal pagina's in hoogte die moeten worden afgedrukt.
### getPagesInWidth() {#getPagesInWidth--}
```
public final int getPagesInWidth()
```


Haalt een aantal pagina's in breedte op die moeten worden afgedrukt.

**Returns:**
int - een aantal pagina's in breedte die moeten worden afgedrukt.
### getPaperSize() {#getPaperSize--}
```
public final int getPaperSize()
```


Haalt een papierformaat op. Kan een van de waarden van de [PrinterPaperSize](../../com.aspose/tasks/printerpapersize) enumeratie zijn.

**Returns:**
int - een papierformaat.
### getPaperSizeId() {#getPaperSizeId--}
```
public final int getPaperSizeId()
```


Haalt een geheel getal op dat een van de PrinterPaperSize-waarden of een aangepast paginagrootte-id vertegenwoordigt. Deze waarde kan worden gebruikt om PaperSize op te halen uit de OS-instellingen ().

**Returns:**
int - een geheel getal dat een van de PrinterPaperSize-waarden of een aangepaste paginagrootte-id vertegenwoordigt.
### getPercentOfNormalSize() {#getPercentOfNormalSize--}
```
public final int getPercentOfNormalSize()
```


Haalt een percentage van de normale grootte op om het afdrukken aan te passen.

**Returns:**
int - een percentage van de normale grootte om de afdruk aan te passen.
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


Haalt een waarde op die aangeeft of de paginarichting portret is; retourneert false als de paginarichting landschap is.

--------------------

Is van toepassing tijdens het renderen wanneer SaveOptions.getPageSize() == PageSize.DefinedInView.

**Returns:**
boolean - een waarde die aangeeft of de paginarichting portret is; retourneert false als de paginarichting landschap is.
### setAdjustToPercentOfNormalSize(boolean value) {#setAdjustToPercentOfNormalSize-boolean-}
```
public final void setAdjustToPercentOfNormalSize(boolean value)
```


Stelt een waarde in die aangeeft of het afdrukken moet worden aangepast naar het opgegeven percentage (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) van de normale grootte.

--------------------

Is niet effectief wanneer het project wordt gerenderd in HTML-indeling.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | boolean | een waarde die aangeeft of het afdrukken moet worden aangepast naar het opgegeven percentage (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose.tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose.tasks/pagesettings\#setPercentOfNormalSize-int-))) van de normale grootte. |

### setFirstPageNumber(short value) {#setFirstPageNumber-short-}
```
public final void setFirstPageNumber(short value)
```


Stelt het eerste paginanummer in voor afdrukken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | short | een eerste paginanummer voor afdrukken. |

### setPagesInHeight(int value) {#setPagesInHeight-int-}
```
public final void setPagesInHeight(int value)
```


Stelt een aantal pagina's in hoogte in die moeten worden afgedrukt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een aantal pagina's in hoogte die moeten worden afgedrukt. |

### setPagesInWidth(int value) {#setPagesInWidth-int-}
```
public final void setPagesInWidth(int value)
```


Stelt een aantal pagina's in breedte in die moeten worden afgedrukt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een aantal pagina's in breedte die moeten worden afgedrukt. |

### setPaperSize(int value) {#setPaperSize-int-}
```
public final void setPaperSize(int value)
```


Stelt een papierformaat in. Kan een van de waarden van de [PrinterPaperSize](../../com.aspose.tasks/printerpapersize) enumeratie zijn.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een papierformaat. |

### setPaperSizeId(int value) {#setPaperSizeId-int-}
```
public final void setPaperSizeId(int value)
```


Stelt een geheel getal in dat een van de PrinterPaperSize-waarden of een aangepaste paginagrootte-id vertegenwoordigt. Deze waarde kan worden gebruikt om PaperSize op te halen uit de OS-instellingen ().

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een geheel getal dat een van de PrinterPaperSize-waarden of een aangepaste paginagrootte-id vertegenwoordigt. |

### setPercentOfNormalSize(int value) {#setPercentOfNormalSize-int-}
```
public final void setPercentOfNormalSize(int value)
```


Stelt een percentage van de normale grootte in om het afdrukken aan te passen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een percentage van de normale grootte om de afdruk aan te passen. |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


Stelt een waarde in die aangeeft of de paginarichting portret is; retourneert false als de paginarichting landschap is.

--------------------

Is van toepassing tijdens het renderen wanneer SaveOptions.getPageSize() == PageSize.DefinedInView.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of de paginarichting portret is; retourneert false als de paginarichting landschap is. |

