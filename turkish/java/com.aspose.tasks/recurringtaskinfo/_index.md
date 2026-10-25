---
title: "RecurringTaskInfo"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Projede bir yineleyen görevin ayrıntılarını temsil eder."
type: docs
weight: 244
url: /tr/java/com.aspose.tasks/recurringtaskinfo/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskInfo
```

Projede bir yineleyen görevin ayrıntılarını temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getDailyRepetitions()](#getDailyRepetitions--) | Günlük yinelenme deseni için bir tekrar sayısı alır. |
| [getDailyUseWorkdays()](#getDailyUseWorkdays--) | Günlük yinelenme deseni için iş günlerinin kullanılıp kullanılmayacağını gösteren bir değer alır. |
| [getDuration()](#getDuration--) | Yinelenen görevin bir gerçekleşmesi için süresi alır. |
| [getEndDate()](#getEndDate--) | Gerçekleşmelerin sona ereceği tarihi alır. |
| [getMonthlyDay()](#getMonthlyDay--) | Aylık yinelenme deseni için bir gün sayısı alır. |
| [getMonthlyOrdinalDay()](#getMonthlyOrdinalDay--) | Sıralı gün kullanıldığında aylık yinelenme deseninin gününü alır. |
| [getMonthlyOrdinalNumber()](#getMonthlyOrdinalNumber--) | Aylık yinelenme deseninin sıralı numarasını alır. |
| [getMonthlyOrdinalRepetitions()](#getMonthlyOrdinalRepetitions--) | Sıralı gün kullanıldığında aylık yinelenme deseni için bir tekrar sayısı alır. |
| [getMonthlyRepetitions()](#getMonthlyRepetitions--) | Aylık yinelenme deseni için bir tekrar sayısı alır. |
| [getMonthlyUseOrdinalDay()](#getMonthlyUseOrdinalDay--) | Aylık yinelenme deseni için sıralı günün kullanılıp kullanılmayacağını gösteren bir değer alır. |
| [getOccurrences()](#getOccurrences--) | Yinelenen görevin gerçekleşme sayısını alır. |
| [getRecurrencePattern()](#getRecurrencePattern--) | Yinelenen görevin yinelenme desenini alır. |
| [getStartDate()](#getStartDate--) | Gerçekleşmelerin başlayacağı tarihi alır. |
| [getTask()](#getTask--) | Bu [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) sınıfının örneğinin üst görevini alır. |
| [getUseEndDate()](#getUseEndDate--) | Yinelenen görev için bitiş tarihinin mi yoksa gerçekleşme sayısının mı kullanılacağını gösteren bir değer alır. |
| [getWeeklyDays()](#getWeeklyDays--) | Haftalık yinelenme deseninde kullanılan günlerin koleksiyonunu alır. |
| [getWeeklyRepetitions()](#getWeeklyRepetitions--) | Haftalık yinelenme deseni için bir tekrar sayısı alır. |
| [getYearlyDate()](#getYearlyDate--) | Yıllık yinelenme deseni için bir tarih alır. |
| [getYearlyOrdinalDay()](#getYearlyOrdinalDay--) | Sıralı gün kullanıldığında yıllık yineleme deseninin bir hafta gününü alır. |
| [getYearlyOrdinalMonth()](#getYearlyOrdinalMonth--) | Sıralı gün kullanıldığında yıllık yineleme deseninin bir ayını alır. |
| [getYearlyOrdinalNumber()](#getYearlyOrdinalNumber--) | Yıllık yineleme deseninin sıralı numarasını alır. |
| [getYearlyUseOrdinalDay()](#getYearlyUseOrdinalDay--) | Yıllık yineleme deseni için sıralı gün kullanılıp kullanılmayacağını gösteren bir değeri alır. |
| [setDailyRepetitions(int value)](#setDailyRepetitions-int-) | Günlük yineleme deseni için tekrar sayısını ayarlar. |
| [setDailyUseWorkdays(boolean value)](#setDailyUseWorkdays-boolean-) | Günlük yineleme deseni için iş günlerinin kullanılıp kullanılmayacağını gösteren bir değeri ayarlar. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Yineleyen görevin bir oluşumu için süresi ayarlar. |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | Oluşumların sona ereceği tarihi ayarlar. |
| [setMonthlyDay(int value)](#setMonthlyDay-int-) | Aylık yineleme deseninin gün sayısını ayarlar. |
| [setMonthlyOrdinalDay(int value)](#setMonthlyOrdinalDay-int-) | Sıralı gün kullanıldığında aylık yineleme deseninin gününü ayarlar. |
| [setMonthlyOrdinalNumber(int value)](#setMonthlyOrdinalNumber-int-) | Aylık yineleme deseninin sıralı numarasını ayarlar. |
| [setMonthlyOrdinalRepetitions(int value)](#setMonthlyOrdinalRepetitions-int-) | Sıralı gün kullanıldığında aylık yineleme deseni için tekrar sayısını ayarlar. |
| [setMonthlyRepetitions(int value)](#setMonthlyRepetitions-int-) | Aylık yineleme deseni için tekrar sayısını ayarlar. |
| [setMonthlyUseOrdinalDay(boolean value)](#setMonthlyUseOrdinalDay-boolean-) | Aylık yineleme deseni için sıralı gün kullanılıp kullanılmayacağını gösteren bir değeri ayarlar. |
| [setOccurrences(int value)](#setOccurrences-int-) | Yineleyen görevin oluşum sayısını ayarlar. |
| [setRecurrencePattern(int value)](#setRecurrencePattern-int-) | Yineleyen görevin yineleme desenini ayarlar. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Oluşumların başlayacağı tarihi ayarlar. |
| [setUseEndDate(boolean value)](#setUseEndDate-boolean-) | Yineleyen görev için bitiş tarihinin mi yoksa oluşum sayısının mı kullanılacağını gösteren bir değeri ayarlar. |
| [setWeeklyDays(int value)](#setWeeklyDays-int-) | Haftalık yineleme deseninde kullanılan günlerin koleksiyonunu ayarlar. |
| [setWeeklyRepetitions(int value)](#setWeeklyRepetitions-int-) | Haftalık yineleme deseni için tekrar sayısını ayarlar. |
| [setYearlyDate(Date value)](#setYearlyDate-java.util.Date-) | Yıllık yineleme deseni için tarihi ayarlar. |
| [setYearlyOrdinalDay(int value)](#setYearlyOrdinalDay-int-) | Sıralı gün kullanıldığında yıllık yineleme deseninin hafta gününü ayarlar. |
| [setYearlyOrdinalMonth(int value)](#setYearlyOrdinalMonth-int-) | Sıralı gün kullanıldığında yıllık yineleme deseninin ayını ayarlar. |
| [setYearlyOrdinalNumber(int value)](#setYearlyOrdinalNumber-int-) | Yıllık yineleme deseninin sıralı numarasını ayarlar. |
| [setYearlyUseOrdinalDay(boolean value)](#setYearlyUseOrdinalDay-boolean-) | Yıllık yineleme deseni için sıralı gün kullanılıp kullanılmayacağını gösteren bir değeri ayarlar. |
### getDailyRepetitions() {#getDailyRepetitions--}
```
public final int getDailyRepetitions()
```


Günlük yinelenme deseni için bir tekrar sayısı alır.

**Returns:**
int - günlük yineleme deseni için tekrar sayısı.
### getDailyUseWorkdays() {#getDailyUseWorkdays--}
```
public final boolean getDailyUseWorkdays()
```


Günlük yinelenme deseni için iş günlerinin kullanılıp kullanılmayacağını gösteren bir değer alır.

**Returns:**
boolean - günlük yineleme deseni için iş günlerinin kullanılıp kullanılmayacağını gösteren bir değer.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Yinelenen görevin bir gerçekleşmesi için süresi alır.

--------------------

`Duration` sınıfının örneği([getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)).

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration for one occurrence of the recurring task.
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


Gerçekleşmelerin sona ereceği tarihi alır.

**Returns:**
java.util.Date - oluşumların sona ereceği tarih.
### getMonthlyDay() {#getMonthlyDay--}
```
public final int getMonthlyDay()
```


Aylık yinelenme deseni için bir gün sayısı alır.

**Returns:**
int - aylık yineleme desenindeki gün sayısı.
### getMonthlyOrdinalDay() {#getMonthlyOrdinalDay--}
```
public final int getMonthlyOrdinalDay()
```


Sıralı gün kullanıldığında aylık yinelenme deseninin gününü alır.

--------------------

[DayOfWeek](../../com.aspose.tasks/dayofweek) enumerasyonunun değerlerinden biri olabilir.

**Returns:**
int - sıralı gün kullanıldığında aylık yineleme desenindeki gün.
### getMonthlyOrdinalNumber() {#getMonthlyOrdinalNumber--}
```
public final int getMonthlyOrdinalNumber()
```


Aylık yinelenme deseninin sıralı numarasını alır.

--------------------

[OrdinalNumber](../../com.aspose.tasks/ordinalnumber) enumerasyonunun değerlerinden biri olabilir.

**Returns:**
int - aylık yineleme deseninin sıralı numarası.
### getMonthlyOrdinalRepetitions() {#getMonthlyOrdinalRepetitions--}
```
public final int getMonthlyOrdinalRepetitions()
```


Sıralı gün kullanıldığında aylık yinelenme deseni için bir tekrar sayısı alır.

**Returns:**
int - sıralı gün kullanıldığında aylık yineleme deseni için tekrar sayısı.
### getMonthlyRepetitions() {#getMonthlyRepetitions--}
```
public final int getMonthlyRepetitions()
```


Aylık yinelenme deseni için bir tekrar sayısı alır.

**Returns:**
int - aylık yineleme deseni için tekrar sayısı.
### getMonthlyUseOrdinalDay() {#getMonthlyUseOrdinalDay--}
```
public final boolean getMonthlyUseOrdinalDay()
```


Aylık yinelenme deseni için sıralı günün kullanılıp kullanılmayacağını gösteren bir değer alır.

**Returns:**
boolean - aylık yineleme deseni için sıralı günün kullanılıp kullanılmayacağını gösteren bir değer.
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


Yinelenen görevin gerçekleşme sayısını alır.

**Returns:**
int - yinelenen görevin oluşum sayısı.
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final int getRecurrencePattern()
```


