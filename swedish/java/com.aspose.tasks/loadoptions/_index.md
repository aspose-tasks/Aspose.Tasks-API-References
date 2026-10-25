---
title: "LoadOptions"
second_title: "Aspose.Tasks for Java API-referens"
description: "Tillåter att ange ytterligare laddningsparametrar när ett projekt läses in från fil eller ström."
type: docs
weight: 148
url: /sv/java/com.aspose.tasks/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Tillåter att ange ytterligare laddningsparametrar när ett projekt läses in från fil eller ström.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | Initierar en ny instans av klassen [LoadOptions](../../com.aspose/tasks/loadoptions). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | Hämtar en token som kan användas för att avbryta en projektladdningsoperation. |
| [getEncoding()](#getEncoding--) | Hämtar kodning som används för att läsa ett projekt från HTML-, MPX-, XER- och Primavera XML-format. |
| [getErrorHandler()](#getErrorHandler--) | Hämtar en återuppringningsmetod för att hantera xml‑tolkningsfel. |
| [getPassword()](#getPassword--) | Hämtar ett skyddslösenord. |
| [getPrimaveraReadOptions()](#getPrimaveraReadOptions--) | Hämtar en specificerad instans av klassen [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions) som kan användas för att anpassa beteendet vid laddning av Primavera-format (Primavera P6 XER eller Primavera P6 Xml). |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | Ställer in en token som kan användas för att avbryta en projektladdningsoperation. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Ställer in kodning som används för att läsa ett projekt från HTML-, MPX-, XER- och Primavera XML-format. |
| [setErrorHandler(ParseErrorCallback value)](#setErrorHandler-com.aspose.tasks.ParseErrorCallback-) | Ställer in en återuppringningsmetod för att hantera xml‑tolkningsfel. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Ställer in ett skyddslösenord. |
| [setPrimaveraReadOptions(PrimaveraReadOptions value)](#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-) | Ställer in en specificerad instans av klassen [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) som kan användas för att anpassa beteendet vid inläsning av Primavera-format (Primavera P6 XER eller Primavera P6 Xml). |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Initierar en ny instans av klassen [LoadOptions](../../com.aspose/tasks/loadoptions).

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


Hämtar en token som kan användas för att avbryta en projektladdningsoperation.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project loading operation.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Hämtar kodning som används för att läsa ett projekt från HTML-, MPX-, XER- och Primavera XML-format. Standardkodningen är UTF8.

**Returns:**
java.nio.charset.Charset – kodning som används för att läsa ett projekt från HTML-, MPX-, XER- och Primavera XML-format.
### getErrorHandler() {#getErrorHandler--}
```
public final ParseErrorCallback getErrorHandler()
```


Hämtar en återuppringningsmetod för att hantera xml‑tolkningsfel.

**Returns:**
[ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) - a callback method to handle xml parse errors.
### getPassword() {#getPassword--}
```
public final String getPassword()
```


Hämtar ett skyddslösenord.

**Returns:**
java.lang.String – ett skyddslösenord.
### getPrimaveraReadOptions() {#getPrimaveraReadOptions--}
```
public final PrimaveraReadOptions getPrimaveraReadOptions()
```


Hämtar en specificerad instans av klassen [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions) som kan användas för att anpassa beteendet vid laddning av Primavera-format (Primavera P6 XER eller Primavera P6 Xml).

**Returns:**
[PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) - a specified instance of the [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) class which can be used to customize the behavior of loading Primavera formats (Primavera P6 XER or Primavera P6 Xml).
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


Ställer in en token som kan användas för att avbryta en projektladdningsoperation.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | en token som kan användas för att avbryta en projektläsningsoperation. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Ställer in kodning som används för att läsa ett projekt från HTML-, MPX-, XER- och Primavera XML-format. Standardkodningen är UTF8.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.nio.charset.Charset | kodning som används för att läsa ett projekt från HTML-, MPX-, XER- och Primavera XML-format. |

### setErrorHandler(ParseErrorCallback value) {#setErrorHandler-com.aspose.tasks.ParseErrorCallback-}
```
public final void setErrorHandler(ParseErrorCallback value)
```


Ställer in en återuppringningsmetod för att hantera xml‑tolkningsfel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | en återuppringningsmetod för att hantera xml‑tolkningsfel. |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Ställer in ett skyddslösenord.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | ett skyddslösenord. |

### setPrimaveraReadOptions(PrimaveraReadOptions value) {#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-}
```
public final void setPrimaveraReadOptions(PrimaveraReadOptions value)
```


Ställer in en specificerad instans av klassen [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) som kan användas för att anpassa beteendet vid inläsning av Primavera-format (Primavera P6 XER eller Primavera P6 Xml).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | en specificerad instans av klassen [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) som kan användas för att anpassa beteendet vid inläsning av Primavera-format (Primavera P6 XER eller Primavera P6 Xml). |

