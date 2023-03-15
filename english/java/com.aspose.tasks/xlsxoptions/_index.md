---
title: XlsxOptions
second_title: Aspose.Tasks for Java API Reference
description: Allows to specify additional options when rendering project pages to XLSX.
type: docs
weight: 342
url: /java/com.aspose.tasks/xlsxoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)
```
public class XlsxOptions extends SaveOptions
```

Allows to specify additional options when rendering project pages to XLSX.
## Constructors

| Constructor | Description |
| --- | --- |
| [XlsxOptions()](#XlsxOptions--) | Initializes a new instance of the [XlsxOptions](../../com.aspose.tasks/xlsxoptions) class that can be used to save project in XLSX format. |
## Methods

| Method | Description |
| --- | --- |
| [getAssignmentView()](#getAssignmentView--) | Gets a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [getEncoding()](#getEncoding--) | Gets the encoding of the resulting XLSX file. |
| [getResourceView()](#getResourceView--) | Gets a list of the resource view columns to render ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [setAssignmentView(ProjectView value)](#setAssignmentView-com.aspose.tasks.ProjectView-) | Sets a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Sets the encoding of the resulting XLSX file. |
| [setResourceView(ProjectView value)](#setResourceView-com.aspose.tasks.ProjectView-) | Sets a list of the resource view columns to render ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
### XlsxOptions() {#XlsxOptions--}
```
public XlsxOptions()
```


Initializes a new instance of the [XlsxOptions](../../com.aspose.tasks/xlsxoptions) class that can be used to save project in XLSX format.

### getAssignmentView() {#getAssignmentView--}
```
public final ProjectView getAssignmentView()
```


Gets a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Gets the encoding of the resulting XLSX file. The default value is java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8.

**Returns:**
java.nio.charset.Charset - the encoding of the resulting XLSX file.
### getResourceView() {#getResourceView--}
```
public final ProjectView getResourceView()
```


Gets a list of the resource view columns to render ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the resource view columns to render ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).
### setAssignmentView(ProjectView value) {#setAssignmentView-com.aspose.tasks.ProjectView-}
```
public final void setAssignmentView(ProjectView value)
```


Sets a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Sets the encoding of the resulting XLSX file. The default value is java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.nio.charset.Charset | the encoding of the resulting XLSX file. |

### setResourceView(ProjectView value) {#setResourceView-com.aspose.tasks.ProjectView-}
```
public final void setResourceView(ProjectView value)
```


Sets a list of the resource view columns to render ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | a list of the resource view columns to render ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |

