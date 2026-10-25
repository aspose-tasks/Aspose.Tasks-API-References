---
title: "DailyRepetitionBase"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Günlük yinelenme desenindeki tekrarlar için temel bir sınıfı temsil eder."
type: docs
weight: 65
url: /tr/java/com.aspose.tasks/dailyrepetitionbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.IValidatorCreator, com.aspose.tasks.ICalculatorCreator
```
public abstract class DailyRepetitionBase implements IValidatorCreator, ICalculatorCreator
```

Günlük yinelenme desenindeki tekrarlar için temel bir sınıfı temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getCalculator(Calendar calendar, Duration duration)](#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-) | \{@inheritDoc\} |
| [getRepetitionInterval()](#getRepetitionInterval--) | Tekrarlar arasındaki aralığı gün cinsinden temsil eden gün sayısını alır. |
| [getValidator(Calendar calendar)](#getValidator-com.aspose.tasks.Calendar-) | \{@inheritDoc\} |
| [setRepetitionInterval(int value)](#setRepetitionInterval-int-) | Tekrarlar arasındaki aralığı gün cinsinden temsil eden gün sayısını ayarlar. |
### getCalculator(Calendar calendar, Duration duration) {#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-}
```
public final RecurrenceDateCalculatorBase getCalculator(Calendar calendar, Duration duration)
```


Bir tekrarı hesaplamak için kullanılan hesaplayıcıyı alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |
| duration | [Duration](../../com.aspose.tasks/duration) | \{@inheritDoc\} |

**Returns:**
com.aspose.tasks.RecurrenceDateCalculatorBase - \{@inheritDoc\}
### getRepetitionInterval() {#getRepetitionInterval--}
```
public final int getRepetitionInterval()
```


Tekrarlar arasındaki aralığı gün cinsinden temsil eden gün sayısını alır.

**Returns:**
int - tekrarlar arasındaki aralığı gün cinsinden temsil eden gün sayısı.
### getValidator(Calendar calendar) {#getValidator-com.aspose.tasks.Calendar-}
```
public final RecurrencePatternValidatorBase getValidator(Calendar calendar)
```


Tekrarlama deseni için bir doğrulayıcı alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |

**Returns:**
com.aspose.tasks.RecurrencePatternValidatorBase - \{@inheritDoc\}
### setRepetitionInterval(int value) {#setRepetitionInterval-int-}
```
public final void setRepetitionInterval(int value)
```


Tekrarlar arasındaki aralığı gün cinsinden temsil eden gün sayısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | tekrarlar arasındaki aralığı gün cinsinden temsil eden gün sayısı. |

