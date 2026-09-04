---
title: "AssignmentBaseline"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل Baseline لتعيين مورد."
type: docs
weight: 17
url: /ar/java/com.aspose.tasks/assignmentbaseline/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.Baseline](../../com.aspose.tasks/baseline)
```
public class AssignmentBaseline extends Baseline
```

يمثل Baseline لتعيين مورد.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [AssignmentBaseline()](#AssignmentBaseline--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [compareTo(AssignmentBaseline other)](#compareTo-com.aspose.tasks.AssignmentBaseline-) | تنفيذ واجهة IComparable. |
| [equals(AssignmentBaseline other)](#equals-com.aspose.tasks.AssignmentBaseline-) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن AssignmentBaseline المحدد. |
| [equals(Object obj)](#equals-java.lang.Object-) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| [getFinish()](#getFinish--) | يحصل على تاريخ الانتهاء المجدول لتعيين المورد عند حفظ الخط الأساسي. |
| [getStart()](#getStart--) | يحصل على تاريخ البدء المجدول لتعيين المورد عند حفظ الخط الأساسي. |
| [getTimephasedData()](#getTimephasedData--) | يحصل على مثيل [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) لهذا الكائن. |
| [hashCode()](#hashCode--) | يعيد قيمة رمز التجزئة لهذا AssignmentBaseline. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | يضبط تاريخ الانتهاء المجدول لتعيين المورد عند حفظ الخط الأساسي. |
| [setStart(Date value)](#setStart-java.util.Date-) | يضبط تاريخ البدء المجدول لتعيين المورد عند حفظ الخط الأساسي. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | يضبط مثيل [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) لهذا الكائن. |
### AssignmentBaseline() {#AssignmentBaseline--}
```
public AssignmentBaseline()
```


### compareTo(AssignmentBaseline other) {#compareTo-com.aspose.tasks.AssignmentBaseline-}
```
public final int compareTo(AssignmentBaseline other)
```


تنفيذ واجهة IComparable. يقارن هذا المثيل بالعنصر Baseline المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| other | [AssignmentBaseline](../../com.aspose.tasks/assignmentbaseline) | العنصر Baseline المحدد للمقارنة مع هذا المثيل. |

**Returns:**
int - يعيد -1 إذا كان هذا المثيل أصغر من العنصر المحدد، 1 إذا كان هذا المثيل أكبر من العنصر المحدد؛ وإلا يعيد 0
### equals(AssignmentBaseline other) {#equals-com.aspose.tasks.AssignmentBaseline-}
```
public final boolean equals(AssignmentBaseline other)
```


يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن AssignmentBaseline المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| other | [AssignmentBaseline](../../com.aspose.tasks/assignmentbaseline) | الكائن AssignmentBaseline المحدد للمقارنة مع هذه الحالة. |

**Returns:**
boolean - يعيد true إذا كانت هذه الحالة مساوية لكائن AssignmentBaseline المحدد؛ وإلا false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | java.lang.Object | العنصر المحدد للمقارنة مع هذا المثيل. |

**Returns:**
boolean - يعيد true إذا كان هذا المثيل مساويًا للعنصر المحدد؛ وإلا false.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


يحصل على تاريخ الانتهاء المجدول لتعيين المورد عند حفظ الخط الأساسي.

القيمة: تاريخ الانتهاء لتعيين المورد عند حفظ هذا الخط الأساسي.

**Returns:**
java.util.Date - تاريخ الانتهاء المجدول لتعيين المورد عند حفظ الخط الأساسي.
### getStart() {#getStart--}
```
public final Date getStart()
```


يحصل على تاريخ البدء المجدول لتعيين المورد عند حفظ الخط الأساسي.

القيمة: تاريخ البدء لتعيين المورد عند حفظ هذا الخط الأساسي.

**Returns:**
java.util.Date - تاريخ البدء المجدول لتعيين المورد عند حفظ الخط الأساسي.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


يحصل على مثيل [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) لهذا الكائن. البيانات الزمنية المرحلية المرتبطة بخط أساس تعيين المورد.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) instance for this object. Value: The collection of Time phased data associated with this baseline.
### hashCode() {#hashCode--}
```
public int hashCode()
```


يعيد قيمة رمز التجزئة لهذا AssignmentBaseline.

**Returns:**
عدد صحيح - يُعيد قيمة رمز التجزئة لهذا الكائن.
### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


يضبط تاريخ الانتهاء المجدول لتعيين المورد عند حفظ الخط الأساسي.

القيمة: تاريخ الانتهاء لتعيين المورد عند حفظ هذا الخط الأساسي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | تاريخ الانتهاء المجدول لتعيين المورد عند حفظ الخط الأساسي. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


يضبط تاريخ البدء المجدول لتعيين المورد عند حفظ الخط الأساسي.

القيمة: تاريخ البدء لتعيين المورد عند حفظ هذا الخط الأساسي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | تاريخ البدء المجدول لتعيين المورد عند حفظ الخط الأساسي. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


يضبط مثيل [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) لهذا الكائن. البيانات الزمنية المرحلية المرتبطة بخط أساس تعيين المورد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | مثيل [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) لهذا الكائن. |

