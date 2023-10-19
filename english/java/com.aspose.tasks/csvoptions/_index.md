---
title: CsvOptions
second_title: Aspose.Tasks for Java API Reference
description: Allows to specify additional options when saving project to CSV.
type: docs
weight: 56
url: /java/com.aspose.tasks/csvoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class CsvOptions extends SimpleSaveOptions
```

Allows to specify additional options when saving project to CSV.
## Constructors

| Constructor | Description |
| --- | --- |
| [CsvOptions()](#CsvOptions--) | Initializes a new instance of the [CsvOptions](../../com.aspose.tasks/csvoptions) class which can be used to save project in CSV format. |
## Methods

| Method | Description |
| --- | --- |
| [getDataCategory()](#getDataCategory--) | Gets a data category to be saved. |
| [getEncoding()](#getEncoding--) | Gets an encoding to save CSV with. |
| [getIncludeHeaders()](#getIncludeHeaders--) | Gets a value indicating whether to include headers or not (default value is TRUE). |
| [getTextDelimiter()](#getTextDelimiter--) | Gets a text delimiter. |
| [getView()](#getView--) | Gets a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format. |
| [setDataCategory(int value)](#setDataCategory-int-) | Sets a data category to be saved. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Sets an encoding to save CSV with. |
| [setIncludeHeaders(boolean value)](#setIncludeHeaders-boolean-) | Sets a value indicating whether to include headers or not (default value is TRUE). |
| [setTextDelimiter(int value)](#setTextDelimiter-int-) | Sets a text delimiter. |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Sets a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format. |
### CsvOptions() {#CsvOptions--}
```
public CsvOptions()
```


Initializes a new instance of the [CsvOptions](../../com.aspose.tasks/csvoptions) class which can be used to save project in CSV format.

### getDataCategory() {#getDataCategory--}
```
public final int getDataCategory()
```


Gets a data category to be saved.

**Returns:**
int - a data category to be saved.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Gets an encoding to save CSV with.

**Returns:**
java.nio.charset.Charset - an encoding to save CSV with.
### getIncludeHeaders() {#getIncludeHeaders--}
```
public final boolean getIncludeHeaders()
```


Gets a value indicating whether to include headers or not (default value is TRUE).

**Returns:**
boolean - a value indicating whether to include headers or not (default value is TRUE).
### getTextDelimiter() {#getTextDelimiter--}
```
public final int getTextDelimiter()
```


Gets a text delimiter.

**Returns:**
int - a text delimiter.
### getView() {#getView--}
```
public final ProjectView getView()
```


Gets a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format. If not set then default columns are saved.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setDataCategory(int value) {#setDataCategory-int-}
```
public final void setDataCategory(int value)
```


Sets a data category to be saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a data category to be saved. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Sets an encoding to save CSV with.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.nio.charset.Charset | an encoding to save CSV with. |

### setIncludeHeaders(boolean value) {#setIncludeHeaders-boolean-}
```
public final void setIncludeHeaders(boolean value)
```


Sets a value indicating whether to include headers or not (default value is TRUE).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to include headers or not (default value is TRUE). |

### setTextDelimiter(int value) {#setTextDelimiter-int-}
```
public final void setTextDelimiter(int value)
```


Sets a text delimiter.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a text delimiter. |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Sets a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format. If not set then default columns are saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format. |

