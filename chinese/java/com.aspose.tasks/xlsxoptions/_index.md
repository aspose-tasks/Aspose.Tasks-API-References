---
title: "XlsxOptions"
second_title: "Aspose.Tasks for Java API 参考"
description: "允许在将项目页面渲染为 XLSX 时指定附加选项。"
type: docs
weight: 368
url: /zh/java/com.aspose.tasks/xlsxoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class XlsxOptions extends SimpleSaveOptions
```

允许在将项目页面渲染为 XLSX 时指定附加选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [XlsxOptions()](#XlsxOptions--) | 初始化一个新的 [XlsxOptions](../../com.aspose.tasks/xlsxoptions) 类实例，可用于以 XLSX 格式保存项目。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getAssignmentView()](#getAssignmentView--) | 获取要呈现的分配视图列的列表 ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn))。 |
| [getEncoding()](#getEncoding--) | 获取生成的 XLSX 文件的编码。 |
| [getResourceView()](#getResourceView--) | 获取要呈现的资源视图列的列表 ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn))。 |
| [getView()](#getView--) | 获取要保存为 XLSX 格式的视图列列表（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）。 |
| [setAssignmentView(ProjectView value)](#setAssignmentView-com.aspose.tasks.ProjectView-) | 设置要呈现的分配视图列的列表 ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn))。 |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | 设置生成的 XLSX 文件的编码。 |
| [setResourceView(ProjectView value)](#setResourceView-com.aspose.tasks.ProjectView-) | 设置要呈现的资源视图列的列表 ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn))。 |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | 设置要保存为 XLSX 格式的视图列列表（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）。 |
### XlsxOptions() {#XlsxOptions--}
```
public XlsxOptions()
```


初始化一个新的 [XlsxOptions](../../com.aspose.tasks/xlsxoptions) 类实例，可用于以 XLSX 格式保存项目。

### getAssignmentView() {#getAssignmentView--}
```
public final ProjectView getAssignmentView()
```


获取要呈现的分配视图列的列表 ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn))。

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


获取生成的 XLSX 文件的编码。默认值为 java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8。

**Returns:**
java.nio.charset.Charset - 生成的 XLSX 文件的编码。
### getResourceView() {#getResourceView--}
```
public final ProjectView getResourceView()
```


获取要呈现的资源视图列的列表 ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn))。

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the resource view columns to render ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).
### getView() {#getView--}
```
public final ProjectView getView()
```


获取要保存为 XLSX 格式的视图列列表（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）。如果未设置，则保存默认列。

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setAssignmentView(ProjectView value) {#setAssignmentView-com.aspose.tasks.ProjectView-}
```
public final void setAssignmentView(ProjectView value)
```


设置要呈现的分配视图列的列表 ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn))。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | 要呈现的分配视图列的列表 ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn))。 |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


设置生成的 XLSX 文件的编码。默认值为 java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.nio.charset.Charset | 生成的 XLSX 文件的编码。 |

### setResourceView(ProjectView value) {#setResourceView-com.aspose.tasks.ProjectView-}
```
public final void setResourceView(ProjectView value)
```


设置要呈现的资源视图列的列表 ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn))。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | 要呈现的资源视图列的列表 ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn))。 |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


设置要保存为 XLSX 格式的视图列列表（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）。如果未设置，则保存默认列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | 要保存为 XLSX 格式的视图列列表（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）。 |

