---
title: "TaskBaseline"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Bir görevin Temel Çizgisini temsil eder."
type: docs
weight: 291
url: /tr/java/com.aspose.tasks/taskbaseline/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.Baseline](../../com.aspose.tasks/baseline)

**All Implemented Interfaces:**
java.lang.Comparable
```
public class TaskBaseline extends Baseline implements Comparable<Baseline>
```

Bir görevin Temel Çizgisini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [TaskBaseline(Task task)](#TaskBaseline-com.aspose.tasks.Task-) | Yeni bir [TaskBaseline](../../com.aspose.tasks/taskbaseline) sınıf örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [compareTo(TaskBaseline other)](#compareTo-com.aspose.tasks.TaskBaseline-) | IComparable arabirimi uygulaması. |
| [equals(TaskBaseline other)](#equals-com.aspose.tasks.TaskBaseline-) | Bu örneğin belirtilen TaskBaseline nesnesine eşit olup olmadığını gösteren bir değer döndürür. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür. |
| [getDuration()](#getDuration--) | Temel çizelge kaydedildiğinde görevin planlanan süresini alır. |
| [getEstimatedDuration()](#getEstimatedDuration--) | Görevin temel çizelge süresinin tahmini olup olmadığını gösteren bir değer alır. |
| [getFinish()](#getFinish--) | Temel çizelge kaydedildiğinde görevin planlanan bitiş tarihini alır. |
| [getFixedCost()](#getFixedCost--) | Temel çizelge kaydedildiğinde görevin sabit maliyetini alır. |
| [getInterim()](#getInterim--) | Bunun ara temel çizelge olup olmadığını gösteren bir değer alır. |
| [getStart()](#getStart--) | Temel çizelge kaydedildiğinde görevin planlanan başlangıç tarihini alır. |
| [getTimephasedData()](#getTimephasedData--) | Bu nesne için bir TimephasedDataCollection örneği alır. |
| [hashCode()](#hashCode--) | [TaskBaseline](../../com.aspose.tasks/taskbaseline) sınıfının örneği için bir karma kod değeri döndürür. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Temel çizelge kaydedildiğinde görevin planlanan süresini ayarlar. |
| [setEstimatedDuration(boolean value)](#setEstimatedDuration-boolean-) | Görevin temel çizelge süresinin tahmini olup olmadığını gösteren bir değeri ayarlar. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Temel çizelge kaydedildiğinde görevin planlanan bitiş tarihini ayarlar. |
| [setFixedCost(double value)](#setFixedCost-double-) | Temel çizgi kaydedildiğinde görevin sabit maliyetini ayarlar. |
| [setInterim(boolean value)](#setInterim-boolean-) | Bunun Ara Temel Çizgi olup olmadığını gösteren bir değeri ayarlar. |
| [setStart(Date value)](#setStart-java.util.Date-) | Temel çizgi kaydedildiğinde görevin planlanan başlangıç tarihini ayarlar. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Bu nesne için bir TimephasedDataCollection örneği ayarlar. |
### TaskBaseline(Task task) {#TaskBaseline-com.aspose.tasks.Task-}
```
public TaskBaseline(Task task)
```


Yeni bir [TaskBaseline](../../com.aspose.tasks/taskbaseline) sınıf örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Temel çizginin üst görev. |

### compareTo(TaskBaseline other) {#compareTo-com.aspose.tasks.TaskBaseline-}
```
public final int compareTo(TaskBaseline other)
```


IComparable arabirimi uygulaması. Bu örneği belirtilen Baseline nesnesiyle karşılaştırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | bu örneğin karşılaştırılacağı belirtilen Baseline nesnesi. |

**Returns:**
int - bu örnek belirtilen nesneden küçükse -1, büyükse 1 döndürür; aksi takdirde 0 döndürür.
### equals(TaskBaseline other) {#equals-com.aspose.tasks.TaskBaseline-}
```
public final boolean equals(TaskBaseline other)
```


Bu örneğin belirtilen TaskBaseline nesnesine eşit olup olmadığını gösteren bir değer döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | Bu örnekle karşılaştırılacak belirtilen AssignmentBaseline nesnesi. |

**Returns:**
boolean - bu örnek belirtilen TaskBaseline nesnesine eşitse true döndürür; aksi takdirde false.
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
boolean - **True** eğer belirtilen nesne bu örnekle aynı UID değerine sahip bir TaskBaseline ise; aksi takdirde **false**.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Temel çizelge kaydedildiğinde görevin planlanan süresini alır.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the scheduled duration of the task when the baseline was saved.
### getEstimatedDuration() {#getEstimatedDuration--}
```
public final boolean getEstimatedDuration()
```


Görevin temel çizelge süresinin tahmini olup olmadığını gösteren bir değer alır.

**Returns:**
boolean - görevin temel çizgi süresinin tahmin edilip edilmediğini gösteren bir değer.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Temel çizelge kaydedildiğinde görevin planlanan bitiş tarihini alır.

**Returns:**
java.util.Date - temel çizgi kaydedildiğinde görevin planlanan bitiş tarihi.
### getFixedCost() {#getFixedCost--}
```
public final double getFixedCost()
```


Temel çizelge kaydedildiğinde görevin sabit maliyetini alır.

**Returns:**
double - temel çizgi kaydedildiğinde görevin sabit maliyeti.
### getInterim() {#getInterim--}
```
public final boolean getInterim()
```


Bunun ara temel çizelge olup olmadığını gösteren bir değer alır.

**Returns:**
boolean - bunun bir Ara Temel Çizgi olup olmadığını gösteren bir değer.
### getStart() {#getStart--}
```
public final Date getStart()
```


Temel çizelge kaydedildiğinde görevin planlanan başlangıç tarihini alır.

**Returns:**
java.util.Date - temel çizgi kaydedildiğinde görevin planlanan başlangıç tarihi.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Bu nesne için bir TimephasedDataCollection örneği alır. Görev temel çizgisiyle ilişkili zaman aşamalı veri.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - a TimephasedDataCollection instance for this object.
### hashCode() {#hashCode--}
```
public int hashCode()
```


[TaskBaseline](../../com.aspose.tasks/taskbaseline) sınıfının örneği için bir karma kod değeri döndürür.

**Returns:**
int - bu nesne için bir karma kod değeri döndürür.
### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Temel çizelge kaydedildiğinde görevin planlanan süresini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | temel çizgi kaydedildiğinde görevin planlanan süresi. |

### setEstimatedDuration(boolean value) {#setEstimatedDuration-boolean-}
```
public final void setEstimatedDuration(boolean value)
```


Görevin temel çizelge süresinin tahmini olup olmadığını gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | görevin temel çizgi süresinin tahmin edilip edilmediğini gösteren bir değer. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Temel çizelge kaydedildiğinde görevin planlanan bitiş tarihini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | temel çizgi kaydedildiğinde görevin planlanan bitiş tarihi. |

### setFixedCost(double value) {#setFixedCost-double-}
```
public final void setFixedCost(double value)
```


Temel çizgi kaydedildiğinde görevin sabit maliyetini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | temel çizgi kaydedildiğinde görevin sabit maliyeti. |

### setInterim(boolean value) {#setInterim-boolean-}
```
public final void setInterim(boolean value)
```


Bunun Ara Temel Çizgi olup olmadığını gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | bunun bir Ara Temel Çizgi olup olmadığını gösteren bir değer. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Temel çizgi kaydedildiğinde görevin planlanan başlangıç tarihini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | temel çizgi kaydedildiğinde görevin planlanan başlangıç tarihi. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Bu nesne için bir TimephasedDataCollection örneği ayarlar. Görev temel çizgisiyle ilişkili zaman aşamalı veri.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | Bu nesne için bir TimephasedDataCollection örneği. |

