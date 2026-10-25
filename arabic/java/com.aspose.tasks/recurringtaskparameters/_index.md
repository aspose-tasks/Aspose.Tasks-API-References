---
title: "RecurringTaskParameters"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل مجموعة المعلمات المستخدمة لإنشاء مهمة متكررة في مشروع."
type: docs
weight: 245
url: /ar/java/com.aspose.tasks/recurringtaskparameters/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskParameters
```

يمثل مجموعة المعلمات المستخدمة لإنشاء مهمة متكررة في مشروع.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [RecurringTaskParameters()](#RecurringTaskParameters--) | ينشئ مثيلاً جديداً من الفئة [RecurringTaskParameters](../../com.aspose/tasks/recurringtaskparameters). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getDuration()](#getDuration--) | يحصل على المدة لحدوث واحد للمهمة المتكررة. |
| [getIgnoreResourceCalendar()](#getIgnoreResourceCalendar--) | يحصل على قيمة تشير إلى ما إذا كان سيتم جدولة المهمة المتكررة حتى إذا لم تحدث عندما تكون أي موارد متاحة للعمل عليها. |
| [getRecurrencePattern()](#getRecurrencePattern--) | يحصل على نمط التكرار للمهمة المتكررة. |
| [getTaskName()](#getTaskName--) | يحصل على اسم المهمة المتكررة. |
| [setCalendar(Project project, String calendarName)](#setCalendar-com.aspose.tasks.Project-java.lang.String-) | حدد تقويماً للمهمة المتكررة. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | يضبط المدة لحدوث واحد للمهمة المتكررة. |
| [setIgnoreResourceCalendar(boolean value)](#setIgnoreResourceCalendar-boolean-) | يضبط قيمة تشير إلى ما إذا كان سيتم جدولة المهمة المتكررة حتى إذا لم تحدث عندما تكون أي موارد متاحة للعمل عليها. |
| [setRecurrencePattern(RecurrencePatternBase value)](#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-) | يضبط نمط التكرار للمهمة المتكررة. |
| [setTaskName(String value)](#setTaskName-java.lang.String-) | يضبط اسم المهمة المتكررة. |
### RecurringTaskParameters() {#RecurringTaskParameters--}
```
public RecurringTaskParameters()
```


ينشئ مثيلاً جديداً من الفئة [RecurringTaskParameters](../../com.aspose/tasks/recurringtaskparameters).

### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


يحصل على المدة لحدوث واحد للمهمة المتكررة.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - The instance of `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskparameters\#setDuration-Duration-)) class.
### getIgnoreResourceCalendar() {#getIgnoreResourceCalendar--}
```
public final boolean getIgnoreResourceCalendar()
```


يحصل على قيمة تشير إلى ما إذا كان سيتم جدولة المهمة المتكررة حتى إذا لم تحدث عندما تكون أي موارد متاحة للعمل عليها.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب جدولة المهمة المتكررة حتى إذا لم تحدث عندما تكون أي موارد متاحة للعمل عليها.
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final RecurrencePatternBase getRecurrencePattern()
```


يحصل على نمط التكرار للمهمة المتكررة.

--------------------

يمكن أن تكون واحدة من قيم تعداد `RecurrencePattern`([getRecurrencePattern()](../../com.aspose/tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose/tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)).

**Returns:**
[RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) - the recurrence pattern of the recurring task.
### getTaskName() {#getTaskName--}
```
public final String getTaskName()
```


يحصل على اسم المهمة المتكررة.

**Returns:**
java.lang.String - اسم المهمة المتكررة.
### setCalendar(Project project, String calendarName) {#setCalendar-com.aspose.tasks.Project-java.lang.String-}
```
public final void setCalendar(Project project, String calendarName)
```


قم بتعيين تقويم للمهمة المتكررة. يتم اختيار التقويم من مجموعة تقويمات المشروع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | المشروع مع مجموعة التقويمات. |
| calendarName | java.lang.String | اسم التقويم. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


يضبط المدة لحدوث واحد للمهمة المتكررة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | مثال من فئة `Duration`([getDuration()](../../com.aspose/tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose/tasks/recurringtaskparameters\#setDuration-Duration-)). |

### setIgnoreResourceCalendar(boolean value) {#setIgnoreResourceCalendar-boolean-}
```
public final void setIgnoreResourceCalendar(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان سيتم جدولة المهمة المتكررة حتى إذا لم تحدث عندما تكون أي موارد متاحة للعمل عليها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب جدولة المهمة المتكررة حتى إذا لم تحدث عندما تكون أي موارد متاحة للعمل عليها. |

### setRecurrencePattern(RecurrencePatternBase value) {#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-}
```
public final void setRecurrencePattern(RecurrencePatternBase value)
```


يضبط نمط التكرار للمهمة المتكررة.

--------------------

يمكن أن تكون واحدة من قيم تعداد `RecurrencePattern`([getRecurrencePattern()](../../com.aspose/tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose/tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) | نمط التكرار للمهمة المتكررة. |

### setTaskName(String value) {#setTaskName-java.lang.String-}
```
public final void setTaskName(String value)
```


يضبط اسم المهمة المتكررة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | اسم المهمة المتكررة. |