Yinelenen görevin yinelenme desenini alır.

--------------------

`RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose.tasks/recurringtaskinfo\#setRecurrencePattern-int-)) enumerasyonunun değerlerinden biri olabilir.

**Returns:**
int - yinelenen görevin yineleme deseni.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Gerçekleşmelerin başlayacağı tarihi alır.

**Returns:**
java.util.Date - oluşumların başlayacağı tarih.
### getTask() {#getTask--}
```
public final Task getTask()
```


Bu [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) sınıfının örneğinin üst görevini alır.

**Returns:**
[Task](../../com.aspose.tasks/task) - the parent task of this instance of [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) class.
### getUseEndDate() {#getUseEndDate--}
```
public final boolean getUseEndDate()
```


Yinelenen görev için bitiş tarihinin mi yoksa gerçekleşme sayısının mı kullanılacağını gösteren bir değer alır.

**Returns:**
boolean - yinelenen görev için bitiş tarihinin mi yoksa oluşum sayısının mı kullanılacağını gösteren bir değer.
### getWeeklyDays() {#getWeeklyDays--}
```
public final int getWeeklyDays()
```


Haftalık yinelenme deseninde kullanılan günlerin koleksiyonunu alır.

--------------------

**Returns:**
int - haftalık yineleme deseninde kullanılan günlerin koleksiyonu.
### getWeeklyRepetitions() {#getWeeklyRepetitions--}
```
public final int getWeeklyRepetitions()
```


Haftalık yinelenme deseni için bir tekrar sayısı alır.

**Returns:**
int - haftalık yineleme deseni için tekrar sayısı.
### getYearlyDate() {#getYearlyDate--}
```
public final Date getYearlyDate()
```


Yıllık yinelenme deseni için bir tarih alır.

**Returns:**
java.util.Date - yıllık yineleme deseni için tarih.
### getYearlyOrdinalDay() {#getYearlyOrdinalDay--}
```
public final int getYearlyOrdinalDay()
```


Sıralı gün kullanıldığında yıllık yineleme deseninin bir hafta gününü alır.

--------------------

[DayOfWeek](../../com.aspose.tasks/dayofweek) enumerasyonunun değerlerinden biri olabilir.

**Returns:**
int - sıralı gün kullanıldığında yıllık yineleme deseninin haftaiçi günü.
### getYearlyOrdinalMonth() {#getYearlyOrdinalMonth--}
```
public final int getYearlyOrdinalMonth()
```


Sıralı gün kullanıldığında yıllık yineleme deseninin bir ayını alır.

--------------------

[Month](../../com.aspose.tasks/month) enumerasyonunun değerlerinden biri olabilir.

**Returns:**
int - sıralı gün kullanıldığında yıllık yineleme deseninin ayı.
### getYearlyOrdinalNumber() {#getYearlyOrdinalNumber--}
```
public final int getYearlyOrdinalNumber()
```


Yıllık yineleme deseninin sıralı numarasını alır.

--------------------

[OrdinalNumber](../../com.aspose.tasks/ordinalnumber) enumerasyonunun değerlerinden biri olabilir.

**Returns:**
int - yıllık yineleme deseninin sıralı numarası.
### getYearlyUseOrdinalDay() {#getYearlyUseOrdinalDay--}
```
public final boolean getYearlyUseOrdinalDay()
```


Yıllık yineleme deseni için sıralı gün kullanılıp kullanılmayacağını gösteren bir değeri alır.

**Returns:**
boolean - yıllık yineleme deseni için sıralı günün kullanılıp kullanılmayacağını gösteren bir değer.
### setDailyRepetitions(int value) {#setDailyRepetitions-int-}
```
public final void setDailyRepetitions(int value)
```


Günlük yineleme deseni için tekrar sayısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | günlük yineleme deseni için bir tekrar sayısı. |

### setDailyUseWorkdays(boolean value) {#setDailyUseWorkdays-boolean-}
```
public final void setDailyUseWorkdays(boolean value)
```


Günlük yineleme deseni için iş günlerinin kullanılıp kullanılmayacağını gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | günlük yineleme deseni için iş günlerinin kullanılıp kullanılmayacağını belirten bir değer. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Yineleyen görevin bir oluşumu için süresi ayarlar.

--------------------

`Duration` sınıfının örneği([getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | yinelenen görevin bir oluşumu için süre. |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


Oluşumların sona ereceği tarihi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | oluşumların sona ereceği tarih. |

### setMonthlyDay(int value) {#setMonthlyDay-int-}
```
public final void setMonthlyDay(int value)
```


Aylık yineleme deseninin gün sayısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | aylık yineleme desenindeki gün sayısı. |

### setMonthlyOrdinalDay(int value) {#setMonthlyOrdinalDay-int-}
```
public final void setMonthlyOrdinalDay(int value)
```


Sıralı gün kullanıldığında aylık yineleme deseninin gününü ayarlar.

--------------------

[DayOfWeek](../../com.aspose.tasks/dayofweek) enumerasyonunun değerlerinden biri olabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | sıralı gün kullanıldığında aylık yineleme deseninin günü. |

### setMonthlyOrdinalNumber(int value) {#setMonthlyOrdinalNumber-int-}
```
public final void setMonthlyOrdinalNumber(int value)
```


Aylık yineleme deseninin sıralı numarasını ayarlar.

--------------------

[OrdinalNumber](../../com.aspose.tasks/ordinalnumber) enumerasyonunun değerlerinden biri olabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | aylık yineleme deseninin sıralı numarası. |

### setMonthlyOrdinalRepetitions(int value) {#setMonthlyOrdinalRepetitions-int-}
```
public final void setMonthlyOrdinalRepetitions(int value)
```


Sıralı gün kullanıldığında aylık yineleme deseni için tekrar sayısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | sıralı gün kullanıldığında aylık yineleme deseni için tekrar sayısı. |

### setMonthlyRepetitions(int value) {#setMonthlyRepetitions-int-}
```
public final void setMonthlyRepetitions(int value)
```


Aylık yineleme deseni için tekrar sayısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | aylık yineleme deseni için tekrar sayısı. |

### setMonthlyUseOrdinalDay(boolean value) {#setMonthlyUseOrdinalDay-boolean-}
```
public final void setMonthlyUseOrdinalDay(boolean value)
```


Aylık yineleme deseni için sıralı gün kullanılıp kullanılmayacağını gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | aylık yineleme deseni için sıralı günün kullanılıp kullanılmayacağını belirten bir değer. |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


Yineleyen görevin oluşum sayısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | yinelenen görevin oluşum sayısı. |

### setRecurrencePattern(int value) {#setRecurrencePattern-int-}
```
public final void setRecurrencePattern(int value)
```


Yineleyen görevin yineleme desenini ayarlar.

--------------------

`RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose.tasks/recurringtaskinfo\#setRecurrencePattern-int-)) enumerasyonunun değerlerinden biri olabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | yinelenen görevin bir yineleme deseni. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Oluşumların başlayacağı tarihi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | oluşumların başlayacağı tarih. |

