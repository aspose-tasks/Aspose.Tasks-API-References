---
title: "TaskBaseline"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل الخط الأساسي لمهمة."
type: docs
weight: 291
url: /ar/java/com.aspose.tasks/taskbaseline/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.Baseline](../../com.aspose.tasks/baseline)

**All Implemented Interfaces:**
java.lang.Comparable
```
public class TaskBaseline extends Baseline implements Comparable<Baseline>
```

يمثل الخط الأساسي لمهمة.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [TaskBaseline(Task task)](#TaskBaseline-com.aspose.tasks.Task-) | ينشئ مثيلاً جديداً من الفئة [TaskBaseline](../../com.aspose.tasks/taskbaseline). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [compareTo(TaskBaseline other)](#compareTo-com.aspose.tasks.TaskBaseline-) | تنفيذ واجهة IComparable. |
| [equals(TaskBaseline other)](#equals-com.aspose.tasks.TaskBaseline-) | يعيد قيمة تشير إلى ما إذا كان هذا المثيل مساويًا لكائن TaskBaseline المحدد. |
| [equals(Object obj)](#equals-java.lang.Object-) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| [getDuration()](#getDuration--) | يحصل على المدة المجدولة للمهمة عندما تم حفظ الخط الأساسي. |
| [getEstimatedDuration()](#getEstimatedDuration--) | يحصل على قيمة تشير إلى ما إذا كانت مدة الخط الأساسي للمهمة مقدرة. |
| [getFinish()](#getFinish--) | يحصل على تاريخ الانتهاء المجدول للمهمة عندما تم حفظ الخط الأساسي. |
| [getFixedCost()](#getFixedCost--) | يحصل على تكلفة ثابتة للمهمة عندما تم حفظ الخط الأساسي. |
| [getInterim()](#getInterim--) | يحصل على قيمة تشير إلى ما إذا كان هذا خطًا أساسيًا مؤقتًا. |
| [getStart()](#getStart--) | يحصل على تاريخ البدء المجدول للمهمة عندما تم حفظ الخط الأساسي. |
| [getTimephasedData()](#getTimephasedData--) | يحصل على مثيل TimephasedDataCollection لهذا الكائن. |
| [hashCode()](#hashCode--) | يعيد قيمة رمز تجزئة للمثيل من الفئة [TaskBaseline](../../com.aspose.tasks/taskbaseline). |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | يضبط المدة المجدولة للمهمة عندما تم حفظ الخط الأساسي. |
| [setEstimatedDuration(boolean value)](#setEstimatedDuration-boolean-) | يضبط قيمة تشير إلى ما إذا كانت مدة الخط الأساسي للمهمة مقدرة. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | يضبط تاريخ الانتهاء المجدول للمهمة عندما تم حفظ الخط الأساسي. |
| [setFixedCost(double value)](#setFixedCost-double-) | يضبط تكلفة ثابتة للمهمة عندما تم حفظ الخط الأساسي. |
| [setInterim(boolean value)](#setInterim-boolean-) | يضبط قيمة تشير إلى ما إذا كان هذا خطًا أساسيًا مؤقتًا. |
| [setStart(Date value)](#setStart-java.util.Date-) | يضبط تاريخ بدء المهمة المجدول عندما تم حفظ الخط الأساسي. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | يضبط مثيل TimephasedDataCollection لهذا الكائن. |
### TaskBaseline(Task task) {#TaskBaseline-com.aspose.tasks.Task-}
```
public TaskBaseline(Task task)
```


ينشئ مثيلاً جديداً من الفئة [TaskBaseline](../../com.aspose.tasks/taskbaseline).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | مهمة الأصل للخط الأساسي. |

### compareTo(TaskBaseline other) {#compareTo-com.aspose.tasks.TaskBaseline-}
```
public final int compareTo(TaskBaseline other)
```


تنفيذ واجهة IComparable. يقارن هذا المثيل بالعنصر Baseline المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | العنصر Baseline المحدد للمقارنة مع هذا المثيل. |

**Returns:**
int - يعيد -1 إذا كان هذا المثيل أصغر من العنصر المحدد، 1 إذا كان هذا المثيل أكبر من العنصر المحدد؛ وإلا يعيد 0
### equals(TaskBaseline other) {#equals-com.aspose.tasks.TaskBaseline-}
```
public final boolean equals(TaskBaseline other)
```


يعيد قيمة تشير إلى ما إذا كان هذا المثيل مساويًا لكائن TaskBaseline المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | الكائن AssignmentBaseline المحدد للمقارنة مع هذه الحالة. |

**Returns:**
boolean - يُرجِع true إذا كان هذا المثيل مساويًا لكائن TaskBaseline المحدد؛ وإلا، false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | java.lang.Object | الكائن للمقارنة مع هذا المثيل. |

**Returns:**
boolean - **True** إذا كان الكائن المحدد هو TaskBaseline يمتلك نفس قيمة UID لهذا المثيل؛ وإلا، **false**.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


يحصل على المدة المجدولة للمهمة عندما تم حفظ الخط الأساسي.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the scheduled duration of the task when the baseline was saved.
### getEstimatedDuration() {#getEstimatedDuration--}
```
public final boolean getEstimatedDuration()
```


يحصل على قيمة تشير إلى ما إذا كانت مدة الخط الأساسي للمهمة مقدرة.

**Returns:**
boolean - قيمة تشير إلى ما إذا كانت مدة الخط الأساسي للمهمة مقدرة.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


يحصل على تاريخ الانتهاء المجدول للمهمة عندما تم حفظ الخط الأساسي.

**Returns:**
java.util.Date - تاريخ الانتهاء المجدول للمهمة عندما تم حفظ الخط الأساسي.
### getFixedCost() {#getFixedCost--}
```
public final double getFixedCost()
```


يحصل على تكلفة ثابتة للمهمة عندما تم حفظ الخط الأساسي.

**Returns:**
double - تكلفة ثابتة للمهمة عندما تم حفظ الخط الأساسي.
### getInterim() {#getInterim--}
```
public final boolean getInterim()
```


يحصل على قيمة تشير إلى ما إذا كان هذا خطًا أساسيًا مؤقتًا.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان هذا خطًا أساسيًا مؤقتًا.
### getStart() {#getStart--}
```
public final Date getStart()
```


يحصل على تاريخ البدء المجدول للمهمة عندما تم حفظ الخط الأساسي.

**Returns:**
java.util.Date - تاريخ بدء المهمة المجدول عندما تم حفظ الخط الأساسي.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


يحصل على مثيل TimephasedDataCollection لهذا الكائن. البيانات المرحلية المرتبطة بالخط الأساسي للمهمة.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - a TimephasedDataCollection instance for this object.
### hashCode() {#hashCode--}
```
public int hashCode()
```


يعيد قيمة رمز تجزئة للمثيل من الفئة [TaskBaseline](../../com.aspose.tasks/taskbaseline).

**Returns:**
عدد صحيح - يُعيد قيمة رمز التجزئة لهذا الكائن.
### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


يضبط المدة المجدولة للمهمة عندما تم حفظ الخط الأساسي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | المدة المجدولة للمهمة عندما تم حفظ الخط الأساسي. |

### setEstimatedDuration(boolean value) {#setEstimatedDuration-boolean-}
```
public final void setEstimatedDuration(boolean value)
```


يضبط قيمة تشير إلى ما إذا كانت مدة الخط الأساسي للمهمة مقدرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كانت مدة الخط الأساسي للمهمة مقدرة. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


يضبط تاريخ الانتهاء المجدول للمهمة عندما تم حفظ الخط الأساسي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | تاريخ الانتهاء المجدول للمهمة عندما تم حفظ الخط الأساسي. |

### setFixedCost(double value) {#setFixedCost-double-}
```
public final void setFixedCost(double value)
```


يضبط تكلفة ثابتة للمهمة عندما تم حفظ الخط الأساسي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | تكلفة ثابتة للمهمة عندما تم حفظ الخط الأساسي. |

### setInterim(boolean value) {#setInterim-boolean-}
```
public final void setInterim(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان هذا خطًا أساسيًا مؤقتًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان هذا خطًا أساسيًا مؤقتًا. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


يضبط تاريخ بدء المهمة المجدول عندما تم حفظ الخط الأساسي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | تاريخ بدء المهمة المجدول عندما تم حفظ الخط الأساسي. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


يضبط مثيل TimephasedDataCollection لهذا الكائن. البيانات المرحلية المرتبطة بالخط الأساسي للمهمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | مثيل TimephasedDataCollection لهذا الكائن. |

