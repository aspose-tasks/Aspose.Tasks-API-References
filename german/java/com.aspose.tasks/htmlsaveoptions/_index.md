---
title: "HtmlSaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Ermöglicht das Angeben zusätzlicher Optionen beim Rendern von Projektseiten zu HTML."
type: docs
weight: 132
url: /de/java/com.aspose.tasks/htmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class HtmlSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Ermöglicht das Angeben zusätzlicher Optionen beim Rendern von Projektseiten zu HTML.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [HtmlSaveOptions()](#HtmlSaveOptions--) | Initialisiert eine neue Instanz der Klasse [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCssSavingCallback()](#getCssSavingCallback--) | Liefert den Callback, der aufgerufen wird, um eine Ressource zum Speichern von CSS zu erstellen. |
| [getCssStylePrefix()](#getCssStylePrefix--) | Liefert das CSS-Stilpräfix. |
| [getExportCss()](#getExportCss--) | Liefert die Art und Weise, wie CSS exportiert werden. |
| [getExportFonts()](#getExportFonts--) | Liefert die Art und Weise, wie Schriftarten exportiert werden. |
| [getExportImages()](#getExportImages--) | Liefert die Art und Weise, wie Bilder exportiert werden. |
| [getFontFaceTypes()](#getFontFaceTypes--) | Liefert die Schriftart-Typen. |
| [getFontSavingCallback()](#getFontSavingCallback--) | Liefert den Callback, der aufgerufen wird, um eine Ressource zum Speichern von Schriftarten zu erstellen. |
| [getFontSettings()](#getFontSettings--) | Gibt die Schriftarteinstellungen an, die beim Rendern der Projektansicht verwendet werden. |
| [getImageSavingCallback()](#getImageSavingCallback--) | Liefert den Callback, der aufgerufen wird, um eine Ressource zum Speichern von Schriftarten zu erstellen. |
| [getIncludeProjectNameInPageHeader()](#getIncludeProjectNameInPageHeader--) | Liefert einen Wert, der angibt, ob der Projektname in die HTML-Seitenkopfzeile aufgenommen werden soll. |
| [getIncludeProjectNameInTitle()](#getIncludeProjectNameInTitle--) | Liefert einen Wert, der angibt, ob der Projektname im HTML-Titel enthalten sein soll. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Liefert einen benutzerdefinierten Callback, der verwendet wird, um einen Ausgabestream für jede gerenderte Seite zu erhalten. |
| [getPages()](#getPages--) | Liefert eine Liste von Seitenzahlen, die beim Rendern des Projektlayouts gespeichert werden sollen. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Liefert einen Wert, der angibt, ob ein Abstand zwischen der letzten Aufgabe und der Fußzeile reduziert werden muss. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Liefert einen Wert, der angibt, ob beim Rendern des Projektlayouts ein Farbverlaufspinsel verwendet werden soll. |
| [setCssSavingCallback(ICssSavingCallback value)](#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-) | Setzt den Callback, der aufgerufen wird, um eine Ressource zum Speichern von CSS zu erstellen. |
| [setCssStylePrefix(String value)](#setCssStylePrefix-java.lang.String-) | Legt das CSS-Stilpräfix fest. |
| [setExportCss(int value)](#setExportCss-int-) | Legt fest, wie CSS exportiert werden. |
| [setExportFonts(int value)](#setExportFonts-int-) | Legt fest, wie Schriftarten exportiert werden. |
| [setExportImages(int value)](#setExportImages-int-) | Legt fest, wie Bilder exportiert werden. |
| [setFontFaceTypes(int value)](#setFontFaceTypes-int-) | Legt die Schriftart-Typen fest. |
| [setFontSavingCallback(IFontSavingCallback value)](#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-) | Legt den Rückruf fest, der aufgerufen wird, um eine Ressource zum Speichern der Schrift zu erstellen. |
| [setImageSavingCallback(IImageSavingCallback value)](#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-) | Legt den Rückruf fest, der aufgerufen wird, um eine Ressource zum Speichern der Schrift zu erstellen. |
| [setIncludeProjectNameInPageHeader(boolean value)](#setIncludeProjectNameInPageHeader-boolean-) | Legt einen Wert fest, der angibt, ob der Projektname in die HTML-Seitenkopfzeile aufgenommen werden soll. |
| [setIncludeProjectNameInTitle(boolean value)](#setIncludeProjectNameInTitle-boolean-) | Legt einen Wert fest, der angibt, ob der Projektname im HTML-Titel enthalten sein soll. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Legt einen benutzerdefinierten Rückruf fest, der verwendet wird, um einen Ausgabestream für jede gerenderte Seite zu erhalten. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Legt eine Liste von Seitenzahlen fest, die beim Rendern des Projektlayouts gespeichert werden sollen. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Legt einen Wert fest, der angibt, ob ein Abstand zwischen der letzten Aufgabe und der Fußzeile reduziert werden muss. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Legt einen Wert fest, der angibt, ob beim Rendern des Projektlayouts ein Farbverlaufspinsel verwendet werden soll. |
### HtmlSaveOptions() {#HtmlSaveOptions--}
```
public HtmlSaveOptions()
```


Initialisiert eine neue Instanz der Klasse [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions).

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public final void copyOutputPropertiesFrom(SaveOptions source)
```


Für den internen Gebrauch reserviert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public SaveOptions deepClone()
```


Für den internen Gebrauch reserviert.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getCssSavingCallback() {#getCssSavingCallback--}
```
public final ICssSavingCallback getCssSavingCallback()
```


Liefert den Callback, der aufgerufen wird, um eine Ressource zum Speichern von CSS zu erstellen.

**Returns:**
[ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) - the callback that is called to create resource to store CSS.
### getCssStylePrefix() {#getCssStylePrefix--}
```
public final String getCssStylePrefix()
```


Liefert das CSS-Stilpräfix.

**Returns:**
java.lang.String - CSS-Stilpräfix.
### getExportCss() {#getExportCss--}
```
public final int getExportCss()
```


Liefert die Art und Weise, wie CSS exportiert werden.

**Returns:**
int - die Art, wie CSS exportiert werden.
### getExportFonts() {#getExportFonts--}
```
public final int getExportFonts()
```


Liefert die Art und Weise, wie Schriftarten exportiert werden.

**Returns:**
int - die Art, wie Schriftarten exportiert werden.
### getExportImages() {#getExportImages--}
```
public final int getExportImages()
```


Liefert die Art und Weise, wie Bilder exportiert werden.

**Returns:**
int - die Art, wie Bilder exportiert werden.
### getFontFaceTypes() {#getFontFaceTypes--}
```
public final int getFontFaceTypes()
```


Liefert die Schriftart-Typen.

Wert: Die Schriftart-Typen.

**Returns:**
int - die Schriftart-Typen.
### getFontSavingCallback() {#getFontSavingCallback--}
```
public final IFontSavingCallback getFontSavingCallback()
```


Liefert den Callback, der aufgerufen wird, um eine Ressource zum Speichern von Schriftarten zu erstellen.

**Returns:**
[IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) - the callback that is called to create resource to store font.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Gibt die Schriftarteinstellungen an, die beim Rendern der Projektansicht verwendet werden.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getImageSavingCallback() {#getImageSavingCallback--}
```
public final IImageSavingCallback getImageSavingCallback()
```


Liefert den Callback, der aufgerufen wird, um eine Ressource zum Speichern von Schriftarten zu erstellen.

**Returns:**
[IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) - the callback that is called to create resource to store font.
### getIncludeProjectNameInPageHeader() {#getIncludeProjectNameInPageHeader--}
```
public final boolean getIncludeProjectNameInPageHeader()
```


Liefert einen Wert, der angibt, ob der Projektname in die HTML-Seitenkopfzeile aufgenommen werden soll.

**Returns:**
boolean - ein Wert, der angibt, ob der Projektname in die HTML-Seitenkopfzeile aufgenommen werden soll.
### getIncludeProjectNameInTitle() {#getIncludeProjectNameInTitle--}
```
public final boolean getIncludeProjectNameInTitle()
```


Liefert einen Wert, der angibt, ob der Projektname im HTML-Titel enthalten sein soll.

**Returns:**
boolean - ein Wert, der angibt, ob der Projektname im HTML-Titel enthalten sein soll.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Liefert einen benutzerdefinierten Callback, der verwendet wird, um einen Ausgabestream für jede gerenderte Seite zu erhalten.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


Liefert eine Liste von Seitenzahlen, die beim Rendern des Projektlayouts gespeichert werden sollen.

--------------------

Alle Projektseiten werden gespeichert, wenn diese Liste leer ist.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - eine Liste von Seitenzahlen, die beim Rendern des Projektlayouts gespeichert werden sollen.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Liefert einen Wert, der angibt, ob ein Abstand zwischen der letzten Aufgabe und der Fußzeile reduziert werden muss.

**Returns:**
boolean - ein Wert, der angibt, ob ein Abstand zwischen der letzten Aufgabe und der Fußzeile reduziert werden muss.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Liefert einen Wert, der angibt, ob beim Rendern des Projektlayouts ein Farbverlaufspinsel verwendet werden soll.

--------------------

Derzeit wird die Verwendung eines Farbverlaufspinsels beim Rendern nach HTML nicht unterstützt.

**Returns:**
boolean - ein Wert, der angibt, ob beim Rendern des Projektlayouts ein Farbverlaufspinsel verwendet werden soll.
### setCssSavingCallback(ICssSavingCallback value) {#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-}
```
public final void setCssSavingCallback(ICssSavingCallback value)
```


Setzt den Callback, der aufgerufen wird, um eine Ressource zum Speichern von CSS zu erstellen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) | Der Callback, der aufgerufen wird, um eine Ressource zum Speichern von CSS zu erstellen. |

### setCssStylePrefix(String value) {#setCssStylePrefix-java.lang.String-}
```
public final void setCssStylePrefix(String value)
```


Legt das CSS-Stilpräfix fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | CSS-Stilpräfix. |

### setExportCss(int value) {#setExportCss-int-}
```
public final void setExportCss(int value)
```


Legt fest, wie CSS exportiert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | Die Art und Weise, wie CSS exportiert werden. |

### setExportFonts(int value) {#setExportFonts-int-}
```
public final void setExportFonts(int value)
```


Legt fest, wie Schriftarten exportiert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | Die Art und Weise, wie Schriftarten exportiert werden. |

### setExportImages(int value) {#setExportImages-int-}
```
public final void setExportImages(int value)
```


Legt fest, wie Bilder exportiert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | Die Art und Weise, wie Bilder exportiert werden. |

### setFontFaceTypes(int value) {#setFontFaceTypes-int-}
```
public final void setFontFaceTypes(int value)
```


Legt die Schriftart-Typen fest.

Wert: Die Schriftart-Typen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | Die Schriftart-Typen. |

### setFontSavingCallback(IFontSavingCallback value) {#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-}
```
public final void setFontSavingCallback(IFontSavingCallback value)
```


Legt den Rückruf fest, der aufgerufen wird, um eine Ressource zum Speichern der Schrift zu erstellen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) | Der Callback, der aufgerufen wird, um eine Ressource zum Speichern von Schriftarten zu erstellen. |

### setImageSavingCallback(IImageSavingCallback value) {#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-}
```
public final void setImageSavingCallback(IImageSavingCallback value)
```


Legt den Rückruf fest, der aufgerufen wird, um eine Ressource zum Speichern der Schrift zu erstellen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) | Der Callback, der aufgerufen wird, um eine Ressource zum Speichern von Schriftarten zu erstellen. |

### setIncludeProjectNameInPageHeader(boolean value) {#setIncludeProjectNameInPageHeader-boolean-}
```
public final void setIncludeProjectNameInPageHeader(boolean value)
```


Legt einen Wert fest, der angibt, ob der Projektname in die HTML-Seitenkopfzeile aufgenommen werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | Ein Wert, der angibt, ob der Projektname in die HTML-Seitenkopfzeile aufgenommen werden soll. |

### setIncludeProjectNameInTitle(boolean value) {#setIncludeProjectNameInTitle-boolean-}
```
public final void setIncludeProjectNameInTitle(boolean value)
```


Legt einen Wert fest, der angibt, ob der Projektname im HTML-Titel enthalten sein soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | Ein Wert, der angibt, ob der Projektname im HTML-Titel enthalten sein soll. |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Legt einen benutzerdefinierten Rückruf fest, der verwendet wird, um einen Ausgabestream für jede gerenderte Seite zu erhalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | Ein benutzerdefinierter Callback, der verwendet wird, um einen Ausgabestream für jede gerenderte Seite zu erhalten. |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


Legt eine Liste von Seitenzahlen fest, die beim Rendern des Projektlayouts gespeichert werden sollen.

--------------------

Alle Projektseiten werden gespeichert, wenn diese Liste leer ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.List&lt;java.lang.Integer&gt; | Eine Liste von Seitenzahlen, die beim Rendern des Projektlayouts gespeichert werden sollen. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Legt einen Wert fest, der angibt, ob ein Abstand zwischen der letzten Aufgabe und der Fußzeile reduziert werden muss.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | Ein Wert, der angibt, ob ein Abstand zwischen der letzten Aufgabe und der Fußzeile reduziert werden muss. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Legt einen Wert fest, der angibt, ob beim Rendern des Projektlayouts ein Farbverlaufspinsel verwendet werden soll.

--------------------

Derzeit wird die Verwendung eines Farbverlaufspinsels beim Rendern nach HTML nicht unterstützt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | Ein Wert, der angibt, ob beim Rendern des Projektlayouts ein Farbverlaufspinsel verwendet werden soll. |

