---
title: "MonthlyRepetitionBase"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل نمطًا أساسيًا لموضع اليوم الشهري."
type: docs
weight: 159
url: /ar/java/com.aspose.tasks/monthlyrepetitionbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.IValidatorCreator, com.aspose.tasks.ICalculatorCreator
```
public abstract class MonthlyRepetitionBase implements IValidatorCreator, ICalculatorCreator
```

يمثل نمطًا أساسيًا لموضع اليوم الشهري.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getCalculator(Calendar calendar, Duration duration)](#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-) | \{@inheritDoc\} |
| [getRepetitionInterval()](#getRepetitionInterval--) | يحصل على عدد الشهور الذي يمثل الفاصل الزمني بين التكرارات بالشهور. |
| [getValidator(Calendar calendar)](#getValidator-com.aspose.tasks.Calendar-) | \{@inheritDoc\} |
| [setRepetitionInterval(int value)](#setRepetitionInterval-int-) | يضبط عدد الشهور الذي يمثل الفاصل الزمني بين التكرارات بالشهور. |
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


يحصل على عدد الشهور الذي يمثل الفاصل الزمني بين التكرارات بالشهور.

**Returns:**
int - عدد الشهور الذي يمثل الفاصل الزمني بين التكرارات بالشهور.
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


يضبط عدد الشهور الذي يمثل الفاصل الزمني بين التكرارات بالشهور.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | عدد الشهور الذي يمثل الفاصل الزمني بين التكرارات بالشهور. |

