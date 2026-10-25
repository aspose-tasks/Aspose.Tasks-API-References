---
title: "LoadOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Ermöglicht das Angeben zusätzlicher Ladeparameter beim Laden eines Projekts aus einer Datei oder einem Stream."
type: docs
weight: 148
url: /de/java/com.aspose.tasks/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Ermöglicht das Angeben zusätzlicher Ladeparameter beim Laden eines Projekts aus einer Datei oder einem Stream.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | Initialisiert eine neue Instanz der Klasse [LoadOptions](../../com.aspose/tasks/loadoptions). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | Liefert ein Token, das zum Abbrechen eines Projektladevorgangs verwendet werden kann. |
| [getEncoding()](#getEncoding--) | Liefert die Kodierung, die zum Lesen eines Projekts aus den Formaten HTML, MPX, XER und Primavera XML verwendet wird. |
| [getErrorHandler()](#getErrorHandler--) | Liefert eine Rückrufmethode zum Behandeln von xml-Parse-Fehlern. |
| [getPassword()](#getPassword--) | Ruft ein Schutzkennwort ab. |
| [getPrimaveraReadOptions()](#getPrimaveraReadOptions--) | Ruft eine angegebene Instanz der [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions)-Klasse ab, die verwendet werden kann, um das Verhalten beim Laden von Primavera-Formaten (Primavera P6 XER oder Primavera P6 Xml) anzupassen. |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | Legt ein Token fest, das verwendet werden kann, um einen Projektladevorgang abzubrechen. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Legt die Codierung fest, die zum Lesen eines Projekts aus HTML-, MPX-, XER- und Primavera-XML-Formaten verwendet wird. |
| [setErrorHandler(ParseErrorCallback value)](#setErrorHandler-com.aspose.tasks.ParseErrorCallback-) | Legt eine Rückruffunktion fest, um XML-Parse-Fehler zu behandeln. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Legt ein Schutzkennwort fest. |
| [setPrimaveraReadOptions(PrimaveraReadOptions value)](#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-) | Legt eine angegebene Instanz der [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions)-Klasse fest, die verwendet werden kann, um das Verhalten beim Laden von Primavera-Formaten (Primavera P6 XER oder Primavera P6 Xml) anzupassen. |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Initialisiert eine neue Instanz der Klasse [LoadOptions](../../com.aspose/tasks/loadoptions).

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


Liefert ein Token, das zum Abbrechen eines Projektladevorgangs verwendet werden kann.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project loading operation.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Ruft die Codierung ab, die zum Lesen eines Projekts aus HTML-, MPX-, XER- und Primavera-XML-Formaten verwendet wird. Die Standardcodierung ist UTF8.

**Returns:**
java.nio.charset.Charset – Codierung, die zum Lesen eines Projekts aus HTML-, MPX-, XER- und Primavera-XML-Formaten verwendet wird.
### getErrorHandler() {#getErrorHandler--}
```
public final ParseErrorCallback getErrorHandler()
```


Liefert eine Rückrufmethode zum Behandeln von xml-Parse-Fehlern.

**Returns:**
[ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) - a callback method to handle xml parse errors.
### getPassword() {#getPassword--}
```
public final String getPassword()
```


Ruft ein Schutzkennwort ab.

**Returns:**
java.lang.String – ein Schutzkennwort.
### getPrimaveraReadOptions() {#getPrimaveraReadOptions--}
```
public final PrimaveraReadOptions getPrimaveraReadOptions()
```


Ruft eine angegebene Instanz der [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions)-Klasse ab, die verwendet werden kann, um das Verhalten beim Laden von Primavera-Formaten (Primavera P6 XER oder Primavera P6 Xml) anzupassen.

**Returns:**
[PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) - a specified instance of the [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) class which can be used to customize the behavior of loading Primavera formats (Primavera P6 XER or Primavera P6 Xml).
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


Legt ein Token fest, das verwendet werden kann, um einen Projektladevorgang abzubrechen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | ein Token, das verwendet werden kann, um einen Projektladevorgang abzubrechen. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Legt die Codierung fest, die zum Lesen eines Projekts aus HTML-, MPX-, XER- und Primavera-XML-Formaten verwendet wird. Die Standardcodierung ist UTF8.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.nio.charset.Charset | Codierung, die zum Lesen eines Projekts aus HTML-, MPX-, XER- und Primavera-XML-Formaten verwendet wird. |

### setErrorHandler(ParseErrorCallback value) {#setErrorHandler-com.aspose.tasks.ParseErrorCallback-}
```
public final void setErrorHandler(ParseErrorCallback value)
```


Legt eine Rückruffunktion fest, um XML-Parse-Fehler zu behandeln.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | eine Rückruffunktion, um XML-Parse-Fehler zu behandeln. |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Legt ein Schutzkennwort fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | ein Schutzkennwort. |

### setPrimaveraReadOptions(PrimaveraReadOptions value) {#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-}
```
public final void setPrimaveraReadOptions(PrimaveraReadOptions value)
```


Legt eine angegebene Instanz der [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions)-Klasse fest, die verwendet werden kann, um das Verhalten beim Laden von Primavera-Formaten (Primavera P6 XER oder Primavera P6 Xml) anzupassen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | eine angegebene Instanz der [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions)-Klasse, die verwendet werden kann, um das Verhalten beim Laden von Primavera-Formaten (Primavera P6 XER oder Primavera P6 Xml) anzupassen. |

