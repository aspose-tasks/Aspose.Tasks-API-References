---
title: "HtmlSaveOptions"
second_title: "Aspose.Tasks for Java API-referens"
description: "Tillåter att ange ytterligare alternativ när projektssidor renderas till HTML."
type: docs
weight: 132
url: /sv/java/com.aspose.tasks/htmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class HtmlSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Tillåter att ange ytterligare alternativ när projektssidor renderas till HTML.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [HtmlSaveOptions()](#HtmlSaveOptions--) | Initierar en ny instans av klassen [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCssSavingCallback()](#getCssSavingCallback--) | Hämtar återuppringningen som anropas för att skapa en resurs för att lagra CSS. |
| [getCssStylePrefix()](#getCssStylePrefix--) | Hämtar CSS-stilprefix. |
| [getExportCss()](#getExportCss--) | Hämtar hur CSS exporteras. |
| [getExportFonts()](#getExportFonts--) | Hämtar hur typsnitt exporteras. |
| [getExportImages()](#getExportImages--) | Hämtar hur bilder exporteras. |
| [getFontFaceTypes()](#getFontFaceTypes--) | Hämtar typsnittstyperna. |
| [getFontSavingCallback()](#getFontSavingCallback--) | Hämtar återuppringningen som anropas för att skapa en resurs för att lagra typsnitt. |
| [getFontSettings()](#getFontSettings--) | Anger teckensnittsinställningar som används när projektets vy renderas. |
| [getImageSavingCallback()](#getImageSavingCallback--) | Hämtar återuppringningen som anropas för att skapa en resurs för att lagra typsnitt. |
| [getIncludeProjectNameInPageHeader()](#getIncludeProjectNameInPageHeader--) | Hämtar ett värde som indikerar om projektnamnet ska inkluderas i HTML-sidhuvudet. |
| [getIncludeProjectNameInTitle()](#getIncludeProjectNameInTitle--) | Hämtar ett värde som indikerar om projektnamnet ska inkluderas i HTML-titeln. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Hämtar en användardefinierad återuppringning som används för att få en utström för varje renderad sida. |
| [getPages()](#getPages--) | Hämtar en lista med sidnummer att spara när projektlayout renderas. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Hämtar ett värde som indikerar om ett gap mellan sista uppgiften och sidfoten ska minskas. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Hämtar ett värde som indikerar om en gradientpensel ska användas när projektlayout renderas. |
| [setCssSavingCallback(ICssSavingCallback value)](#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-) | Ställer in återuppringningen som anropas för att skapa en resurs för att lagra CSS. |
| [setCssStylePrefix(String value)](#setCssStylePrefix-java.lang.String-) | Ställer in CSS-stilprefix. |
| [setExportCss(int value)](#setExportCss-int-) | Ställer in hur CSS exporteras. |
| [setExportFonts(int value)](#setExportFonts-int-) | Ställer in hur teckensnitt exporteras. |
| [setExportImages(int value)](#setExportImages-int-) | Ställer in hur bilder exporteras. |
| [setFontFaceTypes(int value)](#setFontFaceTypes-int-) | Ställer in teckensnittstyperna. |
| [setFontSavingCallback(IFontSavingCallback value)](#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-) | Ställer in återanropet som anropas för att skapa en resurs för att lagra teckensnitt. |
| [setImageSavingCallback(IImageSavingCallback value)](#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-) | Ställer in återanropet som anropas för att skapa en resurs för att lagra teckensnitt. |
| [setIncludeProjectNameInPageHeader(boolean value)](#setIncludeProjectNameInPageHeader-boolean-) | Ställer in ett värde som anger om projektnamnet ska inkluderas i HTML-sidhuvudet. |
| [setIncludeProjectNameInTitle(boolean value)](#setIncludeProjectNameInTitle-boolean-) | Ställer in ett värde som anger om projektnamnet ska inkluderas i HTML-titeln. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Ställer in ett användardefinierat återanrop som används för att hämta en utdataström för varje renderad sida. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Ställer in en lista med sidnummer att spara när projektlayouten renderas. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Ställer in ett värde som anger om ett mellanrum mellan sista uppgiften och sidfoten ska minskas. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Ställer in ett värde som anger om en gradientpensel ska användas när projektlayouten renderas. |
### HtmlSaveOptions() {#HtmlSaveOptions--}
```
public HtmlSaveOptions()
```


Initierar en ny instans av klassen [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions).

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
### getCssSavingCallback() {#getCssSavingCallback--}
```
public final ICssSavingCallback getCssSavingCallback()
```


Hämtar återuppringningen som anropas för att skapa en resurs för att lagra CSS.

**Returns:**
[ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) - the callback that is called to create resource to store CSS.
### getCssStylePrefix() {#getCssStylePrefix--}
```
public final String getCssStylePrefix()
```


Hämtar CSS-stilprefix.

**Returns:**
java.lang.String - CSS-stilprefix.
### getExportCss() {#getExportCss--}
```
public final int getExportCss()
```


Hämtar hur CSS exporteras.

**Returns:**
int - hur CSS exporteras.
### getExportFonts() {#getExportFonts--}
```
public final int getExportFonts()
```


Hämtar hur typsnitt exporteras.

**Returns:**
int - hur teckensnitt exporteras.
### getExportImages() {#getExportImages--}
```
public final int getExportImages()
```


Hämtar hur bilder exporteras.

**Returns:**
int - hur bilder exporteras.
### getFontFaceTypes() {#getFontFaceTypes--}
```
public final int getFontFaceTypes()
```


Hämtar typsnittstyperna.

Värde: Teckensnittstyperna.

**Returns:**
int - teckensnittstyperna.
### getFontSavingCallback() {#getFontSavingCallback--}
```
public final IFontSavingCallback getFontSavingCallback()
```


Hämtar återuppringningen som anropas för att skapa en resurs för att lagra typsnitt.

**Returns:**
[IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) - the callback that is called to create resource to store font.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Anger teckensnittsinställningar som används när projektets vy renderas.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getImageSavingCallback() {#getImageSavingCallback--}
```
public final IImageSavingCallback getImageSavingCallback()
```


Hämtar återuppringningen som anropas för att skapa en resurs för att lagra typsnitt.

**Returns:**
[IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) - the callback that is called to create resource to store font.
### getIncludeProjectNameInPageHeader() {#getIncludeProjectNameInPageHeader--}
```
public final boolean getIncludeProjectNameInPageHeader()
```


Hämtar ett värde som indikerar om projektnamnet ska inkluderas i HTML-sidhuvudet.

**Returns:**
boolean - ett värde som anger om projektnamnet ska inkluderas i HTML-sidhuvudet.
### getIncludeProjectNameInTitle() {#getIncludeProjectNameInTitle--}
```
public final boolean getIncludeProjectNameInTitle()
```


Hämtar ett värde som indikerar om projektnamnet ska inkluderas i HTML-titeln.

**Returns:**
boolean - ett värde som anger om projektnamnet ska inkluderas i HTML-titeln.
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


Hämtar en lista med sidnummer att spara när projektlayout renderas.

--------------------

Alla projektsidor kommer att sparas om denna lista är tom.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - en lista med sidnummer att spara när projektlayouten renderas.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Hämtar ett värde som indikerar om ett gap mellan sista uppgiften och sidfoten ska minskas.

**Returns:**
boolean - ett värde som anger om ett mellanrum mellan sista uppgiften och sidfoten ska minskas.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Hämtar ett värde som indikerar om en gradientpensel ska användas när projektlayout renderas.

--------------------

För närvarande stöds inte användning av gradientpensel vid rendering till HTML.

**Returns:**
boolean - ett värde som anger om en gradientpensel ska användas när projektlayouten renderas.
### setCssSavingCallback(ICssSavingCallback value) {#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-}
```
public final void setCssSavingCallback(ICssSavingCallback value)
```


Ställer in återuppringningen som anropas för att skapa en resurs för att lagra CSS.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) | återanropet som anropas för att skapa en resurs för att lagra CSS. |

### setCssStylePrefix(String value) {#setCssStylePrefix-java.lang.String-}
```
public final void setCssStylePrefix(String value)
```


Ställer in CSS-stilprefix.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | CSS-stilprefix. |

### setExportCss(int value) {#setExportCss-int-}
```
public final void setExportCss(int value)
```


Ställer in hur CSS exporteras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | sättet CSS exporteras. |

### setExportFonts(int value) {#setExportFonts-int-}
```
public final void setExportFonts(int value)
```


Ställer in hur teckensnitt exporteras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | sättet teckensnitt exporteras. |

### setExportImages(int value) {#setExportImages-int-}
```
public final void setExportImages(int value)
```


Ställer in hur bilder exporteras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | sättet bilder exporteras. |

### setFontFaceTypes(int value) {#setFontFaceTypes-int-}
```
public final void setFontFaceTypes(int value)
```


Ställer in teckensnittstyperna.

Värde: Teckensnittstyperna.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | typer av teckensnitt. |

### setFontSavingCallback(IFontSavingCallback value) {#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-}
```
public final void setFontSavingCallback(IFontSavingCallback value)
```


Ställer in återanropet som anropas för att skapa en resurs för att lagra teckensnitt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) | återanropet som anropas för att skapa en resurs för att lagra teckensnitt. |

### setImageSavingCallback(IImageSavingCallback value) {#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-}
```
public final void setImageSavingCallback(IImageSavingCallback value)
```


Ställer in återanropet som anropas för att skapa en resurs för att lagra teckensnitt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) | återanropet som anropas för att skapa en resurs för att lagra teckensnitt. |

### setIncludeProjectNameInPageHeader(boolean value) {#setIncludeProjectNameInPageHeader-boolean-}
```
public final void setIncludeProjectNameInPageHeader(boolean value)
```


Ställer in ett värde som anger om projektnamnet ska inkluderas i HTML-sidhuvudet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som anger om projektnamnet ska inkluderas i HTML-sidhuvudet. |

### setIncludeProjectNameInTitle(boolean value) {#setIncludeProjectNameInTitle-boolean-}
```
public final void setIncludeProjectNameInTitle(boolean value)
```


Ställer in ett värde som anger om projektnamnet ska inkluderas i HTML-titeln.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som anger om projektnamnet ska inkluderas i HTML-titeln. |

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


Ställer in en lista med sidnummer att spara när projektlayouten renderas.

--------------------

Alla projektsidor kommer att sparas om denna lista är tom.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.List&lt;java.lang.Integer&gt; | en lista med sidnummer att spara när projektlayout renderas. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Ställer in ett värde som anger om ett mellanrum mellan sista uppgiften och sidfoten ska minskas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som anger om ett mellanrum mellan sista uppgift och sidfot ska minskas. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Ställer in ett värde som anger om en gradientpensel ska användas när projektlayouten renderas.

--------------------

För närvarande stöds inte användning av gradientpensel vid rendering till HTML.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som anger om en gradientpensel ska användas när projektlayout renderas. |

