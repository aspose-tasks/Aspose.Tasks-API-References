---
title: "HtmlSaveOptions"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Staat toe extra opties op te geven bij het renderen van projectpagina's naar HTML."
type: docs
weight: 132
url: /nl/java/com.aspose.tasks/htmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class HtmlSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Staat toe extra opties op te geven bij het renderen van projectpagina's naar HTML.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [HtmlSaveOptions()](#HtmlSaveOptions--) | Initialiseert een nieuw exemplaar van de [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCssSavingCallback()](#getCssSavingCallback--) | Haalt de callback op die wordt aangeroepen om een bron te maken om CSS op te slaan. |
| [getCssStylePrefix()](#getCssStylePrefix--) | Haalt CSS-stijlprefix op. |
| [getExportCss()](#getExportCss--) | Haalt de manier op waarop CSS wordt geëxporteerd. |
| [getExportFonts()](#getExportFonts--) | Haalt de manier op waarop lettertypen worden geëxporteerd. |
| [getExportImages()](#getExportImages--) | Haalt de manier op waarop afbeeldingen worden geëxporteerd. |
| [getFontFaceTypes()](#getFontFaceTypes--) | Haalt de lettertype‑typen op. |
| [getFontSavingCallback()](#getFontSavingCallback--) | Haalt de callback op die wordt aangeroepen om een bron te maken om lettertype op te slaan. |
| [getFontSettings()](#getFontSettings--) | Specificeert lettertype‑instellingen die worden gebruikt bij het renderen van de projectweergave. |
| [getImageSavingCallback()](#getImageSavingCallback--) | Haalt de callback op die wordt aangeroepen om een bron te maken om lettertype op te slaan. |
| [getIncludeProjectNameInPageHeader()](#getIncludeProjectNameInPageHeader--) | Haalt een waarde op die aangeeft of de projectnaam moet worden opgenomen in de HTML-pagina‑header. |
| [getIncludeProjectNameInTitle()](#getIncludeProjectNameInTitle--) | Haalt een waarde op die aangeeft of de projectnaam moet worden opgenomen in de HTML‑titel. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Haalt een door de gebruiker gedefinieerde callback op die wordt gebruikt om een uitvoerstroom voor elke gerenderde pagina te verkrijgen. |
| [getPages()](#getPages--) | Haalt een lijst met paginanummers op die moeten worden opgeslagen bij het renderen van de projectlay-out. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Haalt een waarde op die aangeeft of een kloof tussen de laatste taak en de voettekst moet worden verkleind. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Haalt een waarde op die aangeeft of een verloopkwast moet worden gebruikt bij het renderen van de projectlay-out. |
| [setCssSavingCallback(ICssSavingCallback value)](#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-) | Stelt de callback in die wordt aangeroepen om een bron te maken om CSS op te slaan. |
| [setCssStylePrefix(String value)](#setCssStylePrefix-java.lang.String-) | Stelt CSS-stijlprefix in. |
| [setExportCss(int value)](#setExportCss-int-) | Stelt de manier in waarop CSS wordt geëxporteerd. |
| [setExportFonts(int value)](#setExportFonts-int-) | Stelt de manier in waarop lettertypen worden geëxporteerd. |
| [setExportImages(int value)](#setExportImages-int-) | Stelt de manier in waarop afbeeldingen worden geëxporteerd. |
| [setFontFaceTypes(int value)](#setFontFaceTypes-int-) | Stelt de lettertype‑soorten in. |
| [setFontSavingCallback(IFontSavingCallback value)](#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-) | Stelt de callback in die wordt aangeroepen om een bron te maken om het lettertype op te slaan. |
| [setImageSavingCallback(IImageSavingCallback value)](#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-) | Stelt de callback in die wordt aangeroepen om een bron te maken om het lettertype op te slaan. |
| [setIncludeProjectNameInPageHeader(boolean value)](#setIncludeProjectNameInPageHeader-boolean-) | Stelt een waarde in die aangeeft of de projectnaam in de HTML-paginaheader moet worden opgenomen. |
| [setIncludeProjectNameInTitle(boolean value)](#setIncludeProjectNameInTitle-boolean-) | Stelt een waarde in die aangeeft of de projectnaam in de HTML-titel moet worden opgenomen. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Stelt een door de gebruiker gedefinieerde callback in die wordt gebruikt om een output‑stream voor elke gerenderde pagina te verkrijgen. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Stelt een lijst met paginanummers in die moet worden opgeslagen bij het renderen van de projectlay-out. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Stelt een waarde in die aangeeft of de ruimte tussen de laatste taak en de voettekst moet worden verkleind. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Stelt een waarde in die aangeeft of een gradient‑kwast moet worden gebruikt bij het renderen van de projectlay-out. |
### HtmlSaveOptions() {#HtmlSaveOptions--}
```
public HtmlSaveOptions()
```


Initialiseert een nieuw exemplaar van de [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions) klasse.

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
### getCssSavingCallback() {#getCssSavingCallback--}
```
public final ICssSavingCallback getCssSavingCallback()
```


Haalt de callback op die wordt aangeroepen om een bron te maken om CSS op te slaan.

**Returns:**
[ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) - the callback that is called to create resource to store CSS.
### getCssStylePrefix() {#getCssStylePrefix--}
```
public final String getCssStylePrefix()
```


Haalt CSS-stijlprefix op.

**Returns:**
java.lang.String - CSS‑stijlvoorvoegsel.
### getExportCss() {#getExportCss--}
```
public final int getExportCss()
```


Haalt de manier op waarop CSS wordt geëxporteerd.

**Returns:**
int - de manier waarop CSS wordt geëxporteerd.
### getExportFonts() {#getExportFonts--}
```
public final int getExportFonts()
```


Haalt de manier op waarop lettertypen worden geëxporteerd.

**Returns:**
int - de manier waarop lettertypen worden geëxporteerd.
### getExportImages() {#getExportImages--}
```
public final int getExportImages()
```


Haalt de manier op waarop afbeeldingen worden geëxporteerd.

**Returns:**
int - de manier waarop afbeeldingen worden geëxporteerd.
### getFontFaceTypes() {#getFontFaceTypes--}
```
public final int getFontFaceTypes()
```


Haalt de lettertype‑typen op.

Waarde: De lettertype‑soorten.

**Returns:**
int - de lettertype‑soorten.
### getFontSavingCallback() {#getFontSavingCallback--}
```
public final IFontSavingCallback getFontSavingCallback()
```


Haalt de callback op die wordt aangeroepen om een bron te maken om lettertype op te slaan.

**Returns:**
[IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) - the callback that is called to create resource to store font.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Specificeert lettertype‑instellingen die worden gebruikt bij het renderen van de projectweergave.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getImageSavingCallback() {#getImageSavingCallback--}
```
public final IImageSavingCallback getImageSavingCallback()
```


Haalt de callback op die wordt aangeroepen om een bron te maken om lettertype op te slaan.

**Returns:**
[IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) - the callback that is called to create resource to store font.
### getIncludeProjectNameInPageHeader() {#getIncludeProjectNameInPageHeader--}
```
public final boolean getIncludeProjectNameInPageHeader()
```


Haalt een waarde op die aangeeft of de projectnaam moet worden opgenomen in de HTML-pagina‑header.

**Returns:**
boolean - een waarde die aangeeft of de projectnaam in de HTML-paginaheader moet worden opgenomen.
### getIncludeProjectNameInTitle() {#getIncludeProjectNameInTitle--}
```
public final boolean getIncludeProjectNameInTitle()
```


Haalt een waarde op die aangeeft of de projectnaam moet worden opgenomen in de HTML‑titel.

**Returns:**
boolean - een waarde die aangeeft of de projectnaam in de HTML-titel moet worden opgenomen.
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


Haalt een lijst met paginanummers op die moeten worden opgeslagen bij het renderen van de projectlay-out.

--------------------

Alle projectpagina's worden opgeslagen als deze lijst leeg is.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - een lijst met paginanummers die moeten worden opgeslagen bij het renderen van de projectlay-out.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Haalt een waarde op die aangeeft of een kloof tussen de laatste taak en de voettekst moet worden verkleind.

**Returns:**
boolean - een waarde die aangeeft of de ruimte tussen de laatste taak en de voettekst moet worden verkleind.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Haalt een waarde op die aangeeft of een verloopkwast moet worden gebruikt bij het renderen van de projectlay-out.

--------------------

Het gebruik van een gradient‑kwast wordt momenteel niet ondersteund bij het renderen naar HTML.

**Returns:**
boolean - een waarde die aangeeft of een gradient‑kwast moet worden gebruikt bij het renderen van de projectlay‑out.
### setCssSavingCallback(ICssSavingCallback value) {#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-}
```
public final void setCssSavingCallback(ICssSavingCallback value)
```


Stelt de callback in die wordt aangeroepen om een bron te maken om CSS op te slaan.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) | de callback die wordt aangeroepen om een bron te maken om CSS op te slaan. |

### setCssStylePrefix(String value) {#setCssStylePrefix-java.lang.String-}
```
public final void setCssStylePrefix(String value)
```


Stelt CSS-stijlprefix in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | CSS‑stijlvoorvoegsel. |

### setExportCss(int value) {#setExportCss-int-}
```
public final void setExportCss(int value)
```


Stelt de manier in waarop CSS wordt geëxporteerd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de manier waarop CSS worden geëxporteerd. |

### setExportFonts(int value) {#setExportFonts-int-}
```
public final void setExportFonts(int value)
```


Stelt de manier in waarop lettertypen worden geëxporteerd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de manier waarop lettertypen worden geëxporteerd. |

### setExportImages(int value) {#setExportImages-int-}
```
public final void setExportImages(int value)
```


Stelt de manier in waarop afbeeldingen worden geëxporteerd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de manier waarop afbeeldingen worden geëxporteerd. |

### setFontFaceTypes(int value) {#setFontFaceTypes-int-}
```
public final void setFontFaceTypes(int value)
```


Stelt de lettertype‑soorten in.

Waarde: De lettertype‑soorten.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de lettertype-typen. |

### setFontSavingCallback(IFontSavingCallback value) {#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-}
```
public final void setFontSavingCallback(IFontSavingCallback value)
```


Stelt de callback in die wordt aangeroepen om een bron te maken om het lettertype op te slaan.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) | de callback die wordt aangeroepen om een bron te maken om het lettertype op te slaan. |

### setImageSavingCallback(IImageSavingCallback value) {#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-}
```
public final void setImageSavingCallback(IImageSavingCallback value)
```


Stelt de callback in die wordt aangeroepen om een bron te maken om het lettertype op te slaan.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) | de callback die wordt aangeroepen om een bron te maken om het lettertype op te slaan. |

### setIncludeProjectNameInPageHeader(boolean value) {#setIncludeProjectNameInPageHeader-boolean-}
```
public final void setIncludeProjectNameInPageHeader(boolean value)
```


Stelt een waarde in die aangeeft of de projectnaam in de HTML-paginaheader moet worden opgenomen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of de projectnaam moet worden opgenomen in de HTML-pagina-header. |

### setIncludeProjectNameInTitle(boolean value) {#setIncludeProjectNameInTitle-boolean-}
```
public final void setIncludeProjectNameInTitle(boolean value)
```


Stelt een waarde in die aangeeft of de projectnaam in de HTML-titel moet worden opgenomen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of de projectnaam moet worden opgenomen in de HTML-titel. |

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


Stelt een lijst met paginanummers in die moet worden opgeslagen bij het renderen van de projectlay-out.

--------------------

Alle projectpagina's worden opgeslagen als deze lijst leeg is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.List&lt;java.lang.Integer&gt; | een lijst met paginanummers die moeten worden opgeslagen bij het renderen van de projectlay-out. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Stelt een waarde in die aangeeft of de ruimte tussen de laatste taak en de voettekst moet worden verkleind.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of een ruimte tussen de laatste taak en de voettekst moet worden verkleind. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Stelt een waarde in die aangeeft of een gradient‑kwast moet worden gebruikt bij het renderen van de projectlay-out.

--------------------

Het gebruik van een gradient‑kwast wordt momenteel niet ondersteund bij het renderen naar HTML.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of een gradient-kwast moet worden gebruikt bij het renderen van de projectlay-out. |

