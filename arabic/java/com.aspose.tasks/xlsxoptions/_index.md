---
title: "XlsxOptions"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يسمح بتحديد خيارات إضافية عند تحويل صفحات المشروع إلى XLSX."
type: docs
weight: 368
url: /ar/java/com.aspose.tasks/xlsxoptions/
---

**Inheritance:**
java.lang.Object، [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class XlsxOptions extends SimpleSaveOptions
```

يسمح بتحديد خيارات إضافية عند تحويل صفحات المشروع إلى XLSX.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [XlsxOptions()](#XlsxOptions--) | ينشئ مثيلاً جديدًا من الفئة [XlsxOptions](../../com.aspose.tasks/xlsxoptions) التي يمكن استخدامها لحفظ المشروع بتنسيق XLSX. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getAssignmentView()](#getAssignmentView--) | يحصل على قائمة بأعمدة عرض التعيينات لتصييرها ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [getEncoding()](#getEncoding--) | يحصل على ترميز ملف XLSX الناتج. |
| [getResourceView()](#getResourceView--) | يحصل على قائمة بأعمدة عرض الموارد لتصييرها ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [getView()](#getView--) | يحصل على قائمة بأعمدة العرض ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) لحفظها بتنسيق XLSX. |
| [setAssignmentView(ProjectView value)](#setAssignmentView-com.aspose.tasks.ProjectView-) | يضبط قائمة بأعمدة عرض التعيينات لتصييرها ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | يضبط ترميز ملف XLSX الناتج. |
| [setResourceView(ProjectView value)](#setResourceView-com.aspose.tasks.ProjectView-) | يضبط قائمة بأعمدة عرض الموارد لتصييرها ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | يضبط قائمة بأعمدة العرض ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) لحفظها بتنسيق XLSX. |
### XlsxOptions() {#XlsxOptions--}
```
public XlsxOptions()
```


ينشئ مثيلاً جديدًا من الفئة [XlsxOptions](../../com.aspose.tasks/xlsxoptions) التي يمكن استخدامها لحفظ المشروع بتنسيق XLSX.

### getAssignmentView() {#getAssignmentView--}
```
public final ProjectView getAssignmentView()
```


يحصل على قائمة بأعمدة عرض التعيينات لتصييرها ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


يحصل على ترميز ملف XLSX الناتج. القيمة الافتراضية هي java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8.

**Returns:**
java.nio.charset.Charset - ترميز ملف XLSX الناتج.
### getResourceView() {#getResourceView--}
```
public final ProjectView getResourceView()
```


يحصل على قائمة بأعمدة عرض الموارد لتصييرها ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the resource view columns to render ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).
### getView() {#getView--}
```
public final ProjectView getView()
```


يحصل على قائمة بأعمدة العرض ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) لحفظها بتنسيق XLSX. إذا لم يتم تحديدها فسيتم حفظ الأعمدة الافتراضية.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setAssignmentView(ProjectView value) {#setAssignmentView-com.aspose.tasks.ProjectView-}
```
public final void setAssignmentView(ProjectView value)
```


يضبط قائمة بأعمدة عرض التعيينات لتصييرها ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | قائمة بأعمدة عرض التعيينات لتصييرها ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


يضبط ترميز ملف XLSX الناتج. القيمة الافتراضية هي java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.nio.charset.Charset | ترميز ملف XLSX الناتج. |

### setResourceView(ProjectView value) {#setResourceView-com.aspose.tasks.ProjectView-}
```
public final void setResourceView(ProjectView value)
```


يضبط قائمة بأعمدة عرض الموارد لتصييرها ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | قائمة بأعمدة عرض الموارد لتصييرها ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


يضبط قائمة بأعمدة العرض ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) لحفظها بتنسيق XLSX. إذا لم يتم تحديدها فسيتم حفظ الأعمدة الافتراضية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | قائمة بأعمدة العرض ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) لحفظها بتنسيق XLSX. |

