---
title: "CalendarException"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Takvimde olağanüstü zaman dilimlerini temsil eder."
type: docs
weight: 43
url: /tr/java/com.aspose.tasks/calendarexception/
---

**Inheritance:**
java.lang.Object
```
public final class CalendarException
```

Takvimde olağanüstü zaman dilimlerini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [CalendarException()](#CalendarException--) | Yeni bir [CalendarException](../../com.aspose.tasks/calendarexception) sınıfının örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [checkException(Date dt)](#checkException-java.util.Date-) | Belirtilen java.util.Date struct örneği istisna günü ise true döndürür. |
| [delete()](#delete--) | İstisna örneğini üst takvim CalendarExceptionCollection nesnesinden siler. |
| [getDayWorking()](#getDayWorking--) | Belirtilen tarih veya gün tipinin çalışıp çalışmadığını gösteren bir değeri alır. |
| [getDaysOfWeek()](#getDaysOfWeek--) | Bu nesne için DayTypeCollection'ı alır. |
| [getEnteredByOccurrences()](#getEnteredByOccurrences--) | Tekrar aralığının bir sayı girilerek tanımlanıp tanımlanmadığını gösteren bir değer alır. |
| [getExceptionDates()](#getExceptionDates--) | Takvim istisnasının geçerli olduğu tarihleri döndürür. |
| [getFromDate()](#getFromDate--) | İstisna zamanının başlangıcını alır. |
| [getMonth()](#getMonth--) | İstisna tekrarının planlandığı ayı alır. |
| [getMonthDay()](#getMonthDay--) | İstisna tekrarının planlandığı ayın gününü alır. |
| [getMonthItem()](#getMonthItem--) | İstisna tekrarının planlandığı ay öğesini alır. |
| [getMonthPosition()](#getMonthPosition--) | Bir ay içinde ay öğesinin konumunu alır. |
| [getName()](#getName--) | İstisnanın adını alır. |
| [getOccurrences()](#getOccurrences--) | Takvim istisnasının geçerli olduğu tekrar sayısını alır. |
| [getParentCalendar()](#getParentCalendar--) | Bu nesne için üst takvimi alır. |
| [getPeriod()](#getPeriod--) | İstisna için tekrar periyodunu alır. |
| [getToDate()](#getToDate--) | İstisna zamanının sonunu alır. |
| [getType()](#getType--) | İstisna tipini alır. |
| [getWorkingTime()](#getWorkingTime--) | Takvim istisnası için çalışma zamanını döndürür. |
| [getWorkingTimes()](#getWorkingTimes--) | WorkingTimeCollection nesnesini alır. |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | Belirtilen tarih veya gün tipinin çalışıp çalışmadığını gösteren bir değeri ayarlar. |
| [setEnteredByOccurrences(boolean value)](#setEnteredByOccurrences-boolean-) | Tekrar aralığının bir sayı girilerek tanımlanıp tanımlanmadığını gösteren bir değeri ayarlar. |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | İstisna zamanının başlangıcını ayarlar. |
| [setMonth(int value)](#setMonth-int-) | İstisna tekrarı planlanan ayı ayarlar. |
| [setMonthDay(int value)](#setMonthDay-int-) | İstisna tekrarı planlanan ayın gününü ayarlar. |
| [setMonthItem(int value)](#setMonthItem-int-) | İstisna tekrarı planlanan ay öğesini ayarlar. |
| [setMonthPosition(int value)](#setMonthPosition-int-) | Bir ay içinde ay öğesinin konumunu ayarlar. |
| [setName(String value)](#setName-java.lang.String-) | İstisnanın adını ayarlar. |
| [setOccurrences(int value)](#setOccurrences-int-) | Takvim istisnasının geçerli olduğu oluşum sayısını ayarlar. |
| [setPeriod(int value)](#setPeriod-int-) | İstisna için tekrarlama dönemini ayarlar. |
| [setToDate(Date value)](#setToDate-java.util.Date-) | İstisna zamanının sonunu ayarlar. |
| [setType(int value)](#setType-int-) | İstisna tipini ayarlar. |
| [setWorkingTimes(WorkingTimeCollection value)](#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-) | WorkingTimeCollection nesnesini ayarlar. |
### CalendarException() {#CalendarException--}
```
public CalendarException()
```


Yeni bir [CalendarException](../../com.aspose.tasks/calendarexception) sınıfının örneğini başlatır.

### checkException(Date dt) {#checkException-java.util.Date-}
```
public final boolean checkException(Date dt)
```


Belirtilen java.util.Date struct örneği istisna günü ise true döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dt | java.util.Date | java.util.Date yapısının belirtilen örneği. |

**Returns:**
boolean - java.util.Date değeri istisna günü ise true döndürür; aksi takdirde false.
### delete() {#delete--}
```
public final void delete()
```


İstisna örneğini üst takvim CalendarExceptionCollection nesnesinden siler.

### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


Belirtilen tarih veya gün tipinin çalışıp çalışmadığını gösteren bir değeri alır.

**Returns:**
boolean - belirtilen tarih veya gün türünün çalışıp çalışmadığını gösteren bir değer.
### getDaysOfWeek() {#getDaysOfWeek--}
```
public final DayTypeCollection getDaysOfWeek()
```


Bu nesne için DayTypeCollection'ı alır. İstisnanın geçerli olduğu haftanın günleri.

**Returns:**
[DayTypeCollection](../../com.aspose.tasks/daytypecollection) - the DayTypeCollection for this object.
### getEnteredByOccurrences() {#getEnteredByOccurrences--}
```
public final boolean getEnteredByOccurrences()
```


Tekrarlama aralığının bir oluşum sayısı girilerek tanımlanıp tanımlanmadığını gösteren bir değer alır. False, tekrarlama aralığının bir bitiş tarihi girilerek tanımlandığını belirtir.

**Returns:**
boolean - bir oluşum sayısı girilerek tekrarlama aralığının tanımlanıp tanımlanmadığını gösteren değer.
### getExceptionDates() {#getExceptionDates--}
```
public final Iterable<Date> getExceptionDates()
```


Takvim istisnasının geçerli olduğu tarihleri döndürür.

**Returns:**
java.lang.Iterable&lt;java.util.Date&gt; - takvim istisnasının uygulanabilir olduğu tarihler.
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


İstisna zamanının başlangıcını alır.

**Returns:**
java.util.Date - istisna zamanının başlangıcı.
### getMonth() {#getMonth--}
```
public final int getMonth()
```


İstisna tekrarının planlandığı ayı alır.

**Returns:**
int - istisna tekrarı planlanan ay.
### getMonthDay() {#getMonthDay--}
```
public final int getMonthDay()
```


İstisna tekrarının planlandığı ayın gününü alır.

**Returns:**
int - istisna tekrarı planlanan ayın günü.
### getMonthItem() {#getMonthItem--}
```
public final int getMonthItem()
```


İstisna tekrarının planlandığı ay öğesini alır.

**Returns:**
int - istisna tekrarı planlanan ay öğesi.
### getMonthPosition() {#getMonthPosition--}
```
public final int getMonthPosition()
```


Bir ay içinde ay öğesinin konumunu alır.

**Returns:**
int - bir ay içinde ay öğesinin konumu.
### getName() {#getName--}
```
public final String getName()
```


İstisnanın adını alır.

**Returns:**
java.lang.String - istisnanın adı.
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


Takvim istisnasının geçerli olduğu tekrar sayısını alır.

**Returns:**
int - takvim istisnasının geçerli olduğu oluşum sayısı.
### getParentCalendar() {#getParentCalendar--}
```
public final Calendar getParentCalendar()
```


Bu nesne için üst takvimi alır.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - the parent calendar for this object.
### getPeriod() {#getPeriod--}
```
public final int getPeriod()
```


İstisna için tekrar periyodunu alır.

**Returns:**
int - istisna için tekrarlama dönemi.
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


İstisna zamanının sonunu alır.

**Returns:**
java.util.Date - istisna zamanının sonu.
### getType() {#getType--}
```
public final int getType()
```


İstisna tipini alır.

**Returns:**
int - istisna türü.
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


Takvim istisnası için çalışma zamanını döndürür.

**Returns:**
double - Bu takvim istisnası için çalışma süresini döndürür.
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


WorkingTimeCollection nesnesini alır. Haftaiçi çalışılan zamanı tanımlayan çalışma zamanları koleksiyonu.

--------------------

En az bir çalışma zamanı bulunmalı ve beşten fazla olamaz.

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - the WorkingTimeCollection object.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


Belirtilen tarih veya gün tipinin çalışıp çalışmadığını gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | belirtilen tarih veya gün türünün çalışıp çalışmadığını gösteren bir değer. |

### setEnteredByOccurrences(boolean value) {#setEnteredByOccurrences-boolean-}
```
public final void setEnteredByOccurrences(boolean value)
```


Tekrarlama aralığının bir olay sayısı girilerek tanımlanıp tanımlanmadığını gösteren bir değer ayarlar. False, tekrarlama aralığının bir bitiş tarihi girilerek tanımlandığını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | Tekrarlama aralığının bir olay sayısı girilerek tanımlanıp tanımlanmadığını gösteren bir değer. |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


İstisna zamanının başlangıcını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | istisna zamanının başlangıcı. |

### setMonth(int value) {#setMonth-int-}
```
public final void setMonth(int value)
```


İstisna tekrarı planlanan ayı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | istisna tekrarlamasının planlandığı ay. |

### setMonthDay(int value) {#setMonthDay-int-}
```
public final void setMonthDay(int value)
```


İstisna tekrarı planlanan ayın gününü ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | istisna tekrarlamasının planlandığı ayın günü. |

### setMonthItem(int value) {#setMonthItem-int-}
```
public final void setMonthItem(int value)
```


İstisna tekrarı planlanan ay öğesini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | istisna tekrarlamasının planlandığı ay öğesi. |

### setMonthPosition(int value) {#setMonthPosition-int-}
```
public final void setMonthPosition(int value)
```


Bir ay içinde ay öğesinin konumunu ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | bir ay içinde ay öğesinin konumu. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


İstisnanın adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | istisnanın adı. |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


Takvim istisnasının geçerli olduğu oluşum sayısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | takvim istisnasının geçerli olduğu olay sayısı. |

### setPeriod(int value) {#setPeriod-int-}
```
public final void setPeriod(int value)
```


İstisna için tekrarlama dönemini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | istisna için tekrarlama dönemi. |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


İstisna zamanının sonunu ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | istisna zamanının sonu. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


İstisna tipini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | istisna türü. |

### setWorkingTimes(WorkingTimeCollection value) {#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-}
```
public final void setWorkingTimes(WorkingTimeCollection value)
```


WorkingTimeCollection nesnesini ayarlar. Haftaiçi çalışılan zamanı tanımlayan çalışma zamanları koleksiyonu.

--------------------

En az bir çalışma zamanı bulunmalı ve beşten fazla olamaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) | WorkingTimeCollection nesnesi. |