### setUseEndDate(boolean value) {#setUseEndDate-boolean-}
```
public final void setUseEndDate(boolean value)
```


Yineleyen görev için bitiş tarihinin mi yoksa oluşum sayısının mı kullanılacağını gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | yinelenen görev için bitiş tarihinin mi yoksa oluşum sayısının mı kullanılacağını belirten bir değer. |

### setWeeklyDays(int value) {#setWeeklyDays-int-}
```
public final void setWeeklyDays(int value)
```


Haftalık yineleme deseninde kullanılan günlerin koleksiyonunu ayarlar.

--------------------

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | haftalık yineleme deseninde kullanılan günlerin koleksiyonu. |

### setWeeklyRepetitions(int value) {#setWeeklyRepetitions-int-}
```
public final void setWeeklyRepetitions(int value)
```


Haftalık yineleme deseni için tekrar sayısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | haftalık yineleme deseni için tekrar sayısı. |

### setYearlyDate(Date value) {#setYearlyDate-java.util.Date-}
```
public final void setYearlyDate(Date value)
```


Yıllık yineleme deseni için tarihi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | yıllık yineleme deseni için tarih. |

### setYearlyOrdinalDay(int value) {#setYearlyOrdinalDay-int-}
```
public final void setYearlyOrdinalDay(int value)
```


