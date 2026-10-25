---
title: "DailyRepetitionBase"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili kelas dasar untuk pengulangan dalam pola berulang harian."
type: docs
weight: 65
url: /id/java/com.aspose.tasks/dailyrepetitionbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.IValidatorCreator, com.aspose.tasks.ICalculatorCreator
```
public abstract class DailyRepetitionBase implements IValidatorCreator, ICalculatorCreator
```

Mewakili kelas dasar untuk pengulangan dalam pola berulang harian.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getCalculator(Calendar calendar, Duration duration)](#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-) | \{@inheritDoc\} |
| [getRepetitionInterval()](#getRepetitionInterval--) | Mendapatkan sejumlah hari yang mewakili interval dalam hari antara kejadian. |
| [getValidator(Calendar calendar)](#getValidator-com.aspose.tasks.Calendar-) | \{@inheritDoc\} |
| [setRepetitionInterval(int value)](#setRepetitionInterval-int-) | Mengatur sejumlah hari yang mewakili interval dalam hari antara kejadian. |
### getCalculator(Calendar calendar, Duration duration) {#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-}
```
public final RecurrenceDateCalculatorBase getCalculator(Calendar calendar, Duration duration)
```


Mendapatkan kalkulator yang digunakan untuk menghitung pengulangan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |
| duration | [Duration](../../com.aspose.tasks/duration) | \{@inheritDoc\} |

**Returns:**
com.aspose.tasks.RecurrenceDateCalculatorBase - \{@inheritDoc\}
### getRepetitionInterval() {#getRepetitionInterval--}
```
public final int getRepetitionInterval()
```


Mendapatkan sejumlah hari yang mewakili interval dalam hari antara kejadian.

**Returns:**
int - sejumlah hari yang mewakili interval dalam hari antara kejadian.
### getValidator(Calendar calendar) {#getValidator-com.aspose.tasks.Calendar-}
```
public final RecurrencePatternValidatorBase getValidator(Calendar calendar)
```


Mendapatkan validator untuk pola pengulangan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |

**Returns:**
com.aspose.tasks.RecurrencePatternValidatorBase - \{@inheritDoc\}
### setRepetitionInterval(int value) {#setRepetitionInterval-int-}
```
public final void setRepetitionInterval(int value)
```


Mengatur sejumlah hari yang mewakili interval dalam hari antara kejadian.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | sejumlah hari yang mewakili interval dalam hari antara kejadian. |

