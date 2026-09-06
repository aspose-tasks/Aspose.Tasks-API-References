---
title: "ImageSaveOptions"
second_title: "Aspose.Tasks for Java API-referens"
description: "Tillåter att ange ytterligare alternativ när projektssidor renderas till bilder."
type: docs
weight: 134
url: /sv/java/com.aspose.tasks/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class ImageSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Tillåter att ange ytterligare alternativ när projektssidor renderas till bilder.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ImageSaveOptions(int saveFormat)](#ImageSaveOptions-int-) | Initierar en ny instans av klassen [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) som kan användas för att spara renderade bilder i TIFF, PNG, BMP eller JPEG-format. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getFontSettings()](#getFontSettings--) | Anger teckensnittsinställningar som används när projektets vy renderas. |
| [getHorizontalResolution()](#getHorizontalResolution--) | Hämtar den horisontella upplösningen i dpi. |
| [getJpegQuality()](#getJpegQuality--) | Hämtar en JPEG-kvalitet. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Hämtar en användardefinierad återuppringning som används för att få en utström för varje renderad sida. |
| [getPages()](#getPages--) | Hämtar en lista med sidnummer att spara när projektlayouten sparas till separata filer. |
| [getPixelFormat()](#getPixelFormat--) | Hämtar formatet för färgdata för varje pixel i bilden. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Hämtar ett värde som indikerar om ett gap mellan sista uppgiften och sidfoten ska minskas. |
| [getTiffCompression()](#getTiffCompression--) | Hämtar typen av komprimering som ska tillämpas när genererade bilder sparas i TIFF-format. |
| [getVerticalResolution()](#getVerticalResolution--) | Hämtar den vertikala upplösningen i dpi. |
| [setHorizontalResolution(float value)](#setHorizontalResolution-float-) | Ställer in den horisontella upplösningen i dpi. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | Ställer in en JPEG-kvalitet. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Ställer in ett användardefinierat återanrop som används för att hämta en utdataström för varje renderad sida. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Ställer in en lista med sidnummer att spara när projektlayouten sparas till separata filer. |
| [setPixelFormat(int value)](#setPixelFormat-int-) | Ställer in formatet för färgdata för varje pixel i bilden. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Ställer in ett värde som anger om ett mellanrum mellan sista uppgiften och sidfoten ska minskas. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Ställer in typen av komprimering som ska tillämpas när genererade bilder sparas i TIFF-format. |
| [setVerticalResolution(float value)](#setVerticalResolution-float-) | Ställer in den vertikala upplösningen i dpi. |
### ImageSaveOptions(int saveFormat) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int saveFormat)
```


Initierar en ny instans av klassen [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) som kan användas för att spara renderade bilder i TIFF, PNG, BMP eller JPEG-format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| saveFormat | int | Kan vara TIFF, PNG, BMP eller JPEG[SaveFileFormat](../../com.aspose.tasks/savefileformat). |

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public final void copyOutputPropertiesFrom(SaveOptions source)
```


Reserverad för intern användning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public SaveOptions deepClone()
```


Reserverad för intern användning.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Anger teckensnittsinställningar som används när projektets vy renderas.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getHorizontalResolution() {#getHorizontalResolution--}
```
public final float getHorizontalResolution()
```


Hämtar den horisontella upplösningen i dpi.

**Returns:**
float - den horisontella upplösningen i dpi.
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


Hämtar en JPEG‑kvalitet. Det tillåtna värdeintervallet är 0..100.

**Returns:**
int - en JPEG‑kvalitet.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Hämtar en användardefinierad återuppringning som används för att få en utström för varje renderad sida.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


Hämtar en lista med sidnummer att spara när projektlayouten sparas till separata filer.

--------------------

Alla sidor sparas om den här listan är tom.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - en lista med sidnummer att spara när projektlayouten sparas till separata filer.
### getPixelFormat() {#getPixelFormat--}
```
public final int getPixelFormat()
```


Hämtar formatet för färgdata för varje pixel i bilden.

**Returns:**
int - formatet för färgdata för varje pixel i bilden.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Hämtar ett värde som indikerar om ett gap mellan sista uppgiften och sidfoten ska minskas.

**Returns:**
boolean - ett värde som anger om ett mellanrum mellan sista uppgiften och sidfoten ska minskas.
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


Hämtar typen av komprimering som ska tillämpas när genererade bilder sparas i TIFF-format.

--------------------

Har endast effekt när du sparar till TIFF. Standardvärdet är `TiffCompressionLZW`([getTiffCompression()](../../com.aspose/tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-)).

**Returns:**
int - typen av komprimering som ska tillämpas när genererade bilder sparas i TIFF‑format.
### getVerticalResolution() {#getVerticalResolution--}
```
public final float getVerticalResolution()
```


Hämtar den vertikala upplösningen i dpi.

**Returns:**
float - den vertikala upplösningen i dpi.
### setHorizontalResolution(float value) {#setHorizontalResolution-float-}
```
public final void setHorizontalResolution(float value)
```


Ställer in den horisontella upplösningen i dpi.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float | den horisontella upplösningen i dpi. |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


Ställer in en JPEG‑kvalitet. Det tillåtna värdeintervallet är 0..100.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | en JPEG‑kvalitet. |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Ställer in ett användardefinierat återanrop som används för att hämta en utdataström för varje renderad sida.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | ett användardefinierat återanrop som används för att hämta en utström för varje renderad sida. |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


Ställer in en lista med sidnummer att spara när projektlayouten sparas till separata filer.

--------------------

Alla sidor sparas om den här listan är tom.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.List&lt;java.lang.Integer&gt; | en lista med sidnummer att spara när projektlayouten sparas till separata filer. |

### setPixelFormat(int value) {#setPixelFormat-int-}
```
public final void setPixelFormat(int value)
```


Ställer in formatet för färgdata för varje pixel i bilden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | formatet för färgdata för varje pixel i bilden. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Ställer in ett värde som anger om ett mellanrum mellan sista uppgiften och sidfoten ska minskas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som anger om ett mellanrum mellan sista uppgift och sidfot ska minskas. |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


Ställer in typen av komprimering som ska tillämpas när genererade bilder sparas i TIFF-format.

--------------------

Har endast effekt när du sparar till TIFF. Standardvärdet är `TiffCompressionLZW`([getTiffCompression()](../../com.aspose/tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-)).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | typen av komprimering som ska tillämpas när genererade bilder sparas i TIFF‑format. |

### setVerticalResolution(float value) {#setVerticalResolution-float-}
```
public final void setVerticalResolution(float value)
```


Ställer in den vertikala upplösningen i dpi.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float | den vertikala upplösningen i dpi. |

