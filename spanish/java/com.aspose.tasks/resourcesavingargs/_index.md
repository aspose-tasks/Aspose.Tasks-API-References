---
title: "ResourceSavingArgs"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Esta clase representa un conjunto de datos relacionados con el guardado de archivos de recursos externos que ocurre durante la conversión al formato HTML."
type: docs
weight: 254
url: /es/java/com.aspose.tasks/resourcesavingargs/
---

**Inheritance:**
java.lang.Object
```
public class ResourceSavingArgs
```

Esta clase representa un conjunto de datos relacionados con el guardado de archivos de recursos externos que ocurre durante la conversión al formato HTML.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ResourceSavingArgs()](#ResourceSavingArgs--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [closeStreamIfRequired()](#closeStreamIfRequired--) | Cierre el flujo si KeepStreamOpen es falso, de lo contrario vacíelo. |
| [getFileName()](#getFileName--) | Obtiene el nombre de archivo supuesto que va del convertidor al código del método personalizado. |
| [getKeepStreamOpen()](#getKeepStreamOpen--) | Obtiene un valor que indica si el flujo permanecerá abierto después de que finalice el guardado de recursos. |
| [getStream()](#getStream--) | Obtiene el contenido binario del archivo guardado. |
| [getUri()](#getUri--) | Obtiene el URI del recurso. |
| [setFileName(String value)](#setFileName-java.lang.String-) | Establece el nombre de archivo supuesto que va del convertidor al código del método personalizado. |
| [setKeepStreamOpen(boolean value)](#setKeepStreamOpen-boolean-) | Establece un valor que indica si el flujo permanecerá abierto después de que finalice el guardado de recursos. |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | Establece el contenido binario del archivo guardado. |
| [setUri(String value)](#setUri-java.lang.String-) | Establece el URI del recurso. |
### ResourceSavingArgs() {#ResourceSavingArgs--}
```
public ResourceSavingArgs()
```


### closeStreamIfRequired() {#closeStreamIfRequired--}
```
public final void closeStreamIfRequired()
```


Cierre el flujo si KeepStreamOpen es falso, de lo contrario vacíelo.

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Obtiene el nombre de archivo supuesto que va del convertidor al código del método personalizado. Puede usarse en código personalizado para decidir cómo procesar o dónde guardar ese archivo.

**Returns:**
java.lang.String - el nombre de archivo supuesto que va del convertidor al código del método personalizado.
### getKeepStreamOpen() {#getKeepStreamOpen--}
```
public final boolean getKeepStreamOpen()
```


Obtiene un valor que indica si el flujo permanecerá abierto después de que finalice el guardado de recursos.

**Returns:**
boolean - un valor que indica si el flujo permanecerá abierto después de que finalice el guardado de recursos.
### getStream() {#getStream--}
```
public final OutputStream getStream()
```


Obtiene el contenido binario del archivo guardado.

**Returns:**
java.io.OutputStream - el contenido binario del archivo guardado.
### getUri() {#getUri--}
```
public final String getUri()
```


Obtiene el URI del recurso.

**Returns:**
java.lang.String - el URI del recurso.
### setFileName(String value) {#setFileName-java.lang.String-}
```
public final void setFileName(String value)
```


Establece el nombre de archivo supuesto que va del convertidor al código del método personalizado. Puede usarse en código personalizado para decidir cómo procesar o dónde guardar ese archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | el nombre de archivo supuesto que va del convertidor al código del método personalizado. |

### setKeepStreamOpen(boolean value) {#setKeepStreamOpen-boolean-}
```
public final void setKeepStreamOpen(boolean value)
```


Establece un valor que indica si el flujo permanecerá abierto después de que finalice el guardado de recursos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si el flujo permanecerá abierto después de que finalice el guardado de recursos. |

### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public final void setStream(OutputStream value)
```


Establece el contenido binario del archivo guardado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.io.OutputStream | el contenido binario del archivo guardado. |

### setUri(String value) {#setUri-java.lang.String-}
```
public final void setUri(String value)
```


Establece el URI del recurso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | el URI del recurso. |

