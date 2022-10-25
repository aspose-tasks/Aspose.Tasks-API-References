---
title: PrimaveraXmlReader
second_title: Aspose.Tasks for Java API Reference
description: Represents a reader which allows to retrieve Project UIDs from Primavera Xml file.
type: docs
weight: 186
url: /java/com.aspose.tasks/primaveraxmlreader/
---

**Inheritance:**
java.lang.Object
```
public class PrimaveraXmlReader
```

Represents a reader which allows to retrieve Project UIDs from Primavera Xml file.
## Constructors

| Constructor | Description |
| --- | --- |
| [PrimaveraXmlReader(String templatePath)](#PrimaveraXmlReader-java.lang.String-) | Initializes a new instance of the [PrimaveraXmlReader](../../com.aspose.tasks/primaveraxmlreader) class. |
| [PrimaveraXmlReader(InputStream stream)](#PrimaveraXmlReader-java.io.InputStream-) | Initializes a new instance of the [PrimaveraXmlReader](../../com.aspose.tasks/primaveraxmlreader) class. |
## Methods

| Method | Description |
| --- | --- |
| [getProjectUids()](#getProjectUids--) | Return a list of the projects' unique identifiers. |
### PrimaveraXmlReader(String templatePath) {#PrimaveraXmlReader-java.lang.String-}
```
public PrimaveraXmlReader(String templatePath)
```


Initializes a new instance of the [PrimaveraXmlReader](../../com.aspose.tasks/primaveraxmlreader) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| templatePath | java.lang.String | Path to template where Primavera Xml project is located |

### PrimaveraXmlReader(InputStream stream) {#PrimaveraXmlReader-java.io.InputStream-}
```
public PrimaveraXmlReader(InputStream stream)
```


Initializes a new instance of the [PrimaveraXmlReader](../../com.aspose.tasks/primaveraxmlreader) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | Stream containing Primavera Xml content. |

### getProjectUids() {#getProjectUids--}
```
public final List<Integer> getProjectUids()
```


Return a list of the projects' unique identifiers.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - List of projects' unique identifiers.
