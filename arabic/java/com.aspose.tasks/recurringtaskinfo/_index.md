---
title: "RecurringTaskInfo"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل تفاصيل مهمة متكررة في مشروع."
type: docs
weight: 244
url: /ar/java/com.aspose.tasks/recurringtaskinfo/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskInfo
```

يمثل تفاصيل مهمة متكررة في مشروع.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getDailyRepetitions()](#getDailyRepetitions--) | يحصل على عدد التكرارات لنمط التكرار اليومي. |
| [getDailyUseWorkdays()](#getDailyUseWorkdays--) | يحصل على قيمة تشير إلى ما إذا كان يجب استخدام أيام العمل لنمط التكرار اليومي. |
| [getDuration()](#getDuration--) | يحصل على المدة لحدوث واحد للمهمة المتكررة. |
| [getEndDate()](#getEndDate--) | يحصل على التاريخ لإنتهاء التكرارات. |
| [getMonthlyDay()](#getMonthlyDay--) | يحصل على عدد الأيام لنمط التكرار الشهري. |
| [getMonthlyOrdinalDay()](#getMonthlyOrdinalDay--) | يحصل على يوم من نمط التكرار الشهري عند استخدام اليوم الترتيبي. |
| [getMonthlyOrdinalNumber()](#getMonthlyOrdinalNumber--) | يحصل على رقم ترتيبي لنمط التكرار الشهري. |
| [getMonthlyOrdinalRepetitions()](#getMonthlyOrdinalRepetitions--) | يحصل على عدد التكرارات لنمط التكرار الشهري عند استخدام اليوم الترتيبي. |
| [getMonthlyRepetitions()](#getMonthlyRepetitions--) | يحصل على عدد التكرارات لنمط التكرار الشهري. |
| [getMonthlyUseOrdinalDay()](#getMonthlyUseOrdinalDay--) | يحصل على قيمة تشير إلى ما إذا كان يجب استخدام اليوم الترتيبي لنمط التكرار الشهري. |
| [getOccurrences()](#getOccurrences--) | يحصل على عدد التكرارات للمهمة المتكررة. |
| [getRecurrencePattern()](#getRecurrencePattern--) | يحصل على نمط التكرار للمهمة المتكررة. |
| [getStartDate()](#getStartDate--) | يحصل على التاريخ لبدء التكرارات. |
| [getTask()](#getTask--) | يحصل على مهمة الأصل لهذه الحالة من الفئة [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo). |
| [getUseEndDate()](#getUseEndDate--) | يحصل على قيمة تشير إلى ما إذا كان يجب استخدام تاريخ الانتهاء أو عدد التكرارات للمهمة المتكررة. |
| [getWeeklyDays()](#getWeeklyDays--) | يحصل على مجموعة الأيام المستخدمة في نمط التكرار الأسبوعي. |
| [getWeeklyRepetitions()](#getWeeklyRepetitions--) | يحصل على عدد التكرارات لنمط التكرار الأسبوعي. |
| [getYearlyDate()](#getYearlyDate--) | يحصل على تاريخ لنمط التكرار السنوي. |
| [getYearlyOrdinalDay()](#getYearlyOrdinalDay--) | يحصل على يوم الأسبوع لنمط التكرار السنوي عند استخدام اليوم الترتيبي. |
| [getYearlyOrdinalMonth()](#getYearlyOrdinalMonth--) | يحصل على شهر لنمط التكرار السنوي عند استخدام اليوم الترتيبي. |
| [getYearlyOrdinalNumber()](#getYearlyOrdinalNumber--) | يحصل على رقم ترتيبي لنمط التكرار السنوي. |
| [getYearlyUseOrdinalDay()](#getYearlyUseOrdinalDay--) | يحصل على قيمة تشير إلى ما إذا كان يجب استخدام اليوم الترتيبي لنمط التكرار السنوي. |
| [setDailyRepetitions(int value)](#setDailyRepetitions-int-) | يضبط عدد التكرارات لنمط التكرار اليومي. |
| [setDailyUseWorkdays(boolean value)](#setDailyUseWorkdays-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب استخدام أيام العمل لنمط التكرار اليومي. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | يضبط المدة لحدوث واحد للمهمة المتكررة. |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | يضبط التاريخ لنهاية الأحداث. |
| [setMonthlyDay(int value)](#setMonthlyDay-int-) | يضبط عدد الأيام لنمط التكرار الشهري. |
| [setMonthlyOrdinalDay(int value)](#setMonthlyOrdinalDay-int-) | يضبط يومًا لنمط التكرار الشهري عند استخدام اليوم الترتيبي. |
| [setMonthlyOrdinalNumber(int value)](#setMonthlyOrdinalNumber-int-) | يضبط رقمًا ترتيبيًا لنمط التكرار الشهري. |
| [setMonthlyOrdinalRepetitions(int value)](#setMonthlyOrdinalRepetitions-int-) | يضبط عدد التكرارات لنمط التكرار الشهري عند استخدام اليوم الترتيبي. |
| [setMonthlyRepetitions(int value)](#setMonthlyRepetitions-int-) | يضبط عدد التكرارات لنمط التكرار الشهري. |
| [setMonthlyUseOrdinalDay(boolean value)](#setMonthlyUseOrdinalDay-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب استخدام اليوم الترتيبي لنمط التكرار الشهري. |
| [setOccurrences(int value)](#setOccurrences-int-) | يضبط عدد مرات حدوث المهمة المتكررة. |
| [setRecurrencePattern(int value)](#setRecurrencePattern-int-) | يضبط نمط التكرار للمهمة المتكررة. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | يضبط التاريخ لبدء الأحداث. |
| [setUseEndDate(boolean value)](#setUseEndDate-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب استخدام تاريخ الانتهاء أو عدد مرات حدوث المهمة المتكررة. |
| [setWeeklyDays(int value)](#setWeeklyDays-int-) | يضبط مجموعة الأيام المستخدمة في نمط التكرار الأسبوعي. |
| [setWeeklyRepetitions(int value)](#setWeeklyRepetitions-int-) | يضبط عدد التكرارات لنمط التكرار الأسبوعي. |
| [setYearlyDate(Date value)](#setYearlyDate-java.util.Date-) | يضبط التاريخ لنمط التكرار السنوي. |
| [setYearlyOrdinalDay(int value)](#setYearlyOrdinalDay-int-) | يضبط يوم الأسبوع لنمط التكرار السنوي عند استخدام اليوم الترتيبي. |
| [setYearlyOrdinalMonth(int value)](#setYearlyOrdinalMonth-int-) | يضبط شهرًا لنمط التكرار السنوي عند استخدام اليوم الترتيبي. |
| [setYearlyOrdinalNumber(int value)](#setYearlyOrdinalNumber-int-) | يضبط رقمًا ترتيبيًا لنمط التكرار السنوي. |
| [setYearlyUseOrdinalDay(boolean value)](#setYearlyUseOrdinalDay-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب استخدام اليوم الترتيبي لنمط التكرار السنوي. |
### getDailyRepetitions() {#getDailyRepetitions--}
```
public final int getDailyRepetitions()
```


يحصل على عدد التكرارات لنمط التكرار اليومي.

**Returns:**
int - عدد التكرارات لنمط التكرار اليومي.
### getDailyUseWorkdays() {#getDailyUseWorkdays--}
```
public final boolean getDailyUseWorkdays()
```


يحصل على قيمة تشير إلى ما إذا كان يجب استخدام أيام العمل لنمط التكرار اليومي.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب استخدام أيام العمل لنمط التكرار اليومي.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


يحصل على المدة لحدوث واحد للمهمة المتكررة.

--------------------

مثال على فئة `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)).

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration for one occurrence of the recurring task.
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


