---
title: "SvgOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Consente di specificare opzioni aggiuntive durante il rendering delle pagine del progetto in SVG."
type: docs
weight: 283
url: /it/java/com.aspose.tasks/svgoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.ICloneableSaveOptions
```
public class SvgOptions extends SaveOptions implements ICloneableSaveOptions
```

Consente di specificare opzioni aggiuntive durante il rendering delle pagine del progetto in SVG.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [SvgOptions()](#SvgOptions--) | Inizializza una nuova istanza della classe [SvgOptions](../../com.aspose.tasks/svgoptions) che può essere utilizzata per salvare il progetto in formato SVG. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getPageSavingCallback()](#getPageSavingCallback--) | Ottiene un callback di implementazione definito dall'utente che viene utilizzato per ottenere un flusso di output per ogni pagina renderizzata. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Determina se utilizzare il pennello gradiente durante il rendering del layout del progetto. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Imposta un callback di implementazione definito dall'utente che viene utilizzato per ottenere un flusso di output per ogni pagina renderizzata. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Determina se utilizzare il pennello gradiente durante il rendering del layout del progetto. |
### SvgOptions() {#SvgOptions--}
```
public SvgOptions()
```


Inizializza una nuova istanza della classe [SvgOptions](../../com.aspose.tasks/svgoptions) che può essere utilizzata per salvare il progetto in formato SVG.

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
public final SaveOptions deepClone()
```


Riservato per uso interno.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Ottiene un callback di implementazione definito dall'utente che viene utilizzato per ottenere un flusso di output per ogni pagina renderizzata.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined implementation callback which is used to get an output stream for each rendered page.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Determina se utilizzare il pennello gradiente durante il rendering del layout del progetto.

--------------------

Attualmente l'uso del pennello gradiente non è supportato per il rendering in SVG.

**Returns:**
boolean - valore che indica se utilizzare il pennello gradiente durante il rendering del layout del progetto.
### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Imposta un callback di implementazione definito dall'utente che viene utilizzato per ottenere un flusso di output per ogni pagina renderizzata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | un callback di implementazione definito dall'utente che viene utilizzato per ottenere un flusso di output per ogni pagina renderizzata. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Determina se utilizzare il pennello gradiente durante il rendering del layout del progetto.

--------------------

Attualmente l'uso del pennello gradiente non è supportato per il rendering in SVG.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | valore che indica se utilizzare il pennello gradiente durante il rendering del layout del progetto. |

