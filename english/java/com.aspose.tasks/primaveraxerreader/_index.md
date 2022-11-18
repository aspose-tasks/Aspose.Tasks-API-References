---
title: PrimaveraXerReader
second_title: Aspose.Tasks for Java API Reference
description: Represents a reader to read Project UIDs from Primavera XER file
type: docs
weight: 186
url: /java/com.aspose.tasks/primaveraxerreader/
---

**Inheritance:**
java.lang.Object
```
public class PrimaveraXerReader
```

Represents a reader to read Project UIDs from Primavera XER file
## Constructors

| Constructor | Description |
| --- | --- |
| [PrimaveraXerReader(String xerFilePath)](#PrimaveraXerReader-java.lang.String-) | Initializes a new instance of the [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader) class. |
| [PrimaveraXerReader(InputStream stream)](#PrimaveraXerReader-java.io.InputStream-) | Initializes a new instance of the [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader) class. |
## Methods

| Method | Description |
| --- | --- |
| [getProjectUids()](#getProjectUids--) | Return a list of the projects' unique identifiers. |
### PrimaveraXerReader(String xerFilePath) {#PrimaveraXerReader-java.lang.String-}
```
public PrimaveraXerReader(String xerFilePath)
```


Initializes a new instance of the [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| xerFilePath | java.lang.String | Path to .xer file where Primavera project or projects are located. |

### PrimaveraXerReader(InputStream stream) {#PrimaveraXerReader-java.io.InputStream-}
```
public PrimaveraXerReader(InputStream stream)
```


Initializes a new instance of the [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | Stream with Primavera XER content. |

### getProjectUids() {#getProjectUids--}
```
public final List<Integer> getProjectUids()
```


Return a list of the projects' unique identifiers.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - List of projects' unique identifiers.