يحصل على التاريخ لإنتهاء التكرارات.

**Returns:**
java.util.Date - التاريخ الذي تنتهي عنده التكرارات.
### getMonthlyDay() {#getMonthlyDay--}
```
public final int getMonthlyDay()
```


يحصل على عدد الأيام لنمط التكرار الشهري.

**Returns:**
int - عدد الأيام لنمط التكرار الشهري.
### getMonthlyOrdinalDay() {#getMonthlyOrdinalDay--}
```
public final int getMonthlyOrdinalDay()
```


يحصل على يوم من نمط التكرار الشهري عند استخدام اليوم الترتيبي.

--------------------

يمكن أن تكون واحدة من قيم تعداد [DayOfWeek](../../com.aspose.tasks/dayofweek).

**Returns:**
int - يوم من نمط التكرار الشهري عند استخدام اليوم الترتيبي.
### getMonthlyOrdinalNumber() {#getMonthlyOrdinalNumber--}
```
public final int getMonthlyOrdinalNumber()
```


يحصل على رقم ترتيبي لنمط التكرار الشهري.

--------------------

يمكن أن تكون واحدة من قيم تعداد [OrdinalNumber](../../com.aspose.tasks/ordinalnumber).

**Returns:**
int - رقم ترتيبي لنمط التكرار الشهري.
### getMonthlyOrdinalRepetitions() {#getMonthlyOrdinalRepetitions--}
```
public final int getMonthlyOrdinalRepetitions()
```


