---
title: "TaskLink"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل ارتباطًا سلفيًا."
type: docs
weight: 295
url: /ar/java/com.aspose.tasks/tasklink/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public final class TaskLink implements System.IEquatable<TaskLink>
```

يمثل ارتباطًا سلفيًا.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(TaskLink other)](#equals-com.aspose.tasks.TaskLink-) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| [equals(Object obj)](#equals-java.lang.Object-) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| [getCrossProjectName()](#getCrossProjectName--) | يحصل على المشروع السابق الخارجي. |
| [getLagFormat()](#getLagFormat--) | يحصل على الصيغة للتعبير عن تنسيق التأخير. |
| [getLinkLag()](#getLinkLag--) | يحصل على التأخير بعُشر الدقيقة أو النسبة المئوية. |
| [getLinkLagTimeSpan()](#getLinkLagTimeSpan--) | يحصل على مدة التأخير، اعتمادًا على LagFormat. |
| [getLinkType()](#getLinkType--) | يحصل على نوع الرابط. |
| [getPredTask()](#getPredTask--) | يحصل على المهمة السابقة. |
| [getSuccTask()](#getSuccTask--) | يحصل على المهمة اللاحقة. |
| [hashCode()](#hashCode--) | يعيد قيمة رمز تجزئة للنسخة من الفئة [TaskLink](../../com.aspose.tasks/tasklink). |
| [isCrossProject()](#isCrossProject--) | يحصل على قيمة تشير إلى ما إذا كان السابق جزءًا من مشروع آخر. |
| [setCrossProject(boolean value)](#setCrossProject-boolean-) | يضبط قيمة تشير إلى ما إذا كان السابق جزءًا من مشروع آخر. |
| [setCrossProjectName(String value)](#setCrossProjectName-java.lang.String-) | يضبط المشروع السابق الخارجي. |
| [setLagFormat(byte value)](#setLagFormat-byte-) | يضبط الصيغة للتعبير عن تنسيق التأخير. |
| [setLinkLag(int value)](#setLinkLag-int-) | يضبط التأخير بعُشر الدقيقة أو النسبة المئوية. |
| [setLinkLagTimeSpan(double value)](#setLinkLagTimeSpan-double-) | يضبط مدة التأخير، اعتمادًا على LagFormat. |
| [setLinkType(int value)](#setLinkType-int-) | يضبط نوع الرابط. |
| [setPredTask(Task value)](#setPredTask-com.aspose.tasks.Task-) | يضبط المهمة السابقة. |
| [setSuccTask(Task value)](#setSuccTask-com.aspose.tasks.Task-) | يضبط المهمة اللاحقة. |
| [toString()](#toString--) | يعيد تمثيل السلسلة النصية لـ TaskLink. |
### equals(TaskLink other) {#equals-com.aspose.tasks.TaskLink-}
```
public final boolean equals(TaskLink other)
```


يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| other | [TaskLink](../../com.aspose.tasks/tasklink) | النسخة المحددة من الفئة [TaskLink](../../com.aspose.tasks/tasklink) للمقارنة مع هذه النسخة. |

**Returns:**
منطقي - **True** إذا كانت النسخة المحددة من الفئة [TaskLink](../../com.aspose.tasks/tasklink) لها نفس المهام السابقة واللاحقة كما في هذه النسخة؛ وإلا، **false**.
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
منطقي - **True** إذا كان الكائن المحدد هو TaskLink الذي له نفس السلف والتابع لهذا المثيل؛ وإلا، **false**.
### getCrossProjectName() {#getCrossProjectName--}
```
public final String getCrossProjectName()
```


يحصل على المشروع السابق الخارجي.

**Returns:**
java.lang.String - المشروع السلف الخارجي.
### getLagFormat() {#getLagFormat--}
```
public final byte getLagFormat()
```


يحصل على الصيغة للتعبير عن تنسيق التأخير.

**Returns:**
byte - الصيغة المستخدمة للتعبير عن تنسيق التأخير.
### getLinkLag() {#getLinkLag--}
```
public final int getLinkLag()
```


يحصل على التأخير بعُشر الدقيقة أو النسبة المئوية.

**Returns:**
int - التأخير بوحدات العشر من الدقيقة أو النسبة المئوية.
### getLinkLagTimeSpan() {#getLinkLagTimeSpan--}
```
public final double getLinkLagTimeSpan()
```


يحصل على مدة التأخير، اعتمادًا على LagFormat.

**Returns:**
double - مدة التأخير، حسب LagFormat.
### getLinkType() {#getLinkType--}
```
public final int getLinkType()
```


يحصل على نوع الرابط.

**Returns:**
int - نوع الرابط.
### getPredTask() {#getPredTask--}
```
public final Task getPredTask()
```


يحصل على المهمة السابقة.

**Returns:**
[Task](../../com.aspose.tasks/task) - the predecessor task.
### getSuccTask() {#getSuccTask--}
```
public final Task getSuccTask()
```


يحصل على المهمة اللاحقة.

**Returns:**
[Task](../../com.aspose.tasks/task) - the successor task.
### hashCode() {#hashCode--}
```
public int hashCode()
```


يعيد قيمة رمز تجزئة للنسخة من الفئة [TaskLink](../../com.aspose.tasks/tasklink).

**Returns:**
عدد صحيح - يُعيد قيمة رمز التجزئة لهذا الكائن.
### isCrossProject() {#isCrossProject--}
```
public final boolean isCrossProject()
```


يحصل على قيمة تشير إلى ما إذا كان السابق جزءًا من مشروع آخر.

**Returns:**
منطقي - قيمة تشير إلى ما إذا كان السلف جزءًا من مشروع آخر.
### setCrossProject(boolean value) {#setCrossProject-boolean-}
```
public final void setCrossProject(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان السابق جزءًا من مشروع آخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان السلف جزءًا من مشروع آخر. |

### setCrossProjectName(String value) {#setCrossProjectName-java.lang.String-}
```
public final void setCrossProjectName(String value)
```


يضبط المشروع السابق الخارجي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | المشروع السلف الخارجي. |

### setLagFormat(byte value) {#setLagFormat-byte-}
```
public final void setLagFormat(byte value)
```


يضبط الصيغة للتعبير عن تنسيق التأخير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | byte | الصيغة المستخدمة للتعبير عن تنسيق التأخير. |

### setLinkLag(int value) {#setLinkLag-int-}
```
public final void setLinkLag(int value)
```


يضبط التأخير بعُشر الدقيقة أو النسبة المئوية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | التأخير بوحدات العشر من الدقيقة أو النسبة المئوية. |

### setLinkLagTimeSpan(double value) {#setLinkLagTimeSpan-double-}
```
public final void setLinkLagTimeSpan(double value)
```


يضبط مدة التأخير، اعتمادًا على LagFormat.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | مدة التأخير، حسب LagFormat. |

### setLinkType(int value) {#setLinkType-int-}
```
public final void setLinkType(int value)
```


يضبط نوع الرابط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | نوع الرابط. |

### setPredTask(Task value) {#setPredTask-com.aspose.tasks.Task-}
```
public final void setPredTask(Task value)
```


يضبط المهمة السابقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | مهمة السلف. |

### setSuccTask(Task value) {#setSuccTask-com.aspose.tasks.Task-}
```
public final void setSuccTask(Task value)
```


يضبط المهمة اللاحقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | مهمة التابع. |

### toString() {#toString--}
```
public String toString()
```


يعيد تمثيل النص لسلسلة TaskLink. التفاصيل الدقيقة للتمثيل غير محددة وقد تتغير.

**Returns:**
java.lang.String - النص الذي يمثل كائن TaskLink.
