---
title: "ICalendar"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Tarih ve sürelerin çeşitli hesaplamaları için kullanılabilecek bir takvim soyutlamasını temsil eder."
type: docs
weight: 376
url: /tr/java/com.aspose.tasks/icalendar/
---
```
public interface ICalendar
```

Tarih ve sürelerin çeşitli hesaplamaları için kullanılabilecek bir takvim soyutlamasını temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getFinishDateByStartAndWork(Date start, Duration work)](#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-) | Takvime göre belirtilen çalışma süresi miktarı geçtiğinde tarihi hesaplar. |
| [getFinishDateByStartAndWork(Date start, double work)](#getFinishDateByStartAndWork-java.util.Date-double-) | Takvime göre belirtilen çalışma süresi miktarı geçtiğinde tarihi hesaplar. |
| [getNextWorkingDayStart(Date date)](#getNextWorkingDayStart-java.util.Date-) | Belirtilen tarih için bir sonraki çalışma gününün başlangıcını hesaplar. |
| [getPreviousWorkingDayEnd(Date date)](#getPreviousWorkingDayEnd-java.util.Date-) | Belirtilen tarihten önceki çalışma gününün sonunu hesaplar. |
| [getStartDateFromFinishAndDuration(Date finish, Duration duration)](#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-) | Belirtilen bitiş tarihi ve sürece göre başlangıç tarihini döndürür. |
| [getStartDateFromFinishAndDuration(Date finish, double duration)](#getStartDateFromFinishAndDuration-java.util.Date-double-) | Belirtilen bitiş tarihi ve sürece göre başlangıç tarihini döndürür. |
| [getTaskFinishDateFromDuration(Task task, double duration)](#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-) | Görevin başlangıç tarihi, bölünmüş parçaları ve çalışma süresinden görev bitiş tarih ve saatini hesaplar. |
| [getWorkStart(Date date)](#getWorkStart-java.util.Date-) | Belirtilen tarih ve saatten itibaren bir sonraki çalışma zamanının başlangıcını hesaplar. |
| [getWorkingHours(Date dt)](#getWorkingHours-java.util.Date-) | Belirtilen tarihteki çalışma saat miktarını döndürür. |
| [getWorkingHours(Date start, Date finish)](#getWorkingHours-java.util.Date-java.util.Date-) | WorkUnit'i döndür - Belirtilen tarih saat aralığı için çalışma saatlerinin Başlangıcı, Bitişi ve Süresi. |
| [getWorkingHoursTimeSpan(Date start, Date finish)](#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-) | Belirtilen tarihler arasındaki çalışma saat miktarını döndürür. |
| [getWorkingTimes(Date dt)](#getWorkingTimes-java.util.Date-) | Belirtilen tarih için çalışma zamanlarının [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) nesnesini döndürür. |
| [isDayWorking(Date dt)](#isDayWorking-java.util.Date-) | Takvime göre belirtilen günün çalışma günü olup olmadığını belirler. |
| [isEmpty()](#isEmpty--) | Takvimin tanımlı çalışma saatleri olup olmadığını döndürür. |
### getFinishDateByStartAndWork(Date start, Duration work) {#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getFinishDateByStartAndWork(Date start, Duration work)
```


Takvime göre belirtilen çalışma süresi miktarı geçtiğinde tarihi hesaplar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlat | java.util.Date | Başlangıç tarihi. |
| work | [Duration](../../com.aspose.tasks/duration) | Çalışma süresi. |

**Returns:**
java.util.Date - Bitiş tarihi.
### getFinishDateByStartAndWork(Date start, double work) {#getFinishDateByStartAndWork-java.util.Date-double-}
```
public abstract Date getFinishDateByStartAndWork(Date start, double work)
```


Takvime göre belirtilen çalışma süresi miktarı geçtiğinde tarihi hesaplar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlat | java.util.Date | Başlangıç tarihi. |
| çalışma | double | Çalışma süresi. |

**Returns:**
java.util.Date - Bitiş tarihi.
### getNextWorkingDayStart(Date date) {#getNextWorkingDayStart-java.util.Date-}
```
public abstract Date getNextWorkingDayStart(Date date)
```


Belirtilen tarih için bir sonraki çalışma gününün başlangıcını hesaplar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tarih | java.util.Date | Sonraki çalışma gününün başlangıcı için alınacak tarih. |

**Returns:**
java.util.Date - Sonraki çalışma gününün başlangıcı System.DateTime.
### getPreviousWorkingDayEnd(Date date) {#getPreviousWorkingDayEnd-java.util.Date-}
```
public abstract Date getPreviousWorkingDayEnd(Date date)
```


Belirtilen tarihten önceki çalışma gününün sonunu hesaplar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tarih | java.util.Date | Önceki çalışma gününün sonunu hesaplamak için tarih. |

**Returns:**
java.util.Date - Önceki çalışma gününün sonu
### getStartDateFromFinishAndDuration(Date finish, Duration duration) {#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, Duration duration)
```


Belirtilen bitiş tarihi ve sürece göre başlangıç tarihini döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bitiş | java.util.Date | Belirtilen bitiş tarihi. |
| duration | [Duration](../../com.aspose.tasks/duration) | Belirtilen süre. |

**Returns:**
java.util.Date - Hesaplanmış başlangıç tarihi.
### getStartDateFromFinishAndDuration(Date finish, double duration) {#getStartDateFromFinishAndDuration-java.util.Date-double-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, double duration)
```


Belirtilen bitiş tarihi ve sürece göre başlangıç tarihini döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bitiş | java.util.Date | Belirtilen bitiş tarihi. |
| süre | double | Belirtilen süre. |

**Returns:**
java.util.Date - Hesaplanmış başlangıç tarihi.
### getTaskFinishDateFromDuration(Task task, double duration) {#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-}
```
public abstract Date getTaskFinishDateFromDuration(Task task, double duration)
```


Görevin başlangıç tarihi, bölünmüş parçaları ve çalışma süresinden görev bitiş tarih ve saatini hesaplar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Bitiş tarihini hesaplamak için görev. |
|  | süre | double | Hesaplanacak süre. |

Görev özet ise, null ise veya başlangıç tarihi ayarlanmamışsa DateTime.MinValue döndürür. |

**Returns:**
java.util.Date - Verilen başlangıç tarihi ve süre için görevin bitiş tarihi.
### getWorkStart(Date date) {#getWorkStart-java.util.Date-}
```
public abstract Date getWorkStart(Date date)
```


Belirtilen tarih ve saatten itibaren bir sonraki çalışma zamanının başlangıcını hesaplar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tarih | java.util.Date | Tarih ve saat. |

**Returns:**
java.util.Date - En yakın çalışma zamanı başlangıcı.
### getWorkingHours(Date dt) {#getWorkingHours-java.util.Date-}
```
public abstract double getWorkingHours(Date dt)
```


Belirtilen tarihteki çalışma saat miktarını döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dt | java.util.Date | Çalışma saatlerini almak için tarih. |

**Returns:**
double - Belirtilen tarihteki çalışma saatleri.
### getWorkingHours(Date start, Date finish) {#getWorkingHours-java.util.Date-java.util.Date-}
```
public abstract WorkUnit getWorkingHours(Date start, Date finish)
```


WorkUnit'i döndür - Belirtilen tarih saat aralığı için çalışma saatlerinin Başlangıcı, Bitişi ve Süresi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlat | java.util.Date | Aralığın başlangıç tarihi. |
| bitiş | java.util.Date | Aralığın bitiş tarihi. |

**Returns:**
[WorkUnit](../../com.aspose.tasks/workunit) - Instance of [WorkUnit](../../com.aspose.tasks/workunit) class containing Start, Finish and Duration of working hours.
### getWorkingHoursTimeSpan(Date start, Date finish) {#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-}
```
public abstract double getWorkingHoursTimeSpan(Date start, Date finish)
```


Belirtilen tarihler arasındaki çalışma saat miktarını döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlat | java.util.Date | Aralığın başlangıç tarihi. |
| bitiş | java.util.Date | Aralığın bitiş tarihi. |

**Returns:**
double - Takvim örneğine göre çalışma saatlerinin miktarı.
### getWorkingTimes(Date dt) {#getWorkingTimes-java.util.Date-}
```
public abstract WorkingTimeCollection getWorkingTimes(Date dt)
```


Belirtilen tarih için çalışma zamanlarının [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) nesnesini döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dt | java.util.Date | Çalışma zamanlarını almak için tarih. |

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - Collection of [WorkingTime](../../com.aspose.tasks/workingtime) instances.
### isDayWorking(Date dt) {#isDayWorking-java.util.Date-}
```
public abstract boolean isDayWorking(Date dt)
```


Takvime göre belirtilen günün çalışma günü olup olmadığını belirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dt | java.util.Date | Günün çalışma günü olup olmadığını kontrol etmek için tarih. |

**Returns:**
boolean - Gün bir çalışma günü ise doğru.
### isEmpty() {#isEmpty--}
```
public abstract boolean isEmpty()
```


Takvimin tanımlı çalışma saatleri olup olmadığını döndürür.

**Returns:**
boolean - Takvimde çalışma saatleri tanımlı değilse True.
