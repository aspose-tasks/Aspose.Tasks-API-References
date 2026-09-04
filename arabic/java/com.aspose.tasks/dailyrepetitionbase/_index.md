---
title: "DailyRepetitionBase"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل فئة أساسية للتكرارات في نمط التكرار اليومي."
type: docs
weight: 65
url: /ar/java/com.aspose.tasks/dailyrepetitionbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.IValidatorCreator, com.aspose.tasks.ICalculatorCreator
```
public abstract class DailyRepetitionBase implements IValidatorCreator, ICalculatorCreator
```

يمثل فئة أساسية للتكرارات في نمط التكرار اليومي.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getCalculator(Calendar calendar, Duration duration)](#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-) | \{@inheritDoc\} |
| [getRepetitionInterval()](#getRepetitionInterval--) | يحصل على عدد الأيام الذي يمثل الفاصل بالأيام بين التكرارات. |
| [getValidator(Calendar calendar)](#getValidator-com.aspose.tasks.Calendar-) | \{@inheritDoc\} |
| [setRepetitionInterval(int value)](#setRepetitionInterval-int-) | يضبط عدد الأيام الذي يمثل الفاصل بالأيام بين التكرارات. |
### getCalculator(Calendar calendar, Duration duration) {#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-}
```
public final RecurrenceDateCalculatorBase getCalculator(Calendar calendar, Duration duration)
```


يحصل على الحاسبة المستخدمة لحساب التكرار.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |
| duration | [Duration](../../com.aspose.tasks/duration) | \{@inheritDoc\} |

**Returns:**
com.aspose.tasks.RecurrenceDateCalculatorBase - \{@inheritDoc\}
### getRepetitionInterval() {#getRepetitionInterval--}
```
public final int getRepetitionInterval()
```


يحصل على عدد الأيام الذي يمثل الفاصل بالأيام بين التكرارات.

**Returns:**
int - عدد الأيام الذي يمثل الفاصل بالأيام بين التكرارات.
### getValidator(Calendar calendar) {#getValidator-com.aspose.tasks.Calendar-}
```
public final RecurrencePatternValidatorBase getValidator(Calendar calendar)
```


يحصل على مدقق لنمط التكرار.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |

**Returns:**
com.aspose.tasks.RecurrencePatternValidatorBase - \{@inheritDoc\}
### setRepetitionInterval(int value) {#setRepetitionInterval-int-}
```
public final void setRepetitionInterval(int value)
```


يضبط عدد الأيام الذي يمثل الفاصل بالأيام بين التكرارات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | عدد الأيام الذي يمثل الفاصل بالأيام بين التكرارات. |

