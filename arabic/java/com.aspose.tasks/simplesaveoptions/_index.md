---
title: "SimpleSaveOptions"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "هذه فئة أساسية مجردة تسمح للمستخدم بتحديد الخيارات الأساسية عند حفظ مشروع بتنسيق معين."
type: docs
weight: 277
url: /ar/java/com.aspose.tasks/simplesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SimpleSaveOptions
```

هذه فئة أساسية مجردة تسمح للمستخدم بتحديد الخيارات الأساسية عند حفظ مشروع بتنسيق معين.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [SimpleSaveOptions()](#SimpleSaveOptions--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getSaveFormat()](#getSaveFormat--) | يحصل على التنسيق الذي سيتم حفظ المستند به إذا تم استخدام كائن خيارات الحفظ هذا. |
| [getTasksComparer()](#getTasksComparer--) | يحصل على المقارن لفرز المهام في مخطط جانت ومخطط ورقة المهام. |
| [getTasksFilter()](#getTasksFilter--) | يحصل على الشرط المستخدم لتصفية المهام المعروضة في مخططات جانت، ورقة المهام واستخدام المهام. |
| [setTasksComparer(Comparator&lt;Task&gt; value)](#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--) | يضبط المقارن لفرز المهام في مخطط جانت ومخطط ورقة المهام. |
| [setTasksFilter(ICondition&lt;Task&gt; value)](#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | يضبط الشرط المستخدم لتصفية المهام المعروضة في مخططات جانت، ورقة المهام واستخدام المهام. |
### SimpleSaveOptions() {#SimpleSaveOptions--}
```
public SimpleSaveOptions()
```


### getSaveFormat() {#getSaveFormat--}
```
public final int getSaveFormat()
```


يحصل على التنسيق الذي سيتم حفظ المستند به إذا تم استخدام كائن خيارات الحفظ هذا.

**Returns:**
int - الـ [SaveFileFormat](../../com.aspose.tasks/savefileformat) الذي سيتم حفظ المستند به.
### getTasksComparer() {#getTasksComparer--}
```
public final Comparator<Task> getTasksComparer()
```


يحصل على المقارن لفرز المهام في مخطط جانت ومخطط ورقة المهام.

**Returns:**
java.util.Comparator&lt;com.aspose.tasks.Task&gt; - المقارن لفرز المهام في مخطط جانت ومخطط ورقة المهام.
### getTasksFilter() {#getTasksFilter--}
```
public final ICondition<Task> getTasksFilter()
```


يحصل على الشرط المستخدم لتصفية المهام المعروضة في مخططات جانت، ورقة المهام واستخدام المهام.

--------------------

إذا لم يتم تحديد القيمة، يتم استخدام الفلتر الافتراضي الذي يزيل المهام غير المرئية — أي المهام التابعة للمهام المدمجة.

**Returns:**
[ICondition](../../com.aspose.tasks/icondition) - the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts.
### setTasksComparer(Comparator&lt;Task&gt; value) {#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--}
```
public final void setTasksComparer(Comparator<Task> value)
```


يضبط المقارن لفرز المهام في مخطط جانت ومخطط ورقة المهام.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Comparator&lt;com.aspose.tasks.Task&gt; | المقارن لفرز المهام في مخطط جانت ومخطط ورقة المهام. |

### setTasksFilter(ICondition&lt;Task&gt; value) {#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public final void setTasksFilter(ICondition<Task> value)
```


يضبط الشرط المستخدم لتصفية المهام المعروضة في مخططات جانت، ورقة المهام واستخدام المهام.

--------------------

إذا لم يتم تحديد القيمة، يتم استخدام الفلتر الافتراضي الذي يزيل المهام غير المرئية — أي المهام التابعة للمهام المدمجة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | الشرط الذي يُستخدم لتصفية المهام المعروضة في مخططات Gantt وTask Sheet وTask Usage. |

