---
title: "WorkingTime"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل وقت عمل خلال يوم من أيام الأسبوع."
type: docs
weight: 365
url: /ar/java/com.aspose.tasks/workingtime/
---

**Inheritance:**
java.lang.Object
```
public class WorkingTime
```

يمثل وقت عمل خلال يوم من أيام الأسبوع.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [WorkingTime(Date fromTime, Date toTime)](#WorkingTime-java.util.Date-java.util.Date-) | يُنشئ مثلاً جديدًا من الفئة [WorkingTime](../../com.aspose.tasks/workingtime) مع فترة مع أوقات البدء والانتهاء المحددة. |
| [WorkingTime(double fromTime, double toTime)](#WorkingTime-double-double-) | يُنشئ مثلاً جديدًا من الفئة [WorkingTime](../../com.aspose.tasks/workingtime) مع عنصر فترة مع أوقات البدء والانتهاء المحددة. |
| [WorkingTime(int fromHours, int toHours)](#WorkingTime-int-int-) | يُنشئ مثلاً جديدًا من الفئة [WorkingTime](../../com.aspose.tasks/workingtime) مع عنصر فترة مع أوقات البدء والانتهاء المحددة. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | يتحقق من أن الكائنات متساوية. |
| [getFrom()](#getFrom--) | يحصل على بداية وقت العمل. |
| [getTo()](#getTo--) | يحصل على نهاية وقت العمل. |
| [hashCode()](#hashCode--) | يرجع قيمة رمز التجزئة (hash code) للنسخة من الفئة [WorkingTime](../../com.aspose.tasks/workingtime). |
### WorkingTime(Date fromTime, Date toTime) {#WorkingTime-java.util.Date-java.util.Date-}
```
public WorkingTime(Date fromTime, Date toTime)
```


يُنشئ مثلاً جديدًا من الفئة [WorkingTime](../../com.aspose.tasks/workingtime) مع فترة مع أوقات البدء والانتهاء المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fromTime | java.util.Date | وقت بدء الفترة |
| toTime | java.util.Date | وقت انتهاء الفترة |

### WorkingTime(double fromTime, double toTime) {#WorkingTime-double-double-}
```
public WorkingTime(double fromTime, double toTime)
```


يُنشئ مثلاً جديدًا من الفئة [WorkingTime](../../com.aspose.tasks/workingtime) مع عنصر فترة مع أوقات البدء والانتهاء المحددة.

--------------------

&gt; ```
&gt; يمكن استخدام التحميل الزائد للمنشئ WorkingTime لتهيئة بدء ونهاية الفترة باستخدام TimeSpans:
&gt; ``````

 [C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fromTime | double | Interval's start time represented by double struct. |
| toTime | double | Interval's end time represented by double struct. |

### WorkingTime(int fromHours, int toHours) {#WorkingTime-int-int-}
```
public WorkingTime(int fromHours, int toHours)
```


Initializes a new instance of the [WorkingTime](../../com.aspose.tasks/workingtime) class with an interval item with the specified start and finish times.

--------------------

&gt; ```
&gt; The overload of WorkingTime ctor can be used to initialize interval's start and end using whole hours:
&gt; ``````

 [C#]
 var wt = new WorkingTime(9, 13);
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fromHours | int | وقت بدء الفترة ممثل برقم كامل للساعات (0-24). |
| toHours | int | وقت انتهاء الفترة ممثل برقم كامل للساعات (0-24). |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


يتحقق من أن الكائنات متساوية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | java.lang.Object | الكائن الثاني للمقارنة. |

**Returns:**
boolean - صحيح إذا كانت الكائنات متساوية، خطأ إذا لم تكن.
### getFrom() {#getFrom--}
```
public final Date getFrom()
```


يحصل على بداية وقت العمل.

**Returns:**
java.util.Date - بداية وقت العمل.
### getTo() {#getTo--}
```
public final Date getTo()
```


يحصل على نهاية وقت العمل.

**Returns:**
java.util.Date - نهاية وقت العمل.
### hashCode() {#hashCode--}
```
public int hashCode()
```


يرجع قيمة رمز التجزئة (hash code) للنسخة من الفئة [WorkingTime](../../com.aspose.tasks/workingtime).

**Returns:**
عدد صحيح - يُعيد قيمة رمز التجزئة لهذا الكائن.
