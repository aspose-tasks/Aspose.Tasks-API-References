---
title: "MonthlyRepetitionBase"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili pola dasar untuk posisi hari bulanan."
type: docs
weight: 159
url: /id/java/com.aspose.tasks/monthlyrepetitionbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.IValidatorCreator, com.aspose.tasks.ICalculatorCreator
```
public abstract class MonthlyRepetitionBase implements IValidatorCreator, ICalculatorCreator
```

Mewakili pola dasar untuk posisi hari bulanan.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getCalculator(Calendar calendar, Duration duration)](#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-) | \{@inheritDoc\} |
| [getRepetitionInterval()](#getRepetitionInterval--) | Mendapatkan jumlah bulan yang mewakili interval dalam bulan antara kejadian. |
| [getValidator(Calendar calendar)](#getValidator-com.aspose.tasks.Calendar-) | \{@inheritDoc\} |
| [setRepetitionInterval(int value)](#setRepetitionInterval-int-) | Mengatur jumlah bulan yang mewakili interval dalam bulan antara kejadian. |
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


Mendapatkan jumlah bulan yang mewakili interval dalam bulan antara kejadian.

**Returns:**
int - jumlah bulan yang mewakili interval dalam bulan antara kejadian.
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


Mengatur jumlah bulan yang mewakili interval dalam bulan antara kejadian.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | jumlah bulan yang mewakili interval dalam bulan antara kejadian. |

