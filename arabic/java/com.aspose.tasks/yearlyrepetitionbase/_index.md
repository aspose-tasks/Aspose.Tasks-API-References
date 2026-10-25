---
title: "YearlyRepetitionBase"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل نمطًا أساسيًا لموضع اليوم السنوي."
type: docs
weight: 372
url: /ar/java/com.aspose.tasks/yearlyrepetitionbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.IValidatorCreator, com.aspose.tasks.ICalculatorCreator
```
public abstract class YearlyRepetitionBase implements IValidatorCreator, ICalculatorCreator
```

يمثل نمطًا أساسيًا لموضع اليوم السنوي.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getCalculator(Calendar calendar, Duration duration)](#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-) | \{@inheritDoc\} |
| [getValidator(Calendar calendar)](#getValidator-com.aspose.tasks.Calendar-) | \{@inheritDoc\} |
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