يحصل على عدد التكرارات لنمط التكرار الشهري عند استخدام اليوم الترتيبي.

**Returns:**
int - عدد التكرارات لنمط التكرار الشهري عند استخدام اليوم الترتيبي.
### getMonthlyRepetitions() {#getMonthlyRepetitions--}
```
public final int getMonthlyRepetitions()
```


يحصل على عدد التكرارات لنمط التكرار الشهري.

**Returns:**
int - عدد التكرارات لنمط التكرار الشهري.
### getMonthlyUseOrdinalDay() {#getMonthlyUseOrdinalDay--}
```
public final boolean getMonthlyUseOrdinalDay()
```


يحصل على قيمة تشير إلى ما إذا كان يجب استخدام اليوم الترتيبي لنمط التكرار الشهري.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب استخدام اليوم الترتيبي لنمط التكرار الشهري.
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


يحصل على عدد التكرارات للمهمة المتكررة.

**Returns:**
int - عدد مرات حدوث المهمة المتكررة.
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final int getRecurrencePattern()
```


يحصل على نمط التكرار للمهمة المتكررة.

--------------------

يمكن أن تكون واحدة من قيم تعداد `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose.tasks/recurringtaskinfo\#setRecurrencePattern-int-)).

**Returns:**
int - نمط تكرار للمهمة المتكررة.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


يحصل على التاريخ لبدء التكرارات.

**Returns:**
java.util.Date - التاريخ الذي تبدأ عنده التكرارات.
### getTask() {#getTask--}
```
public final Task getTask()
```


يحصل على مهمة الأصل لهذه الحالة من الفئة [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo).

**Returns:**
[Task](../../com.aspose.tasks/task) - the parent task of this instance of [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) class.
### getUseEndDate() {#getUseEndDate--}
```
public final boolean getUseEndDate()
```


يحصل على قيمة تشير إلى ما إذا كان يجب استخدام تاريخ الانتهاء أو عدد التكرارات للمهمة المتكررة.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب استخدام تاريخ الانتهاء أو عدد التكرارات للمهمة المتكررة.
### getWeeklyDays() {#getWeeklyDays--}
```
public final int getWeeklyDays()
```


يحصل على مجموعة الأيام المستخدمة في نمط التكرار الأسبوعي.

--------------------

**Returns:**
int - مجموعة الأيام المستخدمة في نمط التكرار الأسبوعي.
### getWeeklyRepetitions() {#getWeeklyRepetitions--}
```
public final int getWeeklyRepetitions()
```


يحصل على عدد التكرارات لنمط التكرار الأسبوعي.

**Returns:**
int - عدد التكرارات لنمط التكرار الأسبوعي.
### getYearlyDate() {#getYearlyDate--}
```
public final Date getYearlyDate()
```


يحصل على تاريخ لنمط التكرار السنوي.

**Returns:**
java.util.Date - تاريخ لنمط التكرار السنوي.
### getYearlyOrdinalDay() {#getYearlyOrdinalDay--}
```
public final int getYearlyOrdinalDay()
```


