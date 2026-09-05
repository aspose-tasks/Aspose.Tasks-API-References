---
title: "ImageSaveOptions"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Staat toe extra opties op te geven bij het renderen van projectpagina's naar afbeeldingen."
type: docs
weight: 134
url: /nl/java/com.aspose.tasks/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class ImageSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Staat toe extra opties op te geven bij het renderen van projectpagina's naar afbeeldingen.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ImageSaveOptions(int saveFormat)](#ImageSaveOptions-int-) | Initialiseert een nieuw exemplaar van de [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) klasse die kan worden gebruikt om gerenderde afbeeldingen op te slaan in TIFF-, PNG-, BMP- of JPEG-formaten. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getFontSettings()](#getFontSettings--) | Specificeert lettertype‑instellingen die worden gebruikt bij het renderen van de projectweergave. |
| [getHorizontalResolution()](#getHorizontalResolution--) | Haalt de horizontale resolutie op in dpi. |
| [getJpegQuality()](#getJpegQuality--) | Haalt een JPEG-kwaliteit op. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Haalt een door de gebruiker gedefinieerde callback op die wordt gebruikt om een uitvoerstroom voor elke gerenderde pagina te verkrijgen. |
| [getPages()](#getPages--) | Haalt een lijst met paginanummers op die moeten worden opgeslagen bij het opslaan van de projectlay-out naar afzonderlijke bestanden. |
| [getPixelFormat()](#getPixelFormat--) | Haalt het formaat van de kleurgegevens voor elke pixel in de afbeelding op. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Haalt een waarde op die aangeeft of een kloof tussen de laatste taak en de voettekst moet worden verkleind. |
| [getTiffCompression()](#getTiffCompression--) | Haalt het type compressie op dat moet worden toegepast bij het opslaan van gegenereerde afbeeldingen in het TIFF-formaat. |
| [getVerticalResolution()](#getVerticalResolution--) | Haalt de verticale resolutie op in dpi. |
| [setHorizontalResolution(float value)](#setHorizontalResolution-float-) | Stelt de horizontale resolutie in in dpi. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | Stelt een JPEG-kwaliteit in. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Stelt een door de gebruiker gedefinieerde callback in die wordt gebruikt om een output‑stream voor elke gerenderde pagina te verkrijgen. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Stelt een lijst met paginanummers in die moeten worden opgeslagen bij het opslaan van de projectlay-out naar afzonderlijke bestanden. |
| [setPixelFormat(int value)](#setPixelFormat-int-) | Stelt het formaat van de kleurgegevens voor elke pixel in de afbeelding in. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Stelt een waarde in die aangeeft of de ruimte tussen de laatste taak en de voettekst moet worden verkleind. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Stelt het type compressie in dat moet worden toegepast bij het opslaan van gegenereerde afbeeldingen in het TIFF-formaat. |
| [setVerticalResolution(float value)](#setVerticalResolution-float-) | Stelt de verticale resolutie in in dpi. |
### ImageSaveOptions(int saveFormat) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int saveFormat)
```


Initialiseert een nieuw exemplaar van de [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) klasse die kan worden gebruikt om gerenderde afbeeldingen op te slaan in TIFF-, PNG-, BMP- of JPEG-formaten.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| saveFormat | int | Kan TIFF, PNG, BMP of JPEG[SaveFileFormat](../../com.aspose.tasks/savefileformat) zijn. |

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public final void copyOutputPropertiesFrom(SaveOptions source)
```


Gereserveerd voor intern gebruik.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public SaveOptions deepClone()
```


Gereserveerd voor intern gebruik.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Specificeert lettertype‑instellingen die worden gebruikt bij het renderen van de projectweergave.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getHorizontalResolution() {#getHorizontalResolution--}
```
public final float getHorizontalResolution()
```


Haalt de horizontale resolutie op in dpi.

**Returns:**
float - de horizontale resolutie in dpi.
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


Haalt een JPEG-kwaliteit op. Het toegestane waardebereik is 0..100.

**Returns:**
int - een JPEG-kwaliteit.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Haalt een door de gebruiker gedefinieerde callback op die wordt gebruikt om een uitvoerstroom voor elke gerenderde pagina te verkrijgen.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


Haalt een lijst met paginanummers op die moeten worden opgeslagen bij het opslaan van de projectlay-out naar afzonderlijke bestanden.

--------------------

Alle pagina's worden opgeslagen als deze lijst leeg is.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - een lijst met paginanummers die moeten worden opgeslagen bij het opslaan van de projectlay-out naar afzonderlijke bestanden.
### getPixelFormat() {#getPixelFormat--}
```
public final int getPixelFormat()
```


Haalt het formaat van de kleurgegevens voor elke pixel in de afbeelding op.

**Returns:**
int - het formaat van de kleurgegevens voor elke pixel in de afbeelding.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Haalt een waarde op die aangeeft of een kloof tussen de laatste taak en de voettekst moet worden verkleind.

**Returns:**
boolean - een waarde die aangeeft of de ruimte tussen de laatste taak en de voettekst moet worden verkleind.
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


Haalt het type compressie op dat moet worden toegepast bij het opslaan van gegenereerde afbeeldingen in het TIFF-formaat.

--------------------

Heeft alleen effect bij het opslaan naar TIFF. De standaardwaarde is `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-)).

**Returns:**
int - het type compressie dat moet worden toegepast bij het opslaan van gegenereerde afbeeldingen in het TIFF-formaat.
### getVerticalResolution() {#getVerticalResolution--}
```
public final float getVerticalResolution()
```


Haalt de verticale resolutie op in dpi.

**Returns:**
float - de verticale resolutie in dpi.
### setHorizontalResolution(float value) {#setHorizontalResolution-float-}
```
public final void setHorizontalResolution(float value)
```


Stelt de horizontale resolutie in in dpi.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | float | de horizontale resolutie in dpi. |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


Stelt een JPEG-kwaliteit in. Het toegestane waardebereik is 0..100.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een JPEG-kwaliteit. |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Stelt een door de gebruiker gedefinieerde callback in die wordt gebruikt om een output‑stream voor elke gerenderde pagina te verkrijgen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | een door de gebruiker gedefinieerde callback die wordt gebruikt om een output-stream voor elke gerenderde pagina te verkrijgen. |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


Stelt een lijst met paginanummers in die moeten worden opgeslagen bij het opslaan van de projectlay-out naar afzonderlijke bestanden.

--------------------

Alle pagina's worden opgeslagen als deze lijst leeg is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.List&lt;java.lang.Integer&gt; | een lijst met paginanummers om op te slaan bij het opslaan van de projectlay-out naar afzonderlijke bestanden. |

### setPixelFormat(int value) {#setPixelFormat-int-}
```
public final void setPixelFormat(int value)
```


Stelt het formaat van de kleurgegevens voor elke pixel in de afbeelding in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | het formaat van de kleurgegevens voor elke pixel in de afbeelding. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Stelt een waarde in die aangeeft of de ruimte tussen de laatste taak en de voettekst moet worden verkleind.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of een ruimte tussen de laatste taak en de voettekst moet worden verkleind. |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


Stelt het type compressie in dat moet worden toegepast bij het opslaan van gegenereerde afbeeldingen in het TIFF-formaat.

--------------------

Heeft alleen effect bij het opslaan naar TIFF. De standaardwaarde is `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-)).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | het type compressie dat moet worden toegepast bij het opslaan van gegenereerde afbeeldingen in het TIFF-formaat. |

### setVerticalResolution(float value) {#setVerticalResolution-float-}
```
public final void setVerticalResolution(float value)
```


Stelt de verticale resolutie in in dpi.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | float | de verticale resolutie in dpi. |

