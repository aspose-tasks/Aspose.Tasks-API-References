---
title: "CsvOptions"
second_title: "Aspose.Tasks for Java API 参考"
description: "允许在将项目保存为 CSV 时指定附加选项。"
type: docs
weight: 56
url: /zh/java/com.aspose.tasks/csvoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class CsvOptions extends SimpleSaveOptions
```

允许在将项目保存为 CSV 时指定附加选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [CsvOptions()](#CsvOptions--) | 初始化一个新的 [CsvOptions](../../com.aspose.tasks/csvoptions) 类实例，可用于以 CSV 格式保存项目。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getDataCategory()](#getDataCategory--) | 获取要保存的数据类别。 |
| [getEncoding()](#getEncoding--) | 获取用于保存 CSV 的编码。 |
| [getIncludeHeaders()](#getIncludeHeaders--) | 获取指示是否包含标题的值（默认值为 TRUE）。 |
| [getTextDelimiter()](#getTextDelimiter--) | 获取文本分隔符。 |
| [getView()](#getView--) | 获取要保存为 XLSX 格式的视图列列表（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）。 |
| [setDataCategory(int value)](#setDataCategory-int-) | 设置要保存的数据类别。 |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | 设置用于保存 CSV 的编码。 |
| [setIncludeHeaders(boolean value)](#setIncludeHeaders-boolean-) | 设置指示是否包含标题的值（默认值为 TRUE）。 |
| [setTextDelimiter(int value)](#setTextDelimiter-int-) | 设置文本分隔符。 |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | 设置要保存为 XLSX 格式的视图列列表（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）。 |
### CsvOptions() {#CsvOptions--}
```
public CsvOptions()
```


初始化一个新的 [CsvOptions](../../com.aspose.tasks/csvoptions) 类实例，可用于以 CSV 格式保存项目。

### getDataCategory() {#getDataCategory--}
```
public final int getDataCategory()
```


获取要保存的数据类别。

**Returns:**
int - 要保存的数据类别。
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


获取用于保存 CSV 的编码。

**Returns:**
java.nio.charset.Charset - 用于保存 CSV 的编码。
### getIncludeHeaders() {#getIncludeHeaders--}
```
public final boolean getIncludeHeaders()
```


获取指示是否包含标题的值（默认值为 TRUE）。

**Returns:**
boolean - 指示是否包含标题的值（默认值为 TRUE）。
### getTextDelimiter() {#getTextDelimiter--}
```
public final int getTextDelimiter()
```


获取文本分隔符。

**Returns:**
int - 文本分隔符。
### getView() {#getView--}
```
public final ProjectView getView()
```


获取要保存为 XLSX 格式的视图列列表（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）。如果未设置，则保存默认列。

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setDataCategory(int value) {#setDataCategory-int-}
```
public final void setDataCategory(int value)
```


设置要保存的数据类别。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 要保存的数据类别。 |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


设置用于保存 CSV 的编码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.nio.charset.Charset | 用于保存 CSV 的编码。 |

### setIncludeHeaders(boolean value) {#setIncludeHeaders-boolean-}
```
public final void setIncludeHeaders(boolean value)
```


设置指示是否包含标题的值（默认值为 TRUE）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示是否包含标题的值（默认值为 TRUE）。 |

### setTextDelimiter(int value) {#setTextDelimiter-int-}
```
public final void setTextDelimiter(int value)
```


设置文本分隔符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 文本分隔符。 |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


设置要保存为 XLSX 格式的视图列列表（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）。如果未设置，则保存默认列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | 要保存为 XLSX 格式的视图列列表（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）。 |

