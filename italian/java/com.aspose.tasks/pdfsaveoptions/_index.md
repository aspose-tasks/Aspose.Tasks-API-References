---
title: "PdfSaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Consente di specificare opzioni aggiuntive durante il rendering delle pagine del progetto in PDF."
type: docs
weight: 191
url: /it/java/com.aspose.tasks/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class PdfSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Consente di specificare opzioni aggiuntive durante il rendering delle pagine del progetto in PDF.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Inizializza una nuova istanza della classe [PdfSaveOptions](../../com.aspose/tasks/pdfsaveoptions) che può essere usata per salvare un documento nel formato [SaveFileFormat](../../com.aspose/tasks/savefileformat). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCompliance()](#getCompliance--) | Ottiene un livello di conformità desiderato per il documento PDF generato. |
| [getEncryptionDetails()](#getEncryptionDetails--) | Ottiene i dettagli della crittografia. |
| [getFontSettings()](#getFontSettings--) | Specifica le impostazioni del carattere usate durante il rendering della vista del progetto. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Ottiene un callback definito dall'utente che viene usato per ottenere uno stream di output per ogni pagina renderizzata. |
| [getPages()](#getPages--) | Ottiene l'elenco dei numeri di pagina da salvare quando si salva il layout del progetto in file separati. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Ottiene un valore che indica se lo spazio tra l'ultimo compito e il piè di pagina deve essere ridotto. |
| [getSaveToSeparateFiles()](#getSaveToSeparateFiles--) | Ottiene un valore che indica se salvare le pagine del progetto in file separati. |
| [getTextCompression()](#getTextCompression--) | Ottiene un tipo di compressione da utilizzare per tutti i flussi di contenuto eccetto le immagini. |
| [setCompliance(int value)](#setCompliance-int-) | Imposta un livello di conformità desiderato per il documento PDF generato. |
| [setEncryptionDetails(PdfEncryptionDetails value)](#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-) | Imposta i dettagli della crittografia. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Imposta una callback definita dall'utente che viene utilizzata per ottenere uno stream di output per ogni pagina renderizzata. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Imposta l'elenco dei numeri di pagina da salvare quando si salva il layout del progetto in file separati. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Imposta un valore che indica se ridurre lo spazio tra l'ultimo compito e il piè di pagina. |
| [setSaveToSeparateFiles(boolean value)](#setSaveToSeparateFiles-boolean-) | Imposta un valore che indica se salvare le pagine del progetto in file separati. |
| [setTextCompression(int value)](#setTextCompression-int-) | Imposta un tipo di compressione da utilizzare per tutti i flussi di contenuto eccetto le immagini. |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Inizializza una nuova istanza della classe [PdfSaveOptions](../../com.aspose/tasks/pdfsaveoptions) che può essere usata per salvare un documento nel formato [SaveFileFormat](../../com.aspose/tasks/savefileformat).

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public void copyOutputPropertiesFrom(SaveOptions source)
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
### getCompliance() {#getCompliance--}
```
public final int getCompliance()
```


Ottiene un livello di conformità desiderato per il documento PDF generato. Il valore predefinito è [PdfCompliance.Pdf15](../../com.aspose/tasks/pdfcompliance\#Pdf15).

**Returns:**
int - un livello di conformità desiderato per il documento PDF generato.
### getEncryptionDetails() {#getEncryptionDetails--}
```
public final PdfEncryptionDetails getEncryptionDetails()
```


Ottiene i dettagli della crittografia. Se non impostato, non verrà eseguita alcuna crittografia.

**Returns:**
[PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) - an encryption details.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Specifica le impostazioni del carattere usate durante il rendering della vista del progetto.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Ottiene una callback definita dall'utente che è usata per ottenere uno stream di output per ogni pagina renderizzata. È applicabile quando l'opzione `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)) è usata.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


Ottiene l'elenco dei numeri di pagina da salvare quando si salva il layout del progetto in file separati.

--------------------

Tutte le pagine saranno salvate se questo elenco è vuoto.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - l'elenco dei numeri di pagina da salvare quando si salva il layout del progetto in file separati.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Ottiene un valore che indica se lo spazio tra l'ultimo compito e il piè di pagina deve essere ridotto.

**Returns:**
boolean - un valore che indica se ridurre lo spazio tra l'ultimo compito e il piè di pagina.
### getSaveToSeparateFiles() {#getSaveToSeparateFiles--}
```
public final boolean getSaveToSeparateFiles()
```


Ottiene un valore che indica se salvare le pagine del progetto in file separati.

**Returns:**
boolean - un valore che indica se salvare le pagine del progetto in file separati.
### getTextCompression() {#getTextCompression--}
```
public final int getTextCompression()
```


Ottiene un tipo di compressione da utilizzare per tutti i flussi di contenuto eccetto le immagini. Il valore predefinito è [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\\#Flate).

**Returns:**
int - un tipo di compressione da utilizzare per tutti i flussi di contenuto eccetto le immagini.
### setCompliance(int value) {#setCompliance-int-}
```
public final void setCompliance(int value)
```


Imposta un livello di conformità desiderato per il documento PDF generato. Il valore predefinito è [PdfCompliance.Pdf15](../../com.aspose.tasks/pdfcompliance\\#Pdf15).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un livello di conformità desiderato per il documento PDF generato. |

### setEncryptionDetails(PdfEncryptionDetails value) {#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-}
```
public final void setEncryptionDetails(PdfEncryptionDetails value)
```


Imposta i dettagli di crittografia. Se non impostato, non verrà eseguita alcuna crittografia.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) | i dettagli di crittografia. |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Imposta una callback definita dall'utente che viene utilizzata per ottenere un flusso di output per ogni pagina renderizzata. È applicabile quando l'opzione `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\\#setSaveToSeparateFiles-boolean-)) è utilizzata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | una callback definita dall'utente utilizzata per ottenere uno stream di output per ogni pagina renderizzata. |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


Imposta l'elenco dei numeri di pagina da salvare quando si salva il layout del progetto in file separati.

--------------------

Tutte le pagine saranno salvate se questo elenco è vuoto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.List&lt;java.lang.Integer&gt; | l'elenco dei numeri di pagina da salvare quando si salva il layout del progetto in file separati. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Imposta un valore che indica se ridurre lo spazio tra l'ultimo compito e il piè di pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se ridurre lo spazio tra l'ultima attività e il piè di pagina. |

### setSaveToSeparateFiles(boolean value) {#setSaveToSeparateFiles-boolean-}
```
public final void setSaveToSeparateFiles(boolean value)
```


Imposta un valore che indica se salvare le pagine del progetto in file separati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se salvare le pagine del progetto in file separati. |

### setTextCompression(int value) {#setTextCompression-int-}
```
public final void setTextCompression(int value)
```


Imposta un tipo di compressione da utilizzare per tutti i flussi di contenuto eccetto le immagini. Il valore predefinito è [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\\#Flate).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un tipo di compressione da utilizzare per tutti i flussi di contenuto eccetto le immagini. |

