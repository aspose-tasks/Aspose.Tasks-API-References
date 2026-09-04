---
title: "ICalendar"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل تجريدًا للتقويم يمكن استخدامه لحسابات مختلفة للتواريخ والمدة."
type: docs
weight: 376
url: /ar/java/com.aspose.tasks/icalendar/
---
```
public interface ICalendar
```

يمثل تجريدًا للتقويم يمكن استخدامه لحسابات مختلفة للتواريخ والمدة.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getFinishDateByStartAndWork(Date start, Duration work)](#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-) | يحسب التاريخ الذي سينقضي فيه مقدار وقت العمل المحدد وفقًا للتقويم. |
| [getFinishDateByStartAndWork(Date start, double work)](#getFinishDateByStartAndWork-java.util.Date-double-) | يحسب التاريخ الذي سينقضي فيه مقدار وقت العمل المحدد وفقًا للتقويم. |
| [getNextWorkingDayStart(Date date)](#getNextWorkingDayStart-java.util.Date-) | يحسب بداية اليوم العملي التالي للتاريخ المحدد. |
| [getPreviousWorkingDayEnd(Date date)](#getPreviousWorkingDayEnd-java.util.Date-) | يحسب نهاية تاريخ العمل السابق من التاريخ المحدد. |
| [getStartDateFromFinishAndDuration(Date finish, Duration duration)](#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-) | يعيد تاريخ البدء بناءً على تاريخ الانتهاء المحدد والمدة. |
| [getStartDateFromFinishAndDuration(Date finish, double duration)](#getStartDateFromFinishAndDuration-java.util.Date-double-) | يعيد تاريخ البدء بناءً على تاريخ الانتهاء المحدد والمدة. |
| [getTaskFinishDateFromDuration(Task task, double duration)](#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-) | يحسب تاريخ ووقت انتهاء المهمة من تاريخ بدايتها، الأجزاء المقسمة ومدة العمل. |
| [getWorkStart(Date date)](#getWorkStart-java.util.Date-) | يحسب بداية وقت العمل التالي بدءًا من التاريخ والوقت المحددين. |
| [getWorkingHours(Date dt)](#getWorkingHours-java.util.Date-) | يعيد عدد ساعات العمل في التاريخ المحدد. |
| [getWorkingHours(Date start, Date finish)](#getWorkingHours-java.util.Date-java.util.Date-) | إرجاع WorkUnit - بدء، انتهاء ومدة ساعات العمل للفترة الزمنية المحددة. |
| [getWorkingHoursTimeSpan(Date start, Date finish)](#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-) | يعيد عدد ساعات العمل بين التواريخ المحددة. |
| [getWorkingTimes(Date dt)](#getWorkingTimes-java.util.Date-) | يعيد [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) لأوقات العمل للتاريخ المحدد. |
| [isDayWorking(Date dt)](#isDayWorking-java.util.Date-) | يحدد ما إذا كان اليوم المحدد يوم عمل وفقًا للتقويم. |
| [isEmpty()](#isEmpty--) | يعيد ما إذا كان التقويم لا يحتوي على ساعات عمل معرفة. |
### getFinishDateByStartAndWork(Date start, Duration work) {#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getFinishDateByStartAndWork(Date start, Duration work)
```


يحسب التاريخ الذي سينقضي فيه مقدار وقت العمل المحدد وفقًا للتقويم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| بدء | java.util.Date | تاريخ البدء. |
| work | [Duration](../../com.aspose.tasks/duration) | مدة العمل. |

**Returns:**
java.util.Date - تاريخ الانتهاء.
### getFinishDateByStartAndWork(Date start, double work) {#getFinishDateByStartAndWork-java.util.Date-double-}
```
public abstract Date getFinishDateByStartAndWork(Date start, double work)
```


يحسب التاريخ الذي سينقضي فيه مقدار وقت العمل المحدد وفقًا للتقويم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| بدء | java.util.Date | تاريخ البدء. |
| عمل | double | مدة العمل. |

**Returns:**
java.util.Date - تاريخ الانتهاء.
### getNextWorkingDayStart(Date date) {#getNextWorkingDayStart-java.util.Date-}
```
public abstract Date getNextWorkingDayStart(Date date)
```


يحسب بداية اليوم العملي التالي للتاريخ المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| التاريخ | java.util.Date | التاريخ للحصول على بداية اليوم العمل التالي. |

**Returns:**
java.util.Date - بداية اليوم العمل التالي System.DateTime.
### getPreviousWorkingDayEnd(Date date) {#getPreviousWorkingDayEnd-java.util.Date-}
```
public abstract Date getPreviousWorkingDayEnd(Date date)
```


يحسب نهاية تاريخ العمل السابق من التاريخ المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| التاريخ | java.util.Date | التاريخ لحساب نهاية اليوم العمل السابق. |

**Returns:**
java.util.Date - نهاية اليوم العمل السابق
### getStartDateFromFinishAndDuration(Date finish, Duration duration) {#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, Duration duration)
```


يعيد تاريخ البدء بناءً على تاريخ الانتهاء المحدد والمدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الانتهاء | java.util.Date | تاريخ الانتهاء المحدد. |
| duration | [Duration](../../com.aspose.tasks/duration) | المدة المحددة. |

**Returns:**
java.util.Date - تاريخ البدء المحسوب.
### getStartDateFromFinishAndDuration(Date finish, double duration) {#getStartDateFromFinishAndDuration-java.util.Date-double-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, double duration)
```


يعيد تاريخ البدء بناءً على تاريخ الانتهاء المحدد والمدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الانتهاء | java.util.Date | تاريخ الانتهاء المحدد. |
| المدة | double | المدة المحددة. |

**Returns:**
java.util.Date - تاريخ البدء المحسوب.
### getTaskFinishDateFromDuration(Task task, double duration) {#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-}
```
public abstract Date getTaskFinishDateFromDuration(Task task, double duration)
```


يحسب تاريخ ووقت انتهاء المهمة من تاريخ بدايتها، الأجزاء المقسمة ومدة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | المهمة لحساب تاريخ الانتهاء لها. |
|  | المدة | double | المدة التي سيتم حسابها. |

يعيد DateTime.MinValue إذا كانت المهمة ملخصًا، أو null أو لم يتم تعيين تاريخ البدء الخاص بها. |

**Returns:**
java.util.Date - تاريخ انتهاء المهمة للتاريخ البدء المحدد والمدة.
### getWorkStart(Date date) {#getWorkStart-java.util.Date-}
```
public abstract Date getWorkStart(Date date)
```


يحسب بداية وقت العمل التالي بدءًا من التاريخ والوقت المحددين.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| التاريخ | java.util.Date | التاريخ والوقت. |

**Returns:**
java.util.Date - أقرب بداية وقت عمل.
### getWorkingHours(Date dt) {#getWorkingHours-java.util.Date-}
```
public abstract double getWorkingHours(Date dt)
```


يعيد عدد ساعات العمل في التاريخ المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| dt | java.util.Date | التاريخ للحصول على ساعات العمل. |

**Returns:**
double - ساعات العمل في التاريخ المحدد.
### getWorkingHours(Date start, Date finish) {#getWorkingHours-java.util.Date-java.util.Date-}
```
public abstract WorkUnit getWorkingHours(Date start, Date finish)
```


إرجاع WorkUnit - بدء، انتهاء ومدة ساعات العمل للفترة الزمنية المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| بدء | java.util.Date | تاريخ البدء للفترة. |
| الانتهاء | java.util.Date | تاريخ الانتهاء للفترة. |

**Returns:**
[WorkUnit](../../com.aspose.tasks/workunit) - Instance of [WorkUnit](../../com.aspose.tasks/workunit) class containing Start, Finish and Duration of working hours.
### getWorkingHoursTimeSpan(Date start, Date finish) {#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-}
```
public abstract double getWorkingHoursTimeSpan(Date start, Date finish)
```


يعيد عدد ساعات العمل بين التواريخ المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| بدء | java.util.Date | تاريخ البدء للفترة. |
| الانتهاء | java.util.Date | تاريخ الانتهاء للفترة. |

**Returns:**
double - كمية ساعات العمل وفقًا لنسخة التقويم.
### getWorkingTimes(Date dt) {#getWorkingTimes-java.util.Date-}
```
public abstract WorkingTimeCollection getWorkingTimes(Date dt)
```


يعيد [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) لأوقات العمل للتاريخ المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| dt | java.util.Date | التاريخ للحصول على أوقات العمل. |

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - Collection of [WorkingTime](../../com.aspose.tasks/workingtime) instances.
### isDayWorking(Date dt) {#isDayWorking-java.util.Date-}
```
public abstract boolean isDayWorking(Date dt)
```


يحدد ما إذا كان اليوم المحدد يوم عمل وفقًا للتقويم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| dt | java.util.Date | التاريخ للتحقق مما إذا كان اليوم عملًا. |

**Returns:**
boolean - صحيح إذا كان اليوم يوم عمل.
### isEmpty() {#isEmpty--}
```
public abstract boolean isEmpty()
```


يعيد ما إذا كان التقويم لا يحتوي على ساعات عمل معرفة.

**Returns:**
boolean - صحيح إذا لم يكن للتقويم ساعات عمل معرفة.
