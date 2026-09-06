---
title: "WorkingTime"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Hafta içi bir gün içinde çalışma zamanını temsil eder."
type: docs
weight: 365
url: /tr/java/com.aspose.tasks/workingtime/
---

**Inheritance:**
java.lang.Object
```
public class WorkingTime
```

Hafta içi bir gün içinde çalışma zamanını temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [WorkingTime(Date fromTime, Date toTime)](#WorkingTime-java.util.Date-java.util.Date-) | Belirtilen başlangıç ve bitiş zamanlarıyla bir aralık kullanarak [WorkingTime](../../com.aspose.tasks/workingtime) sınıfının yeni bir örneğini başlatır. |
| [WorkingTime(double fromTime, double toTime)](#WorkingTime-double-double-) | Belirtilen başlangıç ve bitiş zamanlarıyla bir aralık öğesi kullanarak [WorkingTime](../../com.aspose.tasks/workingtime) sınıfının yeni bir örneğini başlatır. |
| [WorkingTime(int fromHours, int toHours)](#WorkingTime-int-int-) | Belirtilen başlangıç ve bitiş zamanlarıyla bir aralık öğesi kullanarak [WorkingTime](../../com.aspose.tasks/workingtime) sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Nesnelerin eşit olduğunu kontrol eder. |
| [getFrom()](#getFrom--) | Bir çalışma zamanının başlangıcını alır. |
| [getTo()](#getTo--) | Bir çalışma zamanının sonunu alır. |
| [hashCode()](#hashCode--) | [WorkingTime](../../com.aspose.tasks/workingtime) sınıfının örneği için bir hash kod değeri döndürür. |
### WorkingTime(Date fromTime, Date toTime) {#WorkingTime-java.util.Date-java.util.Date-}
```
public WorkingTime(Date fromTime, Date toTime)
```


Belirtilen başlangıç ve bitiş zamanlarıyla bir aralık kullanarak [WorkingTime](../../com.aspose.tasks/workingtime) sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fromTime | java.util.Date | aralık başlangıç zamanı |
| toTime | java.util.Date | aralık bitiş zamanı |

### WorkingTime(double fromTime, double toTime) {#WorkingTime-double-double-}
```
public WorkingTime(double fromTime, double toTime)
```


Belirtilen başlangıç ve bitiş zamanlarıyla bir aralık öğesi kullanarak [WorkingTime](../../com.aspose.tasks/workingtime) sınıfının yeni bir örneğini başlatır.

--------------------

&gt; ```
&gt; WorkingTime ctor aşırı yüklemesi, aralığın başlangıç ve bitişini TimeSpan'ler kullanarak başlatmak için kullanılabilir:
&gt; ``````

 [C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fromTime | double | Interval's start time represented by double struct. |
| toTime | double | Interval's end time represented by double struct. |

### WorkingTime(int fromHours, int toHours) {#WorkingTime-int-int-}
```
public WorkingTime(int fromHours, int toHours)
```


Initializes a new instance of the [WorkingTime](../../com.aspose.tasks/workingtime) class with an interval item with the specified start and finish times.

--------------------

&gt; ```
&gt; The overload of WorkingTime ctor can be used to initialize interval's start and end using whole hours:
&gt; ``````

 [C#]
 var wt = new WorkingTime(9, 13);
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fromHours | int | Aralığın başlangıç zamanı, tam saat sayısı (0-24) olarak temsil edilir. |
| toHours | int | Aralığın bitiş zamanı, tam saat sayısı (0-24) olarak temsil edilir. |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Nesnelerin eşit olduğunu kontrol eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object | Karşılaştırılacak ikinci nesne. |

**Returns:**
boolean - Nesneler eşitse True, aksi takdirde false.
### getFrom() {#getFrom--}
```
public final Date getFrom()
```


Bir çalışma zamanının başlangıcını alır.

**Returns:**
java.util.Date - bir çalışma zamanının başlangıcı.
### getTo() {#getTo--}
```
public final Date getTo()
```


Bir çalışma zamanının sonunu alır.

**Returns:**
java.util.Date - bir çalışma zamanının sonu.
### hashCode() {#hashCode--}
```
public int hashCode()
```


[WorkingTime](../../com.aspose.tasks/workingtime) sınıfının örneği için bir hash kod değeri döndürür.

**Returns:**
int - bu nesne için bir karma kod değeri döndürür.
