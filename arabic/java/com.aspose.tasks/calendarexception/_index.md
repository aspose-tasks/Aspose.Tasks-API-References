---
title: "CalendarException"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل فترات زمنية استثنائية في تقويم."
type: docs
weight: 43
url: /ar/java/com.aspose.tasks/calendarexception/
---

**Inheritance:**
java.lang.Object
```
public final class CalendarException
```

يمثل فترات زمنية استثنائية في تقويم.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [CalendarException()](#CalendarException--) | يُهيئ نسخة جديدة من الفئة [CalendarException](../../com.aspose.tasks/calendarexception). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [checkException(Date dt)](#checkException-java.util.Date-) | يرجع true إذا كانت النسخة المحددة من هيكل java.util.Date هي يوم الاستثناء. |
| [delete()](#delete--) | يحذف نسخة الاستثناء من كائن التقويم الأب CalendarExceptionCollection. |
| [getDayWorking()](#getDayWorking--) | يحصل على قيمة تشير إلى ما إذا كان التاريخ أو نوع اليوم المحدد يعمل. |
| [getDaysOfWeek()](#getDaysOfWeek--) | يحصل على DayTypeCollection لهذا الكائن. |
| [getEnteredByOccurrences()](#getEnteredByOccurrences--) | يحصل على قيمة تشير إلى ما إذا كان نطاق التكرار معرفًا بإدخال عدد من التكرارات. |
| [getExceptionDates()](#getExceptionDates--) | يرجع التواريخ التي يكون فيها استثناء التقويم قابلاً للتطبيق. |
| [getFromDate()](#getFromDate--) | يحصل على بداية وقت الاستثناء. |
| [getMonth()](#getMonth--) | يحصل على الشهر الذي تم جدولة تكرار الاستثناء له. |
| [getMonthDay()](#getMonthDay--) | يحصل على اليوم من الشهر الذي تم جدولة تكرار الاستثناء له. |
| [getMonthItem()](#getMonthItem--) | يحصل على عنصر الشهر الذي تم جدولة تكرار الاستثناء له. |
| [getMonthPosition()](#getMonthPosition--) | يحصل على موضع عنصر الشهر داخل شهر. |
| [getName()](#getName--) | يحصل على اسم الاستثناء. |
| [getOccurrences()](#getOccurrences--) | يحصل على عدد التكرارات التي يكون فيها استثناء التقويم صالحًا. |
| [getParentCalendar()](#getParentCalendar--) | يحصل على التقويم الأب لهذا الكائن. |
| [getPeriod()](#getPeriod--) | يحصل على فترة تكرار الاستثناء. |
| [getToDate()](#getToDate--) | يحصل على نهاية وقت الاستثناء. |
| [getType()](#getType--) | يحصل على نوع الاستثناء. |
| [getWorkingTime()](#getWorkingTime--) | يرجع وقت العمل لاستثناء التقويم. |
| [getWorkingTimes()](#getWorkingTimes--) | يحصل على كائن WorkingTimeCollection. |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | يضبط قيمة تشير إلى ما إذا كان التاريخ أو نوع اليوم المحدد يعمل. |
| [setEnteredByOccurrences(boolean value)](#setEnteredByOccurrences-boolean-) | يضبط قيمة تشير إلى ما إذا كان نطاق التكرار معرفًا بإدخال عدد من التكرارات. |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | يضبط بداية وقت الاستثناء. |
| [setMonth(int value)](#setMonth-int-) | يضبط الشهر الذي يتم جدولة تكرار الاستثناء له. |
| [setMonthDay(int value)](#setMonthDay-int-) | يضبط يوم الشهر الذي يتم جدولة تكرار الاستثناء فيه. |
| [setMonthItem(int value)](#setMonthItem-int-) | يضبط عنصر الشهر الذي يتم جدولة تكرار الاستثناء له. |
| [setMonthPosition(int value)](#setMonthPosition-int-) | يضبط موضع عنصر الشهر داخل الشهر. |
| [setName(String value)](#setName-java.lang.String-) | يضبط اسم الاستثناء. |
| [setOccurrences(int value)](#setOccurrences-int-) | يضبط عدد مرات التكرار التي يكون فيها استثناء التقويم صالحًا. |
| [setPeriod(int value)](#setPeriod-int-) | يضبط فترة تكرار الاستثناء. |
| [setToDate(Date value)](#setToDate-java.util.Date-) | يضبط نهاية وقت الاستثناء. |
| [setType(int value)](#setType-int-) | يضبط نوع الاستثناء. |
| [setWorkingTimes(WorkingTimeCollection value)](#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-) | يضبط كائن WorkingTimeCollection. |
### CalendarException() {#CalendarException--}
```
public CalendarException()
```


يُهيئ نسخة جديدة من الفئة [CalendarException](../../com.aspose.tasks/calendarexception).

### checkException(Date dt) {#checkException-java.util.Date-}
```
public final boolean checkException(Date dt)
```


يرجع true إذا كانت النسخة المحددة من هيكل java.util.Date هي يوم الاستثناء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| dt | java.util.Date | العينة المحددة من بنية java.util.Date. |

**Returns:**
boolean - يُرجع true إذا كانت قيمة java.util.Date هي يوم الاستثناء؛ وإلا، false.
### delete() {#delete--}
```
public final void delete()
```


يحذف نسخة الاستثناء من كائن التقويم الأب CalendarExceptionCollection.

### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


يحصل على قيمة تشير إلى ما إذا كان التاريخ أو نوع اليوم المحدد يعمل.

**Returns:**
منطقي - قيمة تشير إلى ما إذا كان التاريخ المحدد أو نوع اليوم يعمل.
### getDaysOfWeek() {#getDaysOfWeek--}
```
public final DayTypeCollection getDaysOfWeek()
```


يحصل على DayTypeCollection لهذا الكائن. أيام الأسبوع التي يكون فيها الاستثناء صالحًا.

**Returns:**
[DayTypeCollection](../../com.aspose.tasks/daytypecollection) - the DayTypeCollection for this object.
### getEnteredByOccurrences() {#getEnteredByOccurrences--}
```
public final boolean getEnteredByOccurrences()
```


يحصل على قيمة تشير إلى ما إذا كان نطاق التكرار معرفًا بإدخال عدد مرات التكرار. False يحدد أن نطاق التكرار معرف بإدخال تاريخ الانتهاء.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان نطاق التكرار معرفًا بإدخال عدد مرات التكرار.
### getExceptionDates() {#getExceptionDates--}
```
public final Iterable<Date> getExceptionDates()
```


يرجع التواريخ التي يكون فيها استثناء التقويم قابلاً للتطبيق.

**Returns:**
java.lang.Iterable&lt;java.util.Date&gt; - التواريخ التي ينطبق عليها استثناء التقويم.
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


يحصل على بداية وقت الاستثناء.

**Returns:**
java.util.Date - بداية وقت الاستثناء.
### getMonth() {#getMonth--}
```
public final int getMonth()
```


يحصل على الشهر الذي تم جدولة تكرار الاستثناء له.

**Returns:**
int - الشهر الذي يتم جدولة تكرار الاستثناء له.
### getMonthDay() {#getMonthDay--}
```
public final int getMonthDay()
```


يحصل على اليوم من الشهر الذي تم جدولة تكرار الاستثناء له.

**Returns:**
int - يوم الشهر الذي يتم جدولة تكرار الاستثناء فيه.
### getMonthItem() {#getMonthItem--}
```
public final int getMonthItem()
```


يحصل على عنصر الشهر الذي تم جدولة تكرار الاستثناء له.

**Returns:**
int - عنصر الشهر الذي يتم جدولة تكرار الاستثناء له.
### getMonthPosition() {#getMonthPosition--}
```
public final int getMonthPosition()
```


يحصل على موضع عنصر الشهر داخل شهر.

**Returns:**
int - موضع عنصر الشهر داخل الشهر.
### getName() {#getName--}
```
public final String getName()
```


يحصل على اسم الاستثناء.

**Returns:**
java.lang.String - اسم الاستثناء.
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


يحصل على عدد التكرارات التي يكون فيها استثناء التقويم صالحًا.

**Returns:**
int - عدد مرات التكرار التي يكون فيها استثناء التقويم صالحًا.
### getParentCalendar() {#getParentCalendar--}
```
public final Calendar getParentCalendar()
```


يحصل على التقويم الأب لهذا الكائن.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - the parent calendar for this object.
### getPeriod() {#getPeriod--}
```
public final int getPeriod()
```


يحصل على فترة تكرار الاستثناء.

**Returns:**
int - فترة تكرار الاستثناء.
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


يحصل على نهاية وقت الاستثناء.

**Returns:**
java.util.Date - نهاية وقت الاستثناء.
### getType() {#getType--}
```
public final int getType()
```


يحصل على نوع الاستثناء.

**Returns:**
int - نوع الاستثناء.
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


يرجع وقت العمل لاستثناء التقويم.

**Returns:**
double - يُرجِع وقت العمل لهذا الاستثناء في التقويم.
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


يحصل على كائن WorkingTimeCollection. مجموعة أوقات العمل التي تحدد الوقت العامل في يوم الأسبوع.

--------------------

يجب أن يكون هناك وقت عمل واحد على الأقل، ولا يمكن أن يكون أكثر من خمسة.

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - the WorkingTimeCollection object.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان التاريخ أو نوع اليوم المحدد يعمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان التاريخ المحدد أو نوع اليوم يعمل. |

### setEnteredByOccurrences(boolean value) {#setEnteredByOccurrences-boolean-}
```
public final void setEnteredByOccurrences(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان نطاق التكرار معرفًا بإدخال عدد مرات التكرار. القيمة False تعني أن نطاق التكرار معرف بإدخال تاريخ الانتهاء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان نطاق التكرار معرفًا بإدخال عدد مرات التكرار. |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


يضبط بداية وقت الاستثناء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | بداية وقت الاستثناء. |

### setMonth(int value) {#setMonth-int-}
```
public final void setMonth(int value)
```


يضبط الشهر الذي يتم جدولة تكرار الاستثناء له.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | الشهر الذي يُجدول فيه تكرار الاستثناء. |

### setMonthDay(int value) {#setMonthDay-int-}
```
public final void setMonthDay(int value)
```


يضبط يوم الشهر الذي يتم جدولة تكرار الاستثناء فيه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | اليوم من الشهر الذي يُجدول فيه تكرار الاستثناء. |

### setMonthItem(int value) {#setMonthItem-int-}
```
public final void setMonthItem(int value)
```


يضبط عنصر الشهر الذي يتم جدولة تكرار الاستثناء له.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | عنصر الشهر الذي يُجدول فيه تكرار الاستثناء. |

### setMonthPosition(int value) {#setMonthPosition-int-}
```
public final void setMonthPosition(int value)
```


يضبط موضع عنصر الشهر داخل الشهر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | موضع عنصر الشهر داخل الشهر. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


يضبط اسم الاستثناء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | اسم الاستثناء. |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


يضبط عدد مرات التكرار التي يكون فيها استثناء التقويم صالحًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | عدد مرات التكرار التي يكون فيها استثناء التقويم صالحًا. |

### setPeriod(int value) {#setPeriod-int-}
```
public final void setPeriod(int value)
```


يضبط فترة تكرار الاستثناء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | فترة تكرار الاستثناء. |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


يضبط نهاية وقت الاستثناء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | نهاية وقت الاستثناء. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


يضبط نوع الاستثناء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | نوع الاستثناء. |

### setWorkingTimes(WorkingTimeCollection value) {#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-}
```
public final void setWorkingTimes(WorkingTimeCollection value)
```


يضبط كائن WorkingTimeCollection. مجموعة أوقات العمل التي تحدد الوقت العامل في يوم الأسبوع.

--------------------

يجب أن يكون هناك وقت عمل واحد على الأقل، ولا يمكن أن يكون أكثر من خمسة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) | كائن WorkingTimeCollection. |

