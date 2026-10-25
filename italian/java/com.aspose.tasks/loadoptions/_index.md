---
title: "LoadOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Consente di specificare parametri di caricamento aggiuntivi quando si carica un progetto da file o stream."
type: docs
weight: 148
url: /it/java/com.aspose.tasks/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Consente di specificare parametri di caricamento aggiuntivi quando si carica un progetto da file o stream.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | Inizializza una nuova istanza della classe [LoadOptions](../../com.aspose.tasks/loadoptions). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | Ottiene un token che può essere usato per annullare un'operazione di caricamento del progetto. |
| [getEncoding()](#getEncoding--) | Ottiene la codifica utilizzata per leggere un progetto da formati HTML, MPX, XER e Primavera XML. |
| [getErrorHandler()](#getErrorHandler--) | Ottiene un metodo di callback per gestire gli errori di parsing XML. |
| [getPassword()](#getPassword--) | Ottiene una password di protezione. |
| [getPrimaveraReadOptions()](#getPrimaveraReadOptions--) | Ottiene un'istanza specificata della classe [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) che può essere usata per personalizzare il comportamento del caricamento dei formati Primavera (Primavera P6 XER o Primavera P6 Xml). |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | Imposta un token che può essere usato per annullare un'operazione di caricamento del progetto. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Imposta la codifica utilizzata per leggere un progetto da formati HTML, MPX, XER e Primavera XML. |
| [setErrorHandler(ParseErrorCallback value)](#setErrorHandler-com.aspose.tasks.ParseErrorCallback-) | Imposta un metodo di callback per gestire gli errori di parsing XML. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Imposta una password di protezione. |
| [setPrimaveraReadOptions(PrimaveraReadOptions value)](#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-) | Imposta un'istanza specificata della classe [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) che può essere usata per personalizzare il comportamento del caricamento dei formati Primavera (Primavera P6 XER o Primavera P6 Xml). |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Inizializza una nuova istanza della classe [LoadOptions](../../com.aspose.tasks/loadoptions).

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


Ottiene un token che può essere usato per annullare un'operazione di caricamento del progetto.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project loading operation.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Ottiene la codifica utilizzata per leggere un progetto da formati HTML, MPX, XER e Primavera XML. La codifica predefinita è UTF8.

**Returns:**
java.nio.charset.Charset - codifica utilizzata per leggere un progetto da formati HTML, MPX, XER e Primavera XML.
### getErrorHandler() {#getErrorHandler--}
```
public final ParseErrorCallback getErrorHandler()
```


Ottiene un metodo di callback per gestire gli errori di parsing XML.

**Returns:**
[ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) - a callback method to handle xml parse errors.
### getPassword() {#getPassword--}
```
public final String getPassword()
```


Ottiene una password di protezione.

**Returns:**
java.lang.String - una password di protezione.
### getPrimaveraReadOptions() {#getPrimaveraReadOptions--}
```
public final PrimaveraReadOptions getPrimaveraReadOptions()
```


Ottiene un'istanza specificata della classe [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) che può essere usata per personalizzare il comportamento del caricamento dei formati Primavera (Primavera P6 XER o Primavera P6 Xml).

**Returns:**
[PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) - a specified instance of the [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) class which can be used to customize the behavior of loading Primavera formats (Primavera P6 XER or Primavera P6 Xml).
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


Imposta un token che può essere usato per annullare un'operazione di caricamento del progetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | un token che può essere usato per annullare un'operazione di caricamento del progetto. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Imposta la codifica utilizzata per leggere un progetto da formati HTML, MPX, XER e Primavera XML. La codifica predefinita è UTF8.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.nio.charset.Charset | codifica utilizzata per leggere un progetto da formati HTML, MPX, XER e Primavera XML. |

### setErrorHandler(ParseErrorCallback value) {#setErrorHandler-com.aspose.tasks.ParseErrorCallback-}
```
public final void setErrorHandler(ParseErrorCallback value)
```


Imposta un metodo di callback per gestire gli errori di parsing XML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | un metodo di callback per gestire gli errori di parsing XML. |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Imposta una password di protezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | una password di protezione. |

### setPrimaveraReadOptions(PrimaveraReadOptions value) {#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-}
```
public final void setPrimaveraReadOptions(PrimaveraReadOptions value)
```


Imposta un'istanza specificata della classe [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) che può essere usata per personalizzare il comportamento del caricamento dei formati Primavera (Primavera P6 XER o Primavera P6 Xml).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | un'istanza specificata della classe [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) che può essere utilizzata per personalizzare il comportamento del caricamento dei formati Primavera (Primavera P6 XER o Primavera P6 Xml). |

