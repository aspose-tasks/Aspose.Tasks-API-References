---
title: "CsvOptions"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يسمح بتحديد خيارات إضافية عند حفظ المشروع إلى CSV."
type: docs
weight: 56
url: /ar/java/com.aspose.tasks/csvoptions/
---

**Inheritance:**
java.lang.Object، [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class CsvOptions extends SimpleSaveOptions
```

يسمح بتحديد خيارات إضافية عند حفظ المشروع إلى CSV.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [CsvOptions()](#CsvOptions--) | ينشئ مثلاً جديداً من الفئة [CsvOptions](../../com.aspose/tasks/csvoptions) التي يمكن استخدامها لحفظ المشروع بتنسيق CSV. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getDataCategory()](#getDataCategory--) | يحصل على فئة البيانات التي سيتم حفظها. |
| [getEncoding()](#getEncoding--) | يحصل على الترميز لحفظ CSV به. |
| [getIncludeHeaders()](#getIncludeHeaders--) | يحصل على قيمة تشير إلى ما إذا كان سيتم تضمين رؤوس الأعمدة أم لا (القيمة الافتراضية هي TRUE). |
| [getTextDelimiter()](#getTextDelimiter--) | يحصل على محدد النص. |
| [getView()](#getView--) | يحصل على قائمة بأعمدة العرض ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) لحفظها بتنسيق XLSX. |
| [setDataCategory(int value)](#setDataCategory-int-) | يضبط فئة البيانات التي سيتم حفظها. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | يضبط الترميز لحفظ CSV به. |
| [setIncludeHeaders(boolean value)](#setIncludeHeaders-boolean-) | يضبط قيمة تشير إلى ما إذا كان سيتم تضمين رؤوس الأعمدة أم لا (القيمة الافتراضية هي TRUE). |
| [setTextDelimiter(int value)](#setTextDelimiter-int-) | يضبط محدد النص. |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | يضبط قائمة بأعمدة العرض ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) لحفظها بتنسيق XLSX. |
### CsvOptions() {#CsvOptions--}
```
public CsvOptions()
```


ينشئ مثلاً جديداً من الفئة [CsvOptions](../../com.aspose/tasks/csvoptions) التي يمكن استخدامها لحفظ المشروع بتنسيق CSV.

### getDataCategory() {#getDataCategory--}
```
public final int getDataCategory()
```


يحصل على فئة البيانات التي سيتم حفظها.

**Returns:**
int - فئة بيانات ليتم حفظها.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


يحصل على الترميز لحفظ CSV به.

**Returns:**
java.nio.charset.Charset - ترميز لحفظ CSV به.
### getIncludeHeaders() {#getIncludeHeaders--}
```
public final boolean getIncludeHeaders()
```


يحصل على قيمة تشير إلى ما إذا كان سيتم تضمين رؤوس الأعمدة أم لا (القيمة الافتراضية هي TRUE).

**Returns:**
boolean - قيمة تشير إلى ما إذا كان سيتم تضمين رؤوس الأعمدة أم لا (القيمة الافتراضية هي TRUE).
### getTextDelimiter() {#getTextDelimiter--}
```
public final int getTextDelimiter()
```


يحصل على محدد النص.

**Returns:**
int - محدد نص.
### getView() {#getView--}
```
public final ProjectView getView()
```


يحصل على قائمة بأعمدة العرض ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) لحفظها بتنسيق XLSX. إذا لم يتم تحديدها فسيتم حفظ الأعمدة الافتراضية.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setDataCategory(int value) {#setDataCategory-int-}
```
public final void setDataCategory(int value)
```


يضبط فئة البيانات التي سيتم حفظها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | فئة بيانات ليتم حفظها. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


يضبط الترميز لحفظ CSV به.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.nio.charset.Charset | ترميز لحفظ CSV به. |

### setIncludeHeaders(boolean value) {#setIncludeHeaders-boolean-}
```
public final void setIncludeHeaders(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان سيتم تضمين رؤوس الأعمدة أم لا (القيمة الافتراضية هي TRUE).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان سيتم تضمين رؤوس الأعمدة أم لا (القيمة الافتراضية هي TRUE). |

### setTextDelimiter(int value) {#setTextDelimiter-int-}
```
public final void setTextDelimiter(int value)
```


يضبط محدد النص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | محدد نص. |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


يضبط قائمة بأعمدة العرض ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) لحفظها بتنسيق XLSX. إذا لم يتم تحديدها فسيتم حفظ الأعمدة الافتراضية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | قائمة بأعمدة العرض ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) لحفظها بتنسيق XLSX. |

