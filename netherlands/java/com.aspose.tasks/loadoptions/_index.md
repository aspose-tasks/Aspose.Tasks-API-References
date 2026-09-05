---
title: "LoadOptions"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Staat toe extra laadparameters op te geven bij het laden van een project vanuit een bestand of stream."
type: docs
weight: 148
url: /nl/java/com.aspose.tasks/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Staat toe extra laadparameters op te geven bij het laden van een project vanuit een bestand of stream.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | Initialiseert een nieuw exemplaar van de [LoadOptions](../../com.aspose/tasks/loadoptions) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | Verkrijgt een token die kan worden gebruikt om een projectlaadoperatie te annuleren. |
| [getEncoding()](#getEncoding--) | Verkrijgt de codering die wordt gebruikt om een project te lezen uit HTML-, MPX-, XER- en Primavera XML-formaten. |
| [getErrorHandler()](#getErrorHandler--) | Verkrijgt een callback-methode om XML-parsefouten af te handelen. |
| [getPassword()](#getPassword--) | Verkrijgt een beveiligingswachtwoord. |
| [getPrimaveraReadOptions()](#getPrimaveraReadOptions--) | Verkrijgt een opgegeven instantie van de [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) klasse die kan worden gebruikt om het gedrag van het laden van Primavera-formaten (Primavera P6 XER of Primavera P6 Xml) aan te passen. |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | Stelt een token in die kan worden gebruikt om een projectlaadoperatie te annuleren. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Stelt de codering in die wordt gebruikt om een project te lezen uit HTML-, MPX-, XER- en Primavera XML-formaten. |
| [setErrorHandler(ParseErrorCallback value)](#setErrorHandler-com.aspose.tasks.ParseErrorCallback-) | Stelt een callback-methode in om XML-parsefouten af te handelen. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Stelt een beveiligingswachtwoord in. |
| [setPrimaveraReadOptions(PrimaveraReadOptions value)](#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-) | Stelt een opgegeven instantie van de [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) klasse in die kan worden gebruikt om het gedrag van het laden van Primavera-formaten (Primavera P6 XER of Primavera P6 Xml) aan te passen. |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Initialiseert een nieuw exemplaar van de [LoadOptions](../../com.aspose/tasks/loadoptions) klasse.

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


Verkrijgt een token die kan worden gebruikt om een projectlaadoperatie te annuleren.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project loading operation.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Verkrijgt de codering die wordt gebruikt om een project te lezen uit HTML-, MPX-, XER- en Primavera XML-formaten. De standaardcodering is UTF8.

**Returns:**
java.nio.charset.Charset - codering die wordt gebruikt om een project te lezen uit HTML-, MPX-, XER- en Primavera XML-formaten.
### getErrorHandler() {#getErrorHandler--}
```
public final ParseErrorCallback getErrorHandler()
```


Verkrijgt een callback-methode om XML-parsefouten af te handelen.

**Returns:**
[ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) - a callback method to handle xml parse errors.
### getPassword() {#getPassword--}
```
public final String getPassword()
```


Verkrijgt een beveiligingswachtwoord.

**Returns:**
java.lang.String - een beveiligingswachtwoord.
### getPrimaveraReadOptions() {#getPrimaveraReadOptions--}
```
public final PrimaveraReadOptions getPrimaveraReadOptions()
```


Verkrijgt een opgegeven instantie van de [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) klasse die kan worden gebruikt om het gedrag van het laden van Primavera-formaten (Primavera P6 XER of Primavera P6 Xml) aan te passen.

**Returns:**
[PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) - a specified instance of the [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) class which can be used to customize the behavior of loading Primavera formats (Primavera P6 XER or Primavera P6 Xml).
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


Stelt een token in die kan worden gebruikt om een projectlaadoperatie te annuleren.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | een token die kan worden gebruikt om een projectlaadoperatie te annuleren. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Stelt de codering in die wordt gebruikt om een project te lezen uit HTML-, MPX-, XER- en Primavera XML-formaten. De standaardcodering is UTF8.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.nio.charset.Charset | codering die wordt gebruikt om een project te lezen uit HTML-, MPX-, XER- en Primavera XML-formaten. |

### setErrorHandler(ParseErrorCallback value) {#setErrorHandler-com.aspose.tasks.ParseErrorCallback-}
```
public final void setErrorHandler(ParseErrorCallback value)
```


Stelt een callback-methode in om XML-parsefouten af te handelen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | een callback-methode om xml-parsefouten af te handelen. |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Stelt een beveiligingswachtwoord in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | een beschermingswachtwoord. |

### setPrimaveraReadOptions(PrimaveraReadOptions value) {#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-}
```
public final void setPrimaveraReadOptions(PrimaveraReadOptions value)
```


Stelt een opgegeven instantie van de [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) klasse in die kan worden gebruikt om het gedrag van het laden van Primavera-formaten (Primavera P6 XER of Primavera P6 Xml) aan te passen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | een opgegeven instantie van de [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) klasse die kan worden gebruikt om het gedrag van het laden van Primavera-formaten (Primavera P6 XER of Primavera P6 Xml) aan te passen. |

