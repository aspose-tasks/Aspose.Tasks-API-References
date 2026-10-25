---
title: "WeekDay"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Bir takvimde haftanın normal günlerini veya istisna günlerini tanımlayan bir hafta gününü temsil eder."
type: docs
weight: 352
url: /tr/java/com.aspose.tasks/weekday/
---

**Inheritance:**
java.lang.Object
```
public class WeekDay
```

Bir takvimde haftanın normal günlerini veya istisna günlerini tanımlayan bir hafta gününü temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [WeekDay(int dayType)](#WeekDay-int-) | Belirtilen gün türüyle yeni bir [WeekDay](../../com.aspose.tasks/weekday) sınıfı örneği başlatır. |
| [WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes)](#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--) | Belirtilen gün türü ve çalışma zaman dilimleri listesiyle yeni bir [WeekDay](../../com.aspose.tasks/weekday) sınıfı örneği başlatır. |
| [WeekDay(int dayType, WorkingTime[] workingTimes)](#WeekDay-int-com.aspose.tasks.WorkingTime...-) | Belirtilen gün türü ve çalışma zaman dilimleriyle yeni bir [WeekDay](../../com.aspose.tasks/weekday) sınıfı örneği başlatır. |
| [WeekDay()](#WeekDay--) | Yeni bir [WeekDay](../../com.aspose.tasks/weekday) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [castToDayType(int dw)](#castToDayType-int-) | `.Net`'in [DayOfWeek](../../com.aspose.tasks/dayofweek) değerini `DayType`'a dönüştürür ([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-)). |
| [createDefaultWorkingDay(int dayType)](#createDefaultWorkingDay-int-) | Varsayılan çalışma gününü oluşturur. |
| [deepClone()](#deepClone--) | Hafta gününün derin bir kopyasını döndürür. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür. |
| [getDayType()](#getDayType--) | Bir günün tipini alır. |
| [getDayWorking()](#getDayWorking--) | Belirtilen tarih veya gün tipinin çalışıp çalışmadığını gösteren bir değeri alır. |
| [getFromDate()](#getFromDate--) | Bir istisna zamanının başlangıcını alır. |
| [getToDate()](#getToDate--) | Bir istisna zamanının sonunu alır. |
| [getWorkingTime()](#getWorkingTime--) | Hafta günü için çalışma zamanını döndürür. |
| [getWorkingTimes()](#getWorkingTimes--) | Bu WeekDay örneği için WorkingTimeCollection'ı alır. |
| [hashCode()](#hashCode--) | [WeekDay](../../com.aspose.tasks/weekday) sınıfının örneği için bir hash kod değeri döndürür. |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | Belirtilen tarih veya gün tipinin çalışıp çalışmadığını gösteren bir değeri ayarlar. |
| [setDefaultWorkingTime(WeekDay day)](#setDefaultWorkingTime-com.aspose.tasks.WeekDay-) | Belirtilen hafta günü için varsayılan zaman dilimlerini ayarlar. |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | Bir istisna zamanının başlangıcını ayarlar. |
| [setToDate(Date value)](#setToDate-java.util.Date-) | Bir istisna zamanının sonunu ayarlar. |
### WeekDay(int dayType) {#WeekDay-int-}
```
public WeekDay(int dayType)
```


Belirtilen gün türüyle yeni bir [WeekDay](../../com.aspose.tasks/weekday) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dayType | int | Belirtilen gün tipi. |

### WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes) {#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--}
```
public WeekDay(int dayType, List<WorkingTime> workingTimes)
```


Belirtilen gün türü ve çalışma zaman dilimleri listesiyle yeni bir [WeekDay](../../com.aspose.tasks/weekday) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dayType | int | Belirtilen gün tipi. |
| workingTimes | java.util.List&lt;com.aspose.tasks.WorkingTime&gt; | Çalışma zaman dilimlerinin listesi. |

### WeekDay(int dayType, WorkingTime[] workingTimes) {#WeekDay-int-com.aspose.tasks.WorkingTime...-}
```
public WeekDay(int dayType, WorkingTime[] workingTimes)
```


Belirtilen gün türü ve çalışma zaman dilimleriyle yeni bir [WeekDay](../../com.aspose.tasks/weekday) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dayType | int | Belirtilen gün tipi. |
| workingTimes | [WorkingTime\[\]](../../com.aspose.tasks/workingtime) | Çalışma zaman dilimlerinin dizisi. |

### WeekDay() {#WeekDay--}
```
public WeekDay()
```


Yeni bir [WeekDay](../../com.aspose.tasks/weekday) sınıfı örneği başlatır.

### castToDayType(int dw) {#castToDayType-int-}
```
public static int castToDayType(int dw)
```


`.Net`'in [DayOfWeek](../../com.aspose.tasks/dayofweek) değerini `DayType`'a dönüştürür ([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-)).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dw | int | Dönüştürülecek haftanın günü. |

**Returns:**
int - Dönüştürülmüş bir gün tipi.
### createDefaultWorkingDay(int dayType) {#createDefaultWorkingDay-int-}
```
public static WeekDay createDefaultWorkingDay(int dayType)
```


Varsayılan çalışma gününü oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dayType | int | Varsayılan çalışma günü oluşturmak için kullanılacak gün tipi. |

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - A default working day with working times 8-12 and 13-17.
### deepClone() {#deepClone--}
```
public final WeekDay deepClone()
```


Hafta gününün derin bir kopyasını döndürür.

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - Returns the deep copy of the week day.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object | Bu örnek ile karşılaştırılacak nesne. |

**Returns:**
boolean - **True** eğer belirtilen nesne, bu örnekle aynı FromDate, ToDate değerlerine ve WorkingTimes değerlerine sahip bir WeekDay ise; aksi takdirde **false**.
### getDayType() {#getDayType--}
```
public final int getDayType()
```


Bir günün tipini alır.

**Returns:**
int - bir günün türü.
### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


Belirtilen tarih veya gün tipinin çalışıp çalışmadığını gösteren bir değeri alır.

**Returns:**
boolean - belirtilen tarih veya gün türünün çalışıp çalışmadığını gösteren bir değer.
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


Bir istisna zamanının başlangıcını alır.

**Returns:**
java.util.Date - bir istisna süresinin başlangıcı.
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


Bir istisna zamanının sonunu alır.

**Returns:**
java.util.Date - bir istisna süresinin sonu.
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


Hafta günü için çalışma zamanını döndürür.

**Returns:**
double - Çalışma süresi.
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


Bu WeekDay örneği için WorkingTimeCollection'ı alır. Haftanın günü üzerinde çalışılan zamanı tanımlayan çalışma zamanları koleksiyonu.

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - WorkingTimeCollection for this WeekDay instance.
### hashCode() {#hashCode--}
```
public int hashCode()
```


[WeekDay](../../com.aspose.tasks/weekday) sınıfının örneği için bir hash kod değeri döndürür.

**Returns:**
int - bu nesne için bir karma kod değeri döndürür.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


Belirtilen tarih veya gün tipinin çalışıp çalışmadığını gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | belirtilen tarih veya gün türünün çalışıp çalışmadığını gösteren bir değer. |

### setDefaultWorkingTime(WeekDay day) {#setDefaultWorkingTime-com.aspose.tasks.WeekDay-}
```
public static void setDefaultWorkingTime(WeekDay day)
```


Belirtilen hafta günü için varsayılan zaman dilimlerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| day | [WeekDay](../../com.aspose.tasks/weekday) | Varsayılan çalışma gününün ayarlanacağı hafta günü. |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


Bir istisna zamanının başlangıcını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | bir istisna süresinin başlangıcı. |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


Bir istisna zamanının sonunu ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | bir istisna süresinin sonu. |

