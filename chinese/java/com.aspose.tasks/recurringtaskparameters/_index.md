---
title: "RecurringTaskParameters"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示用于在项目中创建循环任务的一组参数。"
type: docs
weight: 245
url: /zh/java/com.aspose.tasks/recurringtaskparameters/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskParameters
```

表示用于在项目中创建循环任务的一组参数。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [RecurringTaskParameters()](#RecurringTaskParameters--) | 初始化一个新的 [RecurringTaskParameters](../../com.aspose/tasks/recurringtaskparameters) 类实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getDuration()](#getDuration--) | 获取循环任务一次出现的持续时间。 |
| [getIgnoreResourceCalendar()](#getIgnoreResourceCalendar--) | 获取一个指示是否在任何资源可用时仍安排循环任务的值，即使它未能发生。 |
| [getRecurrencePattern()](#getRecurrencePattern--) | 获取循环任务的重复模式。 |
| [getTaskName()](#getTaskName--) | 获取循环任务的名称。 |
| [setCalendar(Project project, String calendarName)](#setCalendar-com.aspose.tasks.Project-java.lang.String-) | 为循环任务设置日历。 |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | 设置循环任务一次出现的持续时间。 |
| [setIgnoreResourceCalendar(boolean value)](#setIgnoreResourceCalendar-boolean-) | 设置一个指示是否在任何资源可用时仍安排循环任务的值，即使它未能发生。 |
| [setRecurrencePattern(RecurrencePatternBase value)](#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-) | 设置循环任务的重复模式。 |
| [setTaskName(String value)](#setTaskName-java.lang.String-) | 设置循环任务的名称。 |
### RecurringTaskParameters() {#RecurringTaskParameters--}
```
public RecurringTaskParameters()
```


初始化一个新的 [RecurringTaskParameters](../../com.aspose/tasks/recurringtaskparameters) 类实例。

### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


获取循环任务一次出现的持续时间。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - The instance of `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskparameters\#setDuration-Duration-)) class.
### getIgnoreResourceCalendar() {#getIgnoreResourceCalendar--}
```
public final boolean getIgnoreResourceCalendar()
```


获取一个指示是否在任何资源可用时仍安排循环任务的值，即使它未能发生。

**Returns:**
boolean - 一个指示是否在任何资源可用时仍安排循环任务的值，即使它未能发生。
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final RecurrencePatternBase getRecurrencePattern()
```


获取循环任务的重复模式。

--------------------

可以是 `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose.tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)) 枚举的其中一个值。

**Returns:**
[RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) - the recurrence pattern of the recurring task.
### getTaskName() {#getTaskName--}
```
public final String getTaskName()
```


获取循环任务的名称。

**Returns:**
java.lang.String - 循环任务的名称。
### setCalendar(Project project, String calendarName) {#setCalendar-com.aspose.tasks.Project-java.lang.String-}
```
public final void setCalendar(Project project, String calendarName)
```


为循环任务设置日历。该日历从项目日历集合中选择。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | 包含日历集合的项目。 |
| calendarName | java.lang.String | 日历的名称。 |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


设置循环任务一次出现的持续时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskparameters\#setDuration-Duration-)) 类的实例。 |

### setIgnoreResourceCalendar(boolean value) {#setIgnoreResourceCalendar-boolean-}
```
public final void setIgnoreResourceCalendar(boolean value)
```


设置一个指示是否在任何资源可用时仍安排循环任务的值，即使它未能发生。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个指示是否在任何资源可用时仍安排循环任务的值，即使它未能发生。 |

### setRecurrencePattern(RecurrencePatternBase value) {#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-}
```
public final void setRecurrencePattern(RecurrencePatternBase value)
```


设置循环任务的重复模式。

--------------------

可以是 `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose.tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)) 枚举的其中一个值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) | 重复任务的重复模式。 |

### setTaskName(String value) {#setTaskName-java.lang.String-}
```
public final void setTaskName(String value)
```


设置循环任务的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 重复任务的名称。 |