Sıralı gün kullanıldığında yıllık yineleme deseninin hafta gününü ayarlar.

--------------------

[DayOfWeek](../../com.aspose.tasks/dayofweek) enumerasyonunun değerlerinden biri olabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | sıralı gün kullanıldığında yıllık yineleme deseninin haftaiçi günü. |

### setYearlyOrdinalMonth(int value) {#setYearlyOrdinalMonth-int-}
```
public final void setYearlyOrdinalMonth(int value)
```


Sıralı gün kullanıldığında yıllık yineleme deseninin ayını ayarlar.

--------------------

[Month](../../com.aspose.tasks/month) enumerasyonunun değerlerinden biri olabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | sıralı gün kullanıldığında yıllık yineleme deseninin ayı. |

### setYearlyOrdinalNumber(int value) {#setYearlyOrdinalNumber-int-}
```
public final void setYearlyOrdinalNumber(int value)
```


Yıllık yineleme deseninin sıralı numarasını ayarlar.

--------------------

[OrdinalNumber](../../com.aspose.tasks/ordinalnumber) enumerasyonunun değerlerinden biri olabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | yıllık yineleme deseninin sıralı numarası. |

### setYearlyUseOrdinalDay(boolean value) {#setYearlyUseOrdinalDay-boolean-}
```
public final void setYearlyUseOrdinalDay(boolean value)
```


Yıllık yineleme deseni için sıralı gün kullanılıp kullanılmayacağını gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | yıllık yineleme deseni için sıralı günün kullanılıp kullanılmayacağını belirten bir değer. |

