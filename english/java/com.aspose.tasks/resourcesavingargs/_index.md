---
title: ResourceSavingArgs
second_title: Aspose.Tasks for Java API Reference
description: This class represents set of data that related to external resource files saving that occurs during conversion to HTML format.
type: docs
weight: 253
url: /java/com.aspose.tasks/resourcesavingargs/
---

**Inheritance:**
java.lang.Object
```
public class ResourceSavingArgs
```

This class represents set of data that related to external resource file's saving that occurs during conversion to HTML format.
## Constructors

| Constructor | Description |
| --- | --- |
| [ResourceSavingArgs()](#ResourceSavingArgs--) |  |
## Methods

| Method | Description |
| --- | --- |
| [closeStreamIfRequired()](#closeStreamIfRequired--) | Close stream if KeepStreamOpen is false, else flush it. |
| [getFileName()](#getFileName--) | Gets the supposed file name that goes from converter to code of custom method. |
| [getKeepStreamOpen()](#getKeepStreamOpen--) | Gets a value indicating whether the stream will be kept open after resource saving finishes. |
| [getStream()](#getStream--) | Gets the binary content of saved file. |
| [getUri()](#getUri--) | Gets the resource URI. |
| [setFileName(String value)](#setFileName-java.lang.String-) | Sets the supposed file name that goes from converter to code of custom method. |
| [setKeepStreamOpen(boolean value)](#setKeepStreamOpen-boolean-) | Sets a value indicating whether the stream will be kept open after resource saving finishes. |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | Sets the binary content of saved file. |
| [setUri(String value)](#setUri-java.lang.String-) | Sets the resource URI. |
### ResourceSavingArgs() {#ResourceSavingArgs--}
```
public ResourceSavingArgs()
```


### closeStreamIfRequired() {#closeStreamIfRequired--}
```
public final void closeStreamIfRequired()
```


Close stream if KeepStreamOpen is false, else flush it.

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Gets the supposed file name that goes from converter to code of custom method. Can be use in custom code to decide how to process or where save that file.

**Returns:**
java.lang.String - the supposed file name that goes from converter to code of custom method.
### getKeepStreamOpen() {#getKeepStreamOpen--}
```
public final boolean getKeepStreamOpen()
```


Gets a value indicating whether the stream will be kept open after resource saving finishes.

**Returns:**
boolean - a value indicating whether the stream will be kept open after resource saving finishes.
### getStream() {#getStream--}
```
public final OutputStream getStream()
```


Gets the binary content of saved file.

**Returns:**
java.io.OutputStream - the binary content of saved file.
### getUri() {#getUri--}
```
public final String getUri()
```


Gets the resource URI.

**Returns:**
java.lang.String - the resource URI.
### setFileName(String value) {#setFileName-java.lang.String-}
```
public final void setFileName(String value)
```


Sets the supposed file name that goes from converter to code of custom method. Can be use in custom code to decide how to process or where save that file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the supposed file name that goes from converter to code of custom method. |

### setKeepStreamOpen(boolean value) {#setKeepStreamOpen-boolean-}
```
public final void setKeepStreamOpen(boolean value)
```


Sets a value indicating whether the stream will be kept open after resource saving finishes.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether the stream will be kept open after resource saving finishes. |

### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public final void setStream(OutputStream value)
```


Sets the binary content of saved file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.io.OutputStream | the binary content of saved file. |

### setUri(String value) {#setUri-java.lang.String-}
```
public final void setUri(String value)
```


Sets the resource URI.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the resource URI. |