يحصل على يوم الأسبوع لنمط التكرار السنوي عند استخدام اليوم الترتيبي.

--------------------

يمكن أن تكون واحدة من قيم تعداد [DayOfWeek](../../com.aspose.tasks/dayofweek).

**Returns:**
int - يوم أسبوعي لنمط التكرار السنوي عند استخدام اليوم الترتيبي.
### getYearlyOrdinalMonth() {#getYearlyOrdinalMonth--}
```
public final int getYearlyOrdinalMonth()
```


يحصل على شهر لنمط التكرار السنوي عند استخدام اليوم الترتيبي.

--------------------

يمكن أن تكون واحدة من قيم تعداد [Month](../../com.aspose.tasks/month).

**Returns:**
int - شهر لنمط التكرار السنوي عند استخدام اليوم الترتيبي.
### getYearlyOrdinalNumber() {#getYearlyOrdinalNumber--}
```
public final int getYearlyOrdinalNumber()
```


يحصل على رقم ترتيبي لنمط التكرار السنوي.

--------------------

يمكن أن تكون واحدة من قيم تعداد [OrdinalNumber](../../com.aspose.tasks/ordinalnumber).

**Returns:**
int - رقم ترتيبي لنمط التكرار السنوي.
### getYearlyUseOrdinalDay() {#getYearlyUseOrdinalDay--}
```
public final boolean getYearlyUseOrdinalDay()
```


يحصل على قيمة تشير إلى ما إذا كان يجب استخدام اليوم الترتيبي لنمط التكرار السنوي.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب استخدام اليوم الترتيبي لنمط التكرار السنوي.
### setDailyRepetitions(int value) {#setDailyRepetitions-int-}
```
public final void setDailyRepetitions(int value)
```


يضبط عدد التكرارات لنمط التكرار اليومي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | عدد من التكرارات لنمط التكرار اليومي. |

### setDailyUseWorkdays(boolean value) {#setDailyUseWorkdays-boolean-}
```
public final void setDailyUseWorkdays(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب استخدام أيام العمل لنمط التكرار اليومي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب استخدام أيام العمل لنمط التكرار اليومي. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


يضبط المدة لحدوث واحد للمهمة المتكررة.

--------------------

مثال على فئة `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | المدة لتكرار واحد للمهمة المتكررة. |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


يضبط التاريخ لنهاية الأحداث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | التاريخ الذي تنتهي فيه التكرارات. |

### setMonthlyDay(int value) {#setMonthlyDay-int-}
```
public final void setMonthlyDay(int value)
```


يضبط عدد الأيام لنمط التكرار الشهري.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | عدد الأيام لنمط التكرار الشهري. |

### setMonthlyOrdinalDay(int value) {#setMonthlyOrdinalDay-int-}
```
public final void setMonthlyOrdinalDay(int value)
```


يضبط يومًا لنمط التكرار الشهري عند استخدام اليوم الترتيبي.

--------------------

يمكن أن تكون واحدة من قيم تعداد [DayOfWeek](../../com.aspose.tasks/dayofweek).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | يوم من نمط التكرار الشهري عند استخدام اليوم الترتيبي. |

### setMonthlyOrdinalNumber(int value) {#setMonthlyOrdinalNumber-int-}
```
public final void setMonthlyOrdinalNumber(int value)
```


يضبط رقمًا ترتيبيًا لنمط التكرار الشهري.

--------------------

يمكن أن تكون واحدة من قيم تعداد [OrdinalNumber](../../com.aspose.tasks/ordinalnumber).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | رقم ترتيبي لنمط التكرار الشهري. |

### setMonthlyOrdinalRepetitions(int value) {#setMonthlyOrdinalRepetitions-int-}
```
public final void setMonthlyOrdinalRepetitions(int value)
```


يضبط عدد التكرارات لنمط التكرار الشهري عند استخدام اليوم الترتيبي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | عدد من التكرارات لنمط التكرار الشهري عند استخدام اليوم الترتيبي. |

