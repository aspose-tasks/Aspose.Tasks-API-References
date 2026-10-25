---
title: "HtmlSaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Consente di specificare opzioni aggiuntive durante il rendering delle pagine del progetto in HTML."
type: docs
weight: 132
url: /it/java/com.aspose.tasks/htmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class HtmlSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Consente di specificare opzioni aggiuntive durante il rendering delle pagine del progetto in HTML.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [HtmlSaveOptions()](#HtmlSaveOptions--) | Inizializza una nuova istanza della classe [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCssSavingCallback()](#getCssSavingCallback--) | Ottiene il callback che viene chiamato per creare la risorsa per memorizzare il CSS. |
| [getCssStylePrefix()](#getCssStylePrefix--) | Ottiene il prefisso dello stile CSS. |
| [getExportCss()](#getExportCss--) | Ottiene il modo in cui il CSS viene esportato. |
| [getExportFonts()](#getExportFonts--) | Ottiene il modo in cui i caratteri vengono esportati. |
| [getExportImages()](#getExportImages--) | Ottiene il modo in cui le immagini vengono esportate. |
| [getFontFaceTypes()](#getFontFaceTypes--) | Ottiene i tipi di carattere. |
| [getFontSavingCallback()](#getFontSavingCallback--) | Ottiene il callback che viene chiamato per creare la risorsa per memorizzare il carattere. |
| [getFontSettings()](#getFontSettings--) | Specifica le impostazioni del carattere usate durante il rendering della vista del progetto. |
| [getImageSavingCallback()](#getImageSavingCallback--) | Ottiene il callback che viene chiamato per creare la risorsa per memorizzare il carattere. |
| [getIncludeProjectNameInPageHeader()](#getIncludeProjectNameInPageHeader--) | Ottiene un valore che indica se includere il nome del progetto nell'intestazione della pagina HTML. |
| [getIncludeProjectNameInTitle()](#getIncludeProjectNameInTitle--) | Ottiene un valore che indica se includere il nome del progetto nel titolo HTML. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Ottiene un callback definito dall'utente che viene usato per ottenere uno stream di output per ogni pagina renderizzata. |
| [getPages()](#getPages--) | Ottiene un elenco di numeri di pagina da salvare durante il rendering del layout del progetto. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Ottiene un valore che indica se lo spazio tra l'ultimo compito e il piè di pagina deve essere ridotto. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Ottiene un valore che indica se utilizzare un pennello gradiente durante il rendering del layout del progetto. |
| [setCssSavingCallback(ICssSavingCallback value)](#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-) | Imposta il callback che viene chiamato per creare la risorsa per memorizzare il CSS. |
| [setCssStylePrefix(String value)](#setCssStylePrefix-java.lang.String-) | Imposta il prefisso dello stile CSS. |
| [setExportCss(int value)](#setExportCss-int-) | Imposta il modo in cui il CSS viene esportato. |
| [setExportFonts(int value)](#setExportFonts-int-) | Imposta il modo in cui i caratteri vengono esportati. |
| [setExportImages(int value)](#setExportImages-int-) | Imposta il modo in cui le immagini vengono esportate. |
| [setFontFaceTypes(int value)](#setFontFaceTypes-int-) | Imposta i tipi di carattere. |
| [setFontSavingCallback(IFontSavingCallback value)](#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-) | Imposta la callback che viene chiamata per creare la risorsa per memorizzare il carattere. |
| [setImageSavingCallback(IImageSavingCallback value)](#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-) | Imposta la callback che viene chiamata per creare la risorsa per memorizzare il carattere. |
| [setIncludeProjectNameInPageHeader(boolean value)](#setIncludeProjectNameInPageHeader-boolean-) | Imposta un valore che indica se includere il nome del progetto nell'intestazione della pagina HTML. |
| [setIncludeProjectNameInTitle(boolean value)](#setIncludeProjectNameInTitle-boolean-) | Imposta un valore che indica se includere il nome del progetto nel titolo HTML. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Imposta una callback definita dall'utente che viene utilizzata per ottenere uno stream di output per ogni pagina renderizzata. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Imposta un elenco di numeri di pagina da salvare durante il rendering del layout del progetto. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Imposta un valore che indica se ridurre lo spazio tra l'ultimo compito e il piè di pagina. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Imposta un valore che indica se utilizzare un pennello gradiente durante il rendering del layout del progetto. |
### HtmlSaveOptions() {#HtmlSaveOptions--}
```
public HtmlSaveOptions()
```


Inizializza una nuova istanza della classe [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions).

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public final void copyOutputPropertiesFrom(SaveOptions source)
```


Riservato per uso interno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public SaveOptions deepClone()
```


Riservato per uso interno.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getCssSavingCallback() {#getCssSavingCallback--}
```
public final ICssSavingCallback getCssSavingCallback()
```


Ottiene il callback che viene chiamato per creare la risorsa per memorizzare il CSS.

**Returns:**
[ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) - the callback that is called to create resource to store CSS.
### getCssStylePrefix() {#getCssStylePrefix--}
```
public final String getCssStylePrefix()
```


Ottiene il prefisso dello stile CSS.

**Returns:**
java.lang.String - prefisso stile CSS.
### getExportCss() {#getExportCss--}
```
public final int getExportCss()
```


Ottiene il modo in cui il CSS viene esportato.

**Returns:**
int - il modo in cui i CSS vengono esportati.
### getExportFonts() {#getExportFonts--}
```
public final int getExportFonts()
```


Ottiene il modo in cui i caratteri vengono esportati.

**Returns:**
int - il modo in cui i caratteri vengono esportati.
### getExportImages() {#getExportImages--}
```
public final int getExportImages()
```


Ottiene il modo in cui le immagini vengono esportate.

**Returns:**
int - il modo in cui le immagini vengono esportate.
### getFontFaceTypes() {#getFontFaceTypes--}
```
public final int getFontFaceTypes()
```


Ottiene i tipi di carattere.

Valore: I tipi di carattere.

**Returns:**
int - i tipi di carattere.
### getFontSavingCallback() {#getFontSavingCallback--}
```
public final IFontSavingCallback getFontSavingCallback()
```


Ottiene il callback che viene chiamato per creare la risorsa per memorizzare il carattere.

**Returns:**
[IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) - the callback that is called to create resource to store font.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Specifica le impostazioni del carattere usate durante il rendering della vista del progetto.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getImageSavingCallback() {#getImageSavingCallback--}
```
public final IImageSavingCallback getImageSavingCallback()
```


Ottiene il callback che viene chiamato per creare la risorsa per memorizzare il carattere.

**Returns:**
[IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) - the callback that is called to create resource to store font.
### getIncludeProjectNameInPageHeader() {#getIncludeProjectNameInPageHeader--}
```
public final boolean getIncludeProjectNameInPageHeader()
```


Ottiene un valore che indica se includere il nome del progetto nell'intestazione della pagina HTML.

**Returns:**
boolean - un valore che indica se includere il nome del progetto nell'intestazione della pagina HTML.
### getIncludeProjectNameInTitle() {#getIncludeProjectNameInTitle--}
```
public final boolean getIncludeProjectNameInTitle()
```


Ottiene un valore che indica se includere il nome del progetto nel titolo HTML.

**Returns:**
boolean - un valore che indica se includere il nome del progetto nel titolo HTML.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Ottiene un callback definito dall'utente che viene usato per ottenere uno stream di output per ogni pagina renderizzata.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


Ottiene un elenco di numeri di pagina da salvare durante il rendering del layout del progetto.

--------------------

Tutte le pagine del progetto saranno salvate se questo elenco è vuoto.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - un elenco di numeri di pagina da salvare durante il rendering del layout del progetto.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Ottiene un valore che indica se lo spazio tra l'ultimo compito e il piè di pagina deve essere ridotto.

**Returns:**
boolean - un valore che indica se ridurre lo spazio tra l'ultimo compito e il piè di pagina.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Ottiene un valore che indica se utilizzare un pennello gradiente durante il rendering del layout del progetto.

--------------------

Attualmente l'uso del pennello gradiente non è supportato durante il rendering in HTML.

**Returns:**
boolean - un valore che indica se utilizzare un pennello gradiente durante il rendering del layout del progetto.
### setCssSavingCallback(ICssSavingCallback value) {#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-}
```
public final void setCssSavingCallback(ICssSavingCallback value)
```


Imposta il callback che viene chiamato per creare la risorsa per memorizzare il CSS.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) | la callback che viene chiamata per creare la risorsa per memorizzare i CSS. |

### setCssStylePrefix(String value) {#setCssStylePrefix-java.lang.String-}
```
public final void setCssStylePrefix(String value)
```


Imposta il prefisso dello stile CSS.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | Prefisso stile CSS. |

### setExportCss(int value) {#setExportCss-int-}
```
public final void setExportCss(int value)
```


Imposta il modo in cui il CSS viene esportato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | il modo in cui i CSS vengono esportati. |

### setExportFonts(int value) {#setExportFonts-int-}
```
public final void setExportFonts(int value)
```


Imposta il modo in cui i caratteri vengono esportati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | il modo in cui i font vengono esportati. |

### setExportImages(int value) {#setExportImages-int-}
```
public final void setExportImages(int value)
```


Imposta il modo in cui le immagini vengono esportate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | il modo in cui le immagini vengono esportate. |

### setFontFaceTypes(int value) {#setFontFaceTypes-int-}
```
public final void setFontFaceTypes(int value)
```


Imposta i tipi di carattere.

Valore: I tipi di carattere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | i tipi di font face. |

### setFontSavingCallback(IFontSavingCallback value) {#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-}
```
public final void setFontSavingCallback(IFontSavingCallback value)
```


Imposta la callback che viene chiamata per creare la risorsa per memorizzare il carattere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) | la callback che viene chiamata per creare la risorsa per memorizzare il font. |

### setImageSavingCallback(IImageSavingCallback value) {#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-}
```
public final void setImageSavingCallback(IImageSavingCallback value)
```


Imposta la callback che viene chiamata per creare la risorsa per memorizzare il carattere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) | la callback che viene chiamata per creare la risorsa per memorizzare il font. |

### setIncludeProjectNameInPageHeader(boolean value) {#setIncludeProjectNameInPageHeader-boolean-}
```
public final void setIncludeProjectNameInPageHeader(boolean value)
```


Imposta un valore che indica se includere il nome del progetto nell'intestazione della pagina HTML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se includere il nome del progetto nell'intestazione della pagina HTML. |

### setIncludeProjectNameInTitle(boolean value) {#setIncludeProjectNameInTitle-boolean-}
```
public final void setIncludeProjectNameInTitle(boolean value)
```


Imposta un valore che indica se includere il nome del progetto nel titolo HTML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se includere il nome del progetto nel titolo HTML. |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Imposta una callback definita dall'utente che viene utilizzata per ottenere uno stream di output per ogni pagina renderizzata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | una callback definita dall'utente utilizzata per ottenere uno stream di output per ogni pagina renderizzata. |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


Imposta un elenco di numeri di pagina da salvare durante il rendering del layout del progetto.

--------------------

Tutte le pagine del progetto saranno salvate se questo elenco è vuoto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.List&lt;java.lang.Integer&gt; | un elenco di numeri di pagina da salvare durante il rendering del layout del progetto. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Imposta un valore che indica se ridurre lo spazio tra l'ultimo compito e il piè di pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se ridurre lo spazio tra l'ultima attività e il piè di pagina. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Imposta un valore che indica se utilizzare un pennello gradiente durante il rendering del layout del progetto.

--------------------

Attualmente l'uso del pennello gradiente non è supportato durante il rendering in HTML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se utilizzare un pennello gradiente durante il rendering del layout del progetto. |

