---
title: "WeeklyRepetitionBase"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل فئة أساسية للتكرارات في نمط التكرار الأسبوعي."
type: docs
weight: 358
url: /ar/java/com.aspose.tasks/weeklyrepetitionbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.IValidatorCreator, com.aspose.tasks.ICalculatorCreator
```
public abstract class WeeklyRepetitionBase implements IValidatorCreator, ICalculatorCreator
```

يمثل فئة أساسية للتكرارات في نمط التكرار الأسبوعي.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getCalculator(Calendar calendar, Duration duration)](#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-) | \{@inheritDoc\} |
| [getRepetitionInterval()](#getRepetitionInterval--) | يحصل على عدد الأسابيع الذي يمثل الفاصل بالأسابيع بين التكرارات. |
| [getValidator(Calendar calendar)](#getValidator-com.aspose.tasks.Calendar-) | \{@inheritDoc\} |
| [setRepetitionInterval(int value)](#setRepetitionInterval-int-) | يضبط عدد الأسابيع الذي يمثل الفاصل بالأسابيع بين التكرارات. |
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


يحصل على عدد الأسابيع الذي يمثل الفاصل بالأسابيع بين التكرارات.

**Returns:**
int - عدد الأسابيع الذي يمثل الفاصل بالأسابيع بين التكرارات.
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


يضبط عدد الأسابيع الذي يمثل الفاصل بالأسابيع بين التكرارات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | عدد الأسابيع الذي يمثل الفاصل بالأسابيع بين التكرارات. |

