---
title: "WeekDay"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل يومًا من أيام الأسبوع يحدد إما الأيام العادية للأسبوع أو أيام الاستثناء في التقويم."
type: docs
weight: 352
url: /ar/java/com.aspose.tasks/weekday/
---

**Inheritance:**
java.lang.Object
```
public class WeekDay
```

يمثل يومًا من أيام الأسبوع يحدد إما الأيام العادية للأسبوع أو أيام الاستثناء في التقويم.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [WeekDay(int dayType)](#WeekDay-int-) | ينشئ مثيلاً جديدًا من الفئة [WeekDay](../../com.aspose.tasks/weekday) بالنوع اليوم المحدد. |
| [WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes)](#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--) | ينشئ مثيلاً جديدًا من الفئة [WeekDay](../../com.aspose.tasks/weekday) بالنوع اليوم المحدد وقائمة فترات العمل. |
| [WeekDay(int dayType, WorkingTime[] workingTimes)](#WeekDay-int-com.aspose.tasks.WorkingTime...-) | ينشئ مثيلاً جديدًا من الفئة [WeekDay](../../com.aspose.tasks/weekday) بالنوع اليوم المحدد وفترات العمل. |
| [WeekDay()](#WeekDay--) | يُنشئ مثيلاً جديدًا من الفئة [WeekDay](../../com.aspose.tasks/weekday). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [castToDayType(int dw)](#castToDayType-int-) | يحوّل [DayOfWeek](../../com.aspose.tasks/dayofweek) الخاص بـ .Net إلى `DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-)). |
| [createDefaultWorkingDay(int dayType)](#createDefaultWorkingDay-int-) | ينشئ يوم عمل افتراضي. |
| [deepClone()](#deepClone--) | يرجع نسخة عميقة من يوم الأسبوع. |
| [equals(Object obj)](#equals-java.lang.Object-) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| [getDayType()](#getDayType--) | يحصل على نوع اليوم. |
| [getDayWorking()](#getDayWorking--) | يحصل على قيمة تشير إلى ما إذا كان التاريخ أو نوع اليوم المحدد يعمل. |
| [getFromDate()](#getFromDate--) | يحصل على بداية وقت الاستثناء. |
| [getToDate()](#getToDate--) | يحصل على نهاية وقت الاستثناء. |
| [getWorkingTime()](#getWorkingTime--) | يرجع وقت العمل ليوم الأسبوع. |
| [getWorkingTimes()](#getWorkingTimes--) | يحصل على WorkingTimeCollection لهذا المثيل من WeekDay. |
| [hashCode()](#hashCode--) | يرجع قيمة رمز تجزئة للمثيل من الفئة [WeekDay](../../com.aspose.tasks/weekday). |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | يضبط قيمة تشير إلى ما إذا كان التاريخ أو نوع اليوم المحدد يعمل. |
| [setDefaultWorkingTime(WeekDay day)](#setDefaultWorkingTime-com.aspose.tasks.WeekDay-) | يضبط فترات الوقت الافتراضية ليوم الأسبوع المحدد. |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | يضبط بداية وقت الاستثناء. |
| [setToDate(Date value)](#setToDate-java.util.Date-) | يضبط نهاية وقت الاستثناء. |
### WeekDay(int dayType) {#WeekDay-int-}
```
public WeekDay(int dayType)
```


ينشئ مثيلاً جديدًا من الفئة [WeekDay](../../com.aspose.tasks/weekday) بالنوع اليوم المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| dayType | int | نوع اليوم المحدد. |

### WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes) {#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--}
```
public WeekDay(int dayType, List<WorkingTime> workingTimes)
```


ينشئ مثيلاً جديدًا من الفئة [WeekDay](../../com.aspose.tasks/weekday) بالنوع اليوم المحدد وقائمة فترات العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| dayType | int | نوع اليوم المحدد. |
| workingTimes | java.util.List&lt;com.aspose.tasks.WorkingTime&gt; | قائمة فترات وقت العمل. |

### WeekDay(int dayType, WorkingTime[] workingTimes) {#WeekDay-int-com.aspose.tasks.WorkingTime...-}
```
public WeekDay(int dayType, WorkingTime[] workingTimes)
```


ينشئ مثيلاً جديدًا من الفئة [WeekDay](../../com.aspose.tasks/weekday) بالنوع اليوم المحدد وفترات العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| dayType | int | نوع اليوم المحدد. |
| workingTimes | [WorkingTime\[\]](../../com.aspose.tasks/workingtime) | مصفوفة فترات وقت العمل. |

### WeekDay() {#WeekDay--}
```
public WeekDay()
```


يُنشئ مثيلاً جديدًا من الفئة [WeekDay](../../com.aspose.tasks/weekday).

### castToDayType(int dw) {#castToDayType-int-}
```
public static int castToDayType(int dw)
```


يحوّل [DayOfWeek](../../com.aspose.tasks/dayofweek) الخاص بـ .Net إلى `DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-)).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| dw | int | يوم الأسبوع للتحويل منه. |

**Returns:**
int - نوع يوم التحويل.
### createDefaultWorkingDay(int dayType) {#createDefaultWorkingDay-int-}
```
public static WeekDay createDefaultWorkingDay(int dayType)
```


ينشئ يوم عمل افتراضي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| dayType | int | نوع اليوم لإنشاء يوم عمل افتراضي منه. |

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - A default working day with working times 8-12 and 13-17.
### deepClone() {#deepClone--}
```
public final WeekDay deepClone()
```


يرجع نسخة عميقة من يوم الأسبوع.

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - Returns the deep copy of the week day.
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
منطقي - **True** إذا كان الكائن المحدد هو WeekDay يمتلك نفس قيم FromDate و ToDate و WorkingTimes مثل هذه الحالة؛ وإلا **false**.
### getDayType() {#getDayType--}
```
public final int getDayType()
```


يحصل على نوع اليوم.

**Returns:**
int - نوع اليوم.
### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


يحصل على قيمة تشير إلى ما إذا كان التاريخ أو نوع اليوم المحدد يعمل.

**Returns:**
منطقي - قيمة تشير إلى ما إذا كان التاريخ المحدد أو نوع اليوم يعمل.
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


يحصل على بداية وقت الاستثناء.

**Returns:**
java.util.Date - بداية وقت الاستثناء.
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


يحصل على نهاية وقت الاستثناء.

**Returns:**
java.util.Date - نهاية وقت الاستثناء.
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


يرجع وقت العمل ليوم الأسبوع.

**Returns:**
double - وقت العمل.
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


يحصل على WorkingTimeCollection لهذا الكائن WeekDay. مجموعة أوقات العمل التي تحدد الوقت الذي تم العمل فيه خلال يوم الأسبوع.

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - WorkingTimeCollection for this WeekDay instance.
### hashCode() {#hashCode--}
```
public int hashCode()
```


يرجع قيمة رمز تجزئة للمثيل من الفئة [WeekDay](../../com.aspose.tasks/weekday).

**Returns:**
عدد صحيح - يُعيد قيمة رمز التجزئة لهذا الكائن.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان التاريخ أو نوع اليوم المحدد يعمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان التاريخ المحدد أو نوع اليوم يعمل. |

### setDefaultWorkingTime(WeekDay day) {#setDefaultWorkingTime-com.aspose.tasks.WeekDay-}
```
public static void setDefaultWorkingTime(WeekDay day)
```


يضبط فترات الوقت الافتراضية ليوم الأسبوع المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| day | [WeekDay](../../com.aspose.tasks/weekday) | يوم الأسبوع لتعيين يوم العمل الافتراضي عليه. |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


يضبط بداية وقت الاستثناء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | بداية وقت الاستثناء. |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


يضبط نهاية وقت الاستثناء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | نهاية وقت الاستثناء. |

