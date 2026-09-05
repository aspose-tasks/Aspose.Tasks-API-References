---
title: "ImageSaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Consente di specificare opzioni aggiuntive durante il rendering delle pagine del progetto in immagini."
type: docs
weight: 134
url: /it/java/com.aspose.tasks/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class ImageSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Consente di specificare opzioni aggiuntive durante il rendering delle pagine del progetto in immagini.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ImageSaveOptions(int saveFormat)](#ImageSaveOptions-int-) | Inizializza una nuova istanza della classe [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) che può essere usata per salvare le immagini renderizzate nei formati TIFF, PNG, BMP o JPEG. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getFontSettings()](#getFontSettings--) | Specifica le impostazioni del carattere usate durante il rendering della vista del progetto. |
| [getHorizontalResolution()](#getHorizontalResolution--) | Restituisce la risoluzione orizzontale in dpi. |
| [getJpegQuality()](#getJpegQuality--) | Restituisce la qualità JPEG. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Ottiene un callback definito dall'utente che viene usato per ottenere uno stream di output per ogni pagina renderizzata. |
| [getPages()](#getPages--) | Restituisce un elenco di numeri di pagina da salvare quando si salva il layout del progetto in file separati. |
| [getPixelFormat()](#getPixelFormat--) | Restituisce il formato dei dati di colore per ogni pixel nell'immagine. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Ottiene un valore che indica se lo spazio tra l'ultimo compito e il piè di pagina deve essere ridotto. |
| [getTiffCompression()](#getTiffCompression--) | Restituisce il tipo di compressione da applicare quando si salvano le immagini generate nel formato TIFF. |
| [getVerticalResolution()](#getVerticalResolution--) | Restituisce la risoluzione verticale in dpi. |
| [setHorizontalResolution(float value)](#setHorizontalResolution-float-) | Imposta la risoluzione orizzontale in dpi. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | Imposta la qualità JPEG. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Imposta una callback definita dall'utente che viene utilizzata per ottenere uno stream di output per ogni pagina renderizzata. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Imposta un elenco di numeri di pagina da salvare quando si salva il layout del progetto in file separati. |
| [setPixelFormat(int value)](#setPixelFormat-int-) | Imposta il formato dei dati di colore per ogni pixel nell'immagine. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Imposta un valore che indica se ridurre lo spazio tra l'ultimo compito e il piè di pagina. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Imposta il tipo di compressione da applicare quando si salvano le immagini generate nel formato TIFF. |
| [setVerticalResolution(float value)](#setVerticalResolution-float-) | Imposta la risoluzione verticale in dpi. |
### ImageSaveOptions(int saveFormat) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int saveFormat)
```


Inizializza una nuova istanza della classe [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) che può essere usata per salvare le immagini renderizzate nei formati TIFF, PNG, BMP o JPEG.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| saveFormat | int | Può essere TIFF, PNG, BMP o JPEG[SaveFileFormat](../../com.aspose.tasks/savefileformat). |

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
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Specifica le impostazioni del carattere usate durante il rendering della vista del progetto.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getHorizontalResolution() {#getHorizontalResolution--}
```
public final float getHorizontalResolution()
```


Restituisce la risoluzione orizzontale in dpi.

**Returns:**
float - la risoluzione orizzontale in dpi.
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


Restituisce una qualità JPEG. L'intervallo di valori consentito è 0..100.

**Returns:**
int - una qualità JPEG.
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


Restituisce un elenco di numeri di pagina da salvare quando si salva il layout del progetto in file separati.

--------------------

Tutte le pagine saranno salvate se questo elenco è vuoto.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - un elenco di numeri di pagina da salvare quando si salva il layout del progetto in file separati.
### getPixelFormat() {#getPixelFormat--}
```
public final int getPixelFormat()
```


Restituisce il formato dei dati di colore per ogni pixel nell'immagine.

**Returns:**
int - il formato dei dati di colore per ogni pixel nell'immagine.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Ottiene un valore che indica se lo spazio tra l'ultimo compito e il piè di pagina deve essere ridotto.

**Returns:**
boolean - un valore che indica se ridurre lo spazio tra l'ultimo compito e il piè di pagina.
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


Restituisce il tipo di compressione da applicare quando si salvano le immagini generate nel formato TIFF.

--------------------

Ha effetto solo quando si salva in TIFF. Il valore predefinito è `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-)).

**Returns:**
int - il tipo di compressione da applicare quando si salvano le immagini generate nel formato TIFF.
### getVerticalResolution() {#getVerticalResolution--}
```
public final float getVerticalResolution()
```


Restituisce la risoluzione verticale in dpi.

**Returns:**
float - la risoluzione verticale in dpi.
### setHorizontalResolution(float value) {#setHorizontalResolution-float-}
```
public final void setHorizontalResolution(float value)
```


Imposta la risoluzione orizzontale in dpi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float | la risoluzione orizzontale in dpi. |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


Imposta la qualità JPEG. L'intervallo di valori consentito è 0..100.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | una qualità JPEG. |

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


Imposta un elenco di numeri di pagina da salvare quando si salva il layout del progetto in file separati.

--------------------

Tutte le pagine saranno salvate se questo elenco è vuoto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.List&lt;java.lang.Integer&gt; | un elenco di numeri di pagina da salvare quando si salva il layout del progetto in file separati. |

### setPixelFormat(int value) {#setPixelFormat-int-}
```
public final void setPixelFormat(int value)
```


Imposta il formato dei dati di colore per ogni pixel nell'immagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | il formato dei dati colore per ogni pixel nell'immagine. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Imposta un valore che indica se ridurre lo spazio tra l'ultimo compito e il piè di pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se ridurre lo spazio tra l'ultima attività e il piè di pagina. |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


Imposta il tipo di compressione da applicare quando si salvano le immagini generate nel formato TIFF.

--------------------

Ha effetto solo quando si salva in TIFF. Il valore predefinito è `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-)).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | il tipo di compressione da applicare quando si salvano le immagini generate nel formato TIFF. |

### setVerticalResolution(float value) {#setVerticalResolution-float-}
```
public final void setVerticalResolution(float value)
```


Imposta la risoluzione verticale in dpi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float | la risoluzione verticale in dpi. |

