---
title: "ResourceSavingArgs"
second_title: "Aspose.Tasks for Java API Reference"
description: "Questa classe rappresenta un insieme di dati relativi al salvataggio di file di risorse esterne che avviene durante la conversione in formato HTML."
type: docs
weight: 254
url: /it/java/com.aspose.tasks/resourcesavingargs/
---

**Inheritance:**
java.lang.Object
```
public class ResourceSavingArgs
```

Questa classe rappresenta un insieme di dati relativi al salvataggio di file di risorse esterni che avviene durante la conversione in formato HTML.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ResourceSavingArgs()](#ResourceSavingArgs--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [closeStreamIfRequired()](#closeStreamIfRequired--) | Chiudi lo stream se KeepStreamOpen è false, altrimenti svuotalo. |
| [getFileName()](#getFileName--) | Ottiene il nome file previsto che passa dal convertitore al codice del metodo personalizzato. |
| [getKeepStreamOpen()](#getKeepStreamOpen--) | Ottiene un valore che indica se lo stream rimarrà aperto dopo il completamento del salvataggio delle risorse. |
| [getStream()](#getStream--) | Ottiene il contenuto binario del file salvato. |
| [getUri()](#getUri--) | Ottiene l'URI della risorsa. |
| [setFileName(String value)](#setFileName-java.lang.String-) | Imposta il nome file previsto che passa dal convertitore al codice del metodo personalizzato. |
| [setKeepStreamOpen(boolean value)](#setKeepStreamOpen-boolean-) | Imposta un valore che indica se lo stream rimarrà aperto dopo il completamento del salvataggio delle risorse. |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | Imposta il contenuto binario del file salvato. |
| [setUri(String value)](#setUri-java.lang.String-) | Imposta l'URI della risorsa. |
### ResourceSavingArgs() {#ResourceSavingArgs--}
```
public ResourceSavingArgs()
```


### closeStreamIfRequired() {#closeStreamIfRequired--}
```
public final void closeStreamIfRequired()
```


Chiudi lo stream se KeepStreamOpen è false, altrimenti svuotalo.

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Ottiene il nome file previsto che passa dal convertitore al codice del metodo personalizzato. Può essere usato nel codice personalizzato per decidere come elaborarlo o dove salvare quel file.

**Returns:**
java.lang.String - il nome file previsto che passa dal convertitore al codice del metodo personalizzato.
### getKeepStreamOpen() {#getKeepStreamOpen--}
```
public final boolean getKeepStreamOpen()
```


Ottiene un valore che indica se lo stream rimarrà aperto dopo il completamento del salvataggio delle risorse.

**Returns:**
boolean - un valore che indica se lo stream rimarrà aperto dopo il completamento del salvataggio delle risorse.
### getStream() {#getStream--}
```
public final OutputStream getStream()
```


Ottiene il contenuto binario del file salvato.

**Returns:**
java.io.OutputStream - il contenuto binario del file salvato.
### getUri() {#getUri--}
```
public final String getUri()
```


Ottiene l'URI della risorsa.

**Returns:**
java.lang.String - l'URI della risorsa.
### setFileName(String value) {#setFileName-java.lang.String-}
```
public final void setFileName(String value)
```


Imposta il nome file previsto che passa dal convertitore al codice del metodo personalizzato. Può essere usato nel codice personalizzato per decidere come elaborarlo o dove salvare quel file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | il nome file previsto che passa dal convertitore al codice del metodo personalizzato. |

### setKeepStreamOpen(boolean value) {#setKeepStreamOpen-boolean-}
```
public final void setKeepStreamOpen(boolean value)
```


Imposta un valore che indica se lo stream rimarrà aperto dopo il completamento del salvataggio delle risorse.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se lo stream rimarrà aperto dopo il completamento del salvataggio delle risorse. |

### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public final void setStream(OutputStream value)
```


Imposta il contenuto binario del file salvato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.io.OutputStream | il contenuto binario del file salvato. |

### setUri(String value) {#setUri-java.lang.String-}
```
public final void setUri(String value)
```


Imposta l'URI della risorsa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | l'URI della risorsa. |