### setMonthlyRepetitions(int value) {#setMonthlyRepetitions-int-}
```
public final void setMonthlyRepetitions(int value)
```


يضبط عدد التكرارات لنمط التكرار الشهري.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | عدد من التكرارات لنمط التكرار الشهري. |

### setMonthlyUseOrdinalDay(boolean value) {#setMonthlyUseOrdinalDay-boolean-}
```
public final void setMonthlyUseOrdinalDay(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب استخدام اليوم الترتيبي لنمط التكرار الشهري.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب استخدام اليوم الترتيبي لنمط التكرار الشهري. |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


يضبط عدد مرات حدوث المهمة المتكررة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | عدد من التكرارات للمهمة المتكررة. |

### setRecurrencePattern(int value) {#setRecurrencePattern-int-}
```
public final void setRecurrencePattern(int value)
```


يضبط نمط التكرار للمهمة المتكررة.

--------------------

يمكن أن تكون واحدة من قيم تعداد `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose.tasks/recurringtaskinfo\#setRecurrencePattern-int-)).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | نمط تكرار للمهمة المتكررة. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


يضبط التاريخ لبدء الأحداث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | التاريخ الذي تبدأ فيه التكرارات. |

### setUseEndDate(boolean value) {#setUseEndDate-boolean-}
```
public final void setUseEndDate(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب استخدام تاريخ الانتهاء أو عدد مرات حدوث المهمة المتكررة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب استخدام تاريخ الانتهاء أو عدد من التكرارات للمهمة المتكررة. |

### setWeeklyDays(int value) {#setWeeklyDays-int-}
```
public final void setWeeklyDays(int value)
```


يضبط مجموعة الأيام المستخدمة في نمط التكرار الأسبوعي.

--------------------

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | مجموعة من الأيام المستخدمة في نمط التكرار الأسبوعي. |

### setWeeklyRepetitions(int value) {#setWeeklyRepetitions-int-}
```
public final void setWeeklyRepetitions(int value)
```


يضبط عدد التكرارات لنمط التكرار الأسبوعي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | عدد من التكرارات لنمط التكرار الأسبوعي. |

### setYearlyDate(Date value) {#setYearlyDate-java.util.Date-}
```
public final void setYearlyDate(Date value)
```


يضبط التاريخ لنمط التكرار السنوي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | تاريخ لنمط التكرار السنوي. |

### setYearlyOrdinalDay(int value) {#setYearlyOrdinalDay-int-}
```
public final void setYearlyOrdinalDay(int value)
```


يضبط يوم الأسبوع لنمط التكرار السنوي عند استخدام اليوم الترتيبي.

--------------------

يمكن أن تكون واحدة من قيم تعداد [DayOfWeek](../../com.aspose.tasks/dayofweek).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | يوم أسبوعي لنمط التكرار السنوي عند استخدام اليوم الترتيبي. |

### setYearlyOrdinalMonth(int value) {#setYearlyOrdinalMonth-int-}
```
public final void setYearlyOrdinalMonth(int value)
```


يضبط شهرًا لنمط التكرار السنوي عند استخدام اليوم الترتيبي.

--------------------

يمكن أن تكون واحدة من قيم تعداد [Month](../../com.aspose.tasks/month).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | شهر لنمط التكرار السنوي عند استخدام اليوم الترتيبي. |

### setYearlyOrdinalNumber(int value) {#setYearlyOrdinalNumber-int-}
```
public final void setYearlyOrdinalNumber(int value)
```


يضبط رقمًا ترتيبيًا لنمط التكرار السنوي.

--------------------

يمكن أن تكون واحدة من قيم تعداد [OrdinalNumber](../../com.aspose.tasks/ordinalnumber).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | رقم ترتيبي لنمط التكرار السنوي. |

### setYearlyUseOrdinalDay(boolean value) {#setYearlyUseOrdinalDay-boolean-}
```
public final void setYearlyUseOrdinalDay(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب استخدام اليوم الترتيبي لنمط التكرار السنوي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب استخدام اليوم الترتيبي لنمط التكرار السنوي. |

