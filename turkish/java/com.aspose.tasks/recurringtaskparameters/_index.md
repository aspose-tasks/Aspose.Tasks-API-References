---
title: "RecurringTaskParameters"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Projede bir yineleyen görev oluşturmak için kullanılan parametre kümesini temsil eder."
type: docs
weight: 245
url: /tr/java/com.aspose.tasks/recurringtaskparameters/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskParameters
```

Projede bir yineleyen görev oluşturmak için kullanılan parametre kümesini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [RecurringTaskParameters()](#RecurringTaskParameters--) | Yeni bir [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters) sınıfının örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getDuration()](#getDuration--) | Yinelenen görevin bir gerçekleşmesi için süresi alır. |
| [getIgnoreResourceCalendar()](#getIgnoreResourceCalendar--) | Kaynakların görev üzerinde çalışabilir olduğu zaman gerçekleşmese bile yinelenen görevi zamanlayıp zamanlamayacağını gösteren bir değeri alır. |
| [getRecurrencePattern()](#getRecurrencePattern--) | Yinelenen görevin yineleme desenini alır. |
| [getTaskName()](#getTaskName--) | Yinelenen görevin adını alır. |
| [setCalendar(Project project, String calendarName)](#setCalendar-com.aspose.tasks.Project-java.lang.String-) | Yinelenen görev için bir takvim ayarlar. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Yineleyen görevin bir oluşumu için süresi ayarlar. |
| [setIgnoreResourceCalendar(boolean value)](#setIgnoreResourceCalendar-boolean-) | Kaynakların görev üzerinde çalışabilir olduğu zaman gerçekleşmese bile yinelenen görevi zamanlayıp zamanlamayacağını gösteren bir değeri ayarlar. |
| [setRecurrencePattern(RecurrencePatternBase value)](#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-) | Yinelenen görevin yineleme desenini ayarlar. |
| [setTaskName(String value)](#setTaskName-java.lang.String-) | Yinelenen görevin adını ayarlar. |
### RecurringTaskParameters() {#RecurringTaskParameters--}
```
public RecurringTaskParameters()
```


Yeni bir [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters) sınıfının örneğini başlatır.

### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Yinelenen görevin bir gerçekleşmesi için süresi alır.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - The instance of `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskparameters\#setDuration-Duration-)) class.
### getIgnoreResourceCalendar() {#getIgnoreResourceCalendar--}
```
public final boolean getIgnoreResourceCalendar()
```


Kaynakların görev üzerinde çalışabilir olduğu zaman gerçekleşmese bile yinelenen görevi zamanlayıp zamanlamayacağını gösteren bir değeri alır.

**Returns:**
boolean - bir değer, tekrarlayan görevi, kaynaklar mevcut olduğunda gerçekleşmese bile zamanlamayı gösterir.
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final RecurrencePatternBase getRecurrencePattern()
```


Yinelenen görevin yineleme desenini alır.

--------------------

`RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose.tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)) enum'ının değerlerinden biri olabilir.

**Returns:**
[RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) - the recurrence pattern of the recurring task.
### getTaskName() {#getTaskName--}
```
public final String getTaskName()
```


Yinelenen görevin adını alır.

**Returns:**
java.lang.String - tekrarlayan görevin adı.
### setCalendar(Project project, String calendarName) {#setCalendar-com.aspose.tasks.Project-java.lang.String-}
```
public final void setCalendar(Project project, String calendarName)
```


Tekrarlayan görev için bir takvim ayarlayın. Takvim, proje takvim koleksiyonundan seçilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Takvim koleksiyonuna sahip proje. |
| calendarName | java.lang.String | Takvimin adı. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Yineleyen görevin bir oluşumu için süresi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskparameters\#setDuration-Duration-)) sınıfının bir örneği. |

### setIgnoreResourceCalendar(boolean value) {#setIgnoreResourceCalendar-boolean-}
```
public final void setIgnoreResourceCalendar(boolean value)
```


Kaynakların görev üzerinde çalışabilir olduğu zaman gerçekleşmese bile yinelenen görevi zamanlayıp zamanlamayacağını gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | bir değer, kaynaklar mevcut olduğunda gerçekleşmese bile tekrarlayan görevi zamanlayıp zamanlamayacağını gösterir. |

### setRecurrencePattern(RecurrencePatternBase value) {#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-}
```
public final void setRecurrencePattern(RecurrencePatternBase value)
```


Yinelenen görevin yineleme desenini ayarlar.

--------------------

`RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose.tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)) enum'ının değerlerinden biri olabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) | tekrarlayan görevin yineleme deseni. |

### setTaskName(String value) {#setTaskName-java.lang.String-}
```
public final void setTaskName(String value)
```


Yinelenen görevin adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | tekrarlayan görevin adı. |

