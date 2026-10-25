---
title: "Spreadsheet2003SaveOptions"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يسمح بتحديد خيارات إضافية عند تصيير صفحات المشروع إلى Spreadsheet2003."
type: docs
weight: 280
url: /ar/java/com.aspose.tasks/spreadsheet2003saveoptions/
---

**Inheritance:**
java.lang.Object، [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class Spreadsheet2003SaveOptions extends SimpleSaveOptions
```

يسمح بتحديد خيارات إضافية عند تصيير صفحات المشروع إلى Spreadsheet2003.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [Spreadsheet2003SaveOptions()](#Spreadsheet2003SaveOptions--) | ينشئ مثلاً جديداً من الفئة [Spreadsheet2003SaveOptions](../../com.aspose.tasks/spreadsheet2003saveoptions). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getAssignmentView()](#getAssignmentView--) | يحصل على قائمة بأعمدة عرض التعيينات لتصييرها ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [getResourceView()](#getResourceView--) | يحصل على قائمة بأعمدة عرض الموارد لتصييرها ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [getView()](#getView--) | يحصل على قائمة بأعمدة العرض ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) لحفظها. |
| [setAssignmentView(ProjectView value)](#setAssignmentView-com.aspose.tasks.ProjectView-) | يضبط قائمة بأعمدة عرض التعيينات لتصييرها ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [setResourceView(ProjectView value)](#setResourceView-com.aspose.tasks.ProjectView-) | يضبط قائمة بأعمدة عرض الموارد لتصييرها ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | يضبط قائمة بأعمدة العرض ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) لحفظها. |
### Spreadsheet2003SaveOptions() {#Spreadsheet2003SaveOptions--}
```
public Spreadsheet2003SaveOptions()
```


ينشئ مثلاً جديداً من الفئة [Spreadsheet2003SaveOptions](../../com.aspose.tasks/spreadsheet2003saveoptions).

### getAssignmentView() {#getAssignmentView--}
```
public final ProjectView getAssignmentView()
```


يحصل على قائمة بأعمدة عرض التعيينات لتصييرها ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).
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


يحصل على قائمة بأعمدة العرض ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) لحفظها. إذا لم يتم الضبط فسيتم حفظ الأعمدة الافتراضية.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save.
### setAssignmentView(ProjectView value) {#setAssignmentView-com.aspose.tasks.ProjectView-}
```
public final void setAssignmentView(ProjectView value)
```


يضبط قائمة بأعمدة عرض التعيينات لتصييرها ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | قائمة بأعمدة عرض التعيينات لتصييرها ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |

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


يضبط قائمة بأعمدة العرض ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) لحفظها. إذا لم يتم الضبط فسيتم حفظ الأعمدة الافتراضية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | قائمة بأعمدة العرض ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) لحفظها. |

