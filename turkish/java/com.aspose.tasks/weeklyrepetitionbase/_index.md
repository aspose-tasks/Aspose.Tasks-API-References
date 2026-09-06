---
title: "WeeklyRepetitionBase"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Haftalık yinelenme deseninde tekrarlar için temel sınıfı temsil eder."
type: docs
weight: 358
url: /tr/java/com.aspose.tasks/weeklyrepetitionbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.IValidatorCreator, com.aspose.tasks.ICalculatorCreator
```
public abstract class WeeklyRepetitionBase implements IValidatorCreator, ICalculatorCreator
```

Haftalık yinelenme deseninde tekrarlar için temel sınıfı temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getCalculator(Calendar calendar, Duration duration)](#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-) | \{@inheritDoc\} |
| [getRepetitionInterval()](#getRepetitionInterval--) | Tekrarlar arasındaki haftalar aralığını temsil eden hafta sayısını alır. |
| [getValidator(Calendar calendar)](#getValidator-com.aspose.tasks.Calendar-) | \{@inheritDoc\} |
| [setRepetitionInterval(int value)](#setRepetitionInterval-int-) | Tekrarlar arasındaki haftalar aralığını temsil eden hafta sayısını ayarlar. |
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


Tekrarlar arasındaki haftalar aralığını temsil eden hafta sayısını alır.

**Returns:**
int - tekrarlar arasındaki haftalar aralığını temsil eden hafta sayısı.
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


Tekrarlar arasındaki haftalar aralığını temsil eden hafta sayısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | tekrarlar arasındaki haftalar aralığını temsil eden hafta sayısı. |

