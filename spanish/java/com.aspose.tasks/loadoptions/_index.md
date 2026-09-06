---
title: "LoadOptions"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Permite especificar parámetros de carga adicionales al cargar un proyecto desde un archivo o flujo."
type: docs
weight: 148
url: /es/java/com.aspose.tasks/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Permite especificar parámetros de carga adicionales al cargar un proyecto desde un archivo o flujo.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | Inicializa una nueva instancia de la clase [LoadOptions](../../com.aspose.tasks/loadoptions). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | Obtiene un token que puede usarse para cancelar una operación de carga de proyecto. |
| [getEncoding()](#getEncoding--) | Obtiene la codificación que se usa para leer un proyecto desde los formatos HTML, MPX, XER y Primavera XML. |
| [getErrorHandler()](#getErrorHandler--) | Obtiene un método de devolución de llamada para manejar errores de análisis XML. |
| [getPassword()](#getPassword--) | Obtiene una contraseña de protección. |
| [getPrimaveraReadOptions()](#getPrimaveraReadOptions--) | Obtiene una instancia especificada de la clase [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) que puede usarse para personalizar el comportamiento de carga de formatos Primavera (Primavera P6 XER o Primavera P6 Xml). |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | Establece un token que puede usarse para cancelar una operación de carga de proyecto. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Establece la codificación que se usa para leer un proyecto desde los formatos HTML, MPX, XER y Primavera XML. |
| [setErrorHandler(ParseErrorCallback value)](#setErrorHandler-com.aspose.tasks.ParseErrorCallback-) | Establece un método de devolución de llamada para manejar errores de análisis XML. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Establece una contraseña de protección. |
| [setPrimaveraReadOptions(PrimaveraReadOptions value)](#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-) | Establece una instancia especificada de la clase [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) que puede usarse para personalizar el comportamiento de carga de formatos Primavera (Primavera P6 XER o Primavera P6 Xml). |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Inicializa una nueva instancia de la clase [LoadOptions](../../com.aspose.tasks/loadoptions).

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


Obtiene un token que puede usarse para cancelar una operación de carga de proyecto.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project loading operation.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Obtiene la codificación que se usa para leer un proyecto desde los formatos HTML, MPX, XER y Primavera XML. La codificación predeterminada es UTF8.

**Returns:**
java.nio.charset.Charset - codificación que se usa para leer un proyecto desde los formatos HTML, MPX, XER y Primavera XML.
### getErrorHandler() {#getErrorHandler--}
```
public final ParseErrorCallback getErrorHandler()
```


Obtiene un método de devolución de llamada para manejar errores de análisis XML.

**Returns:**
[ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) - a callback method to handle xml parse errors.
### getPassword() {#getPassword--}
```
public final String getPassword()
```


Obtiene una contraseña de protección.

**Returns:**
java.lang.String - una contraseña de protección.
### getPrimaveraReadOptions() {#getPrimaveraReadOptions--}
```
public final PrimaveraReadOptions getPrimaveraReadOptions()
```


Obtiene una instancia especificada de la clase [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) que puede usarse para personalizar el comportamiento de carga de formatos Primavera (Primavera P6 XER o Primavera P6 Xml).

**Returns:**
[PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) - a specified instance of the [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) class which can be used to customize the behavior of loading Primavera formats (Primavera P6 XER or Primavera P6 Xml).
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


Establece un token que puede usarse para cancelar una operación de carga de proyecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | un token que puede usarse para cancelar una operación de carga de proyecto. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Establece la codificación que se usa para leer un proyecto desde los formatos HTML, MPX, XER y Primavera XML. La codificación predeterminada es UTF8.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.nio.charset.Charset | codificación que se usa para leer un proyecto desde los formatos HTML, MPX, XER y Primavera XML. |

### setErrorHandler(ParseErrorCallback value) {#setErrorHandler-com.aspose.tasks.ParseErrorCallback-}
```
public final void setErrorHandler(ParseErrorCallback value)
```


Establece un método de devolución de llamada para manejar errores de análisis XML.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | un método de devolución de llamada para manejar errores de análisis xml. |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Establece una contraseña de protección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | una contraseña de protección. |

### setPrimaveraReadOptions(PrimaveraReadOptions value) {#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-}
```
public final void setPrimaveraReadOptions(PrimaveraReadOptions value)
```


Establece una instancia especificada de la clase [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) que puede usarse para personalizar el comportamiento de carga de formatos Primavera (Primavera P6 XER o Primavera P6 Xml).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | una instancia especificada de la clase [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) que puede usarse para personalizar el comportamiento de carga de formatos Primavera (Primavera P6 XER o Primavera P6 Xml). |

