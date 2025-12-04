---
title: RecurringTaskParameters
second_title: Aspose.Tasks for Java API Reference
description: Represents the set of parameters are used to create a recurring task in a project.
type: docs
weight: 244
url: /java/com.aspose.tasks/recurringtaskparameters/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskParameters
```

Represents the set of parameters are used to create a recurring task in a project.
## Constructors

| Constructor | Description |
| --- | --- |
| [RecurringTaskParameters()](#RecurringTaskParameters--) | Initializes a new instance of the [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters) class. |
## Methods

| Method | Description |
| --- | --- |
| [getDuration()](#getDuration--) | Gets the duration for one occurrence of the recurring task. |
| [getIgnoreResourceCalendar()](#getIgnoreResourceCalendar--) | Gets a value indicating whether to schedule the recurring task even if it does not happen when any resources are available to work on it. |
| [getRecurrencePattern()](#getRecurrencePattern--) | Gets the recurrence pattern of the recurring task. |
| [getTaskName()](#getTaskName--) | Gets the name of the recurring task. |
| [setCalendar(Project project, String calendarName)](#setCalendar-com.aspose.tasks.Project-java.lang.String-) | Set a calendar for recurring task. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Sets the duration for one occurrence of the recurring task. |
| [setIgnoreResourceCalendar(boolean value)](#setIgnoreResourceCalendar-boolean-) | Sets a value indicating whether to schedule the recurring task even if it does not happen when any resources are available to work on it. |
| [setRecurrencePattern(RecurrencePatternBase value)](#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-) | Sets the recurrence pattern of the recurring task. |
| [setTaskName(String value)](#setTaskName-java.lang.String-) | Sets the name of the recurring task. |
### RecurringTaskParameters() {#RecurringTaskParameters--}
```
public RecurringTaskParameters()
```


Initializes a new instance of the [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters) class.

### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Gets the duration for one occurrence of the recurring task.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - The instance of `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskparameters\#setDuration-Duration-)) class.
### getIgnoreResourceCalendar() {#getIgnoreResourceCalendar--}
```
public final boolean getIgnoreResourceCalendar()
```


Gets a value indicating whether to schedule the recurring task even if it does not happen when any resources are available to work on it.

**Returns:**
boolean - a value indicating whether to schedule the recurring task even if it does not happen when any resources are available to work on it.
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final RecurrencePatternBase getRecurrencePattern()
```


Gets the recurrence pattern of the recurring task.

--------------------

Can be one of the values of `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose.tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)) enumeration.

**Returns:**
[RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) - the recurrence pattern of the recurring task.
### getTaskName() {#getTaskName--}
```
public final String getTaskName()
```


Gets the name of the recurring task.

**Returns:**
java.lang.String - the name of the recurring task.
### setCalendar(Project project, String calendarName) {#setCalendar-com.aspose.tasks.Project-java.lang.String-}
```
public final void setCalendar(Project project, String calendarName)
```


Set a calendar for recurring task. The calendar is selected from project calendar collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | The project with calendar collection. |
| calendarName | java.lang.String | The name of calendar. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Sets the duration for one occurrence of the recurring task.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | The instance of `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskparameters\#setDuration-Duration-)) class. |

### setIgnoreResourceCalendar(boolean value) {#setIgnoreResourceCalendar-boolean-}
```
public final void setIgnoreResourceCalendar(boolean value)
```


Sets a value indicating whether to schedule the recurring task even if it does not happen when any resources are available to work on it.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to schedule the recurring task even if it does not happen when any resources are available to work on it. |

### setRecurrencePattern(RecurrencePatternBase value) {#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-}
```
public final void setRecurrencePattern(RecurrencePatternBase value)
```


Sets the recurrence pattern of the recurring task.

--------------------

Can be one of the values of `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose.tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)) enumeration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) | the recurrence pattern of the recurring task. |

### setTaskName(String value) {#setTaskName-java.lang.String-}
```
public final void setTaskName(String value)
```


Sets the name of the recurring task.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the name of the recurring task. |

