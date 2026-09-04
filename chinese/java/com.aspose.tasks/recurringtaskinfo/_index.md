---
title: "RecurringTaskInfo"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示项目中循环任务的详细信息。"
type: docs
weight: 244
url: /zh/java/com.aspose.tasks/recurringtaskinfo/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskInfo
```

表示项目中循环任务的详细信息。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getDailyRepetitions()](#getDailyRepetitions--) | 获取每日重复模式的重复次数。 |
| [getDailyUseWorkdays()](#getDailyUseWorkdays--) | 获取一个值，指示是否在每日重复模式中使用工作日。 |
| [getDuration()](#getDuration--) | 获取循环任务一次出现的持续时间。 |
| [getEndDate()](#getEndDate--) | 获取出现结束的日期。 |
| [getMonthlyDay()](#getMonthlyDay--) | 获取每月循环模式的天数。 |
| [getMonthlyOrdinalDay()](#getMonthlyOrdinalDay--) | 在使用序数日时，获取每月循环模式的天。 |
| [getMonthlyOrdinalNumber()](#getMonthlyOrdinalNumber--) | 获取每月循环模式的序数。 |
| [getMonthlyOrdinalRepetitions()](#getMonthlyOrdinalRepetitions--) | 在使用序数日时，获取每月循环模式的重复次数。 |
| [getMonthlyRepetitions()](#getMonthlyRepetitions--) | 获取每月循环模式的重复次数。 |
| [getMonthlyUseOrdinalDay()](#getMonthlyUseOrdinalDay--) | 获取一个值，指示是否在每月循环模式中使用序数日。 |
| [getOccurrences()](#getOccurrences--) | 获取循环任务的出现次数。 |
| [getRecurrencePattern()](#getRecurrencePattern--) | 获取循环任务的重复模式。 |
| [getStartDate()](#getStartDate--) | 获取出现开始的日期。 |
| [getTask()](#getTask--) | 获取此实例的父任务，属于 [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) 类。 |
| [getUseEndDate()](#getUseEndDate--) | 获取一个值，指示循环任务是使用结束日期还是出现次数。 |
| [getWeeklyDays()](#getWeeklyDays--) | 获取每周循环模式中使用的天集合。 |
| [getWeeklyRepetitions()](#getWeeklyRepetitions--) | 获取每周循环模式的重复次数。 |
| [getYearlyDate()](#getYearlyDate--) | 获取每年循环模式的日期。 |
| [getYearlyOrdinalDay()](#getYearlyOrdinalDay--) | 在使用序数日时，获取每年循环模式的工作日。 |
| [getYearlyOrdinalMonth()](#getYearlyOrdinalMonth--) | 在使用序数日时，获取每年循环模式的月份。 |
| [getYearlyOrdinalNumber()](#getYearlyOrdinalNumber--) | 获取每年循环模式的序数。 |
| [getYearlyUseOrdinalDay()](#getYearlyUseOrdinalDay--) | 获取一个值，指示是否在每年循环模式中使用序数日。 |
| [setDailyRepetitions(int value)](#setDailyRepetitions-int-) | 设置每日循环模式的重复次数。 |
| [setDailyUseWorkdays(boolean value)](#setDailyUseWorkdays-boolean-) | 设置一个值，指示是否在每日循环模式中使用工作日。 |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | 设置循环任务一次出现的持续时间。 |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | 设置出现结束的日期。 |
| [setMonthlyDay(int value)](#setMonthlyDay-int-) | 设置每月循环模式的天数。 |
| [setMonthlyOrdinalDay(int value)](#setMonthlyOrdinalDay-int-) | 在使用序数日时，设置每月重复模式的某一天。 |
| [setMonthlyOrdinalNumber(int value)](#setMonthlyOrdinalNumber-int-) | 设置每月重复模式的序数号。 |
| [setMonthlyOrdinalRepetitions(int value)](#setMonthlyOrdinalRepetitions-int-) | 在使用序数日时，设置每月重复模式的重复次数。 |
| [setMonthlyRepetitions(int value)](#setMonthlyRepetitions-int-) | 设置每月重复模式的重复次数。 |
| [setMonthlyUseOrdinalDay(boolean value)](#setMonthlyUseOrdinalDay-boolean-) | 设置一个值，指示是否在每月重复模式中使用序数日。 |
| [setOccurrences(int value)](#setOccurrences-int-) | 设置循环任务的出现次数。 |
| [setRecurrencePattern(int value)](#setRecurrencePattern-int-) | 设置循环任务的重复模式。 |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | 设置出现开始的日期。 |
| [setUseEndDate(boolean value)](#setUseEndDate-boolean-) | 设置一个值，指示是否在循环任务中使用结束日期或出现次数。 |
| [setWeeklyDays(int value)](#setWeeklyDays-int-) | 设置每周重复模式中使用的天集合。 |
| [setWeeklyRepetitions(int value)](#setWeeklyRepetitions-int-) | 设置每周重复模式的重复次数。 |
| [setYearlyDate(Date value)](#setYearlyDate-java.util.Date-) | 设置每年重复模式的日期。 |
| [setYearlyOrdinalDay(int value)](#setYearlyOrdinalDay-int-) | 在使用序数日时，设置每年重复模式的工作日。 |
| [setYearlyOrdinalMonth(int value)](#setYearlyOrdinalMonth-int-) | 在使用序数日时，设置每年重复模式的月份。 |
| [setYearlyOrdinalNumber(int value)](#setYearlyOrdinalNumber-int-) | 设置每年重复模式的序数号。 |
| [setYearlyUseOrdinalDay(boolean value)](#setYearlyUseOrdinalDay-boolean-) | 设置一个值，指示是否在每年重复模式中使用序数日。 |
### getDailyRepetitions() {#getDailyRepetitions--}
```
public final int getDailyRepetitions()
```


获取每日重复模式的重复次数。

**Returns:**
int - 每日重复模式的重复次数。
### getDailyUseWorkdays() {#getDailyUseWorkdays--}
```
public final boolean getDailyUseWorkdays()
```


获取一个值，指示是否在每日重复模式中使用工作日。

**Returns:**
boolean - 一个值，指示是否在每日重复模式中使用工作日。
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


获取循环任务一次出现的持续时间。

--------------------

`Duration` 类的实例（[getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-))。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration for one occurrence of the recurring task.
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


获取出现结束的日期。

**Returns:**
java.util.Date - 出现结束的日期。
### getMonthlyDay() {#getMonthlyDay--}
```
public final int getMonthlyDay()
```


获取每月循环模式的天数。

**Returns:**
int - 每月重复模式的天数。
### getMonthlyOrdinalDay() {#getMonthlyOrdinalDay--}
```
public final int getMonthlyOrdinalDay()
```


在使用序数日时，获取每月循环模式的天。

--------------------

可以是 [DayOfWeek](../../com.aspose.tasks/dayofweek) 枚举的一个值。

**Returns:**
int - 在使用序数日时，每月重复模式的天数。
### getMonthlyOrdinalNumber() {#getMonthlyOrdinalNumber--}
```
public final int getMonthlyOrdinalNumber()
```


获取每月循环模式的序数。

--------------------

可以是 [OrdinalNumber](../../com.aspose.tasks/ordinalnumber) 枚举的一个值。

**Returns:**
int - 每月重复模式的序数号。
### getMonthlyOrdinalRepetitions() {#getMonthlyOrdinalRepetitions--}
```
public final int getMonthlyOrdinalRepetitions()
```


在使用序数日时，获取每月循环模式的重复次数。

**Returns:**
int - 使用序数日时的月度重复模式的重复次数。
### getMonthlyRepetitions() {#getMonthlyRepetitions--}
```
public final int getMonthlyRepetitions()
```


获取每月循环模式的重复次数。

**Returns:**
int - 月度重复模式的重复次数。
### getMonthlyUseOrdinalDay() {#getMonthlyUseOrdinalDay--}
```
public final boolean getMonthlyUseOrdinalDay()
```


获取一个值，指示是否在每月循环模式中使用序数日。

**Returns:**
boolean - 指示是否在月度重复模式中使用序数日的值。
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


获取循环任务的出现次数。

**Returns:**
int - 循环任务的出现次数。
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final int getRecurrencePattern()
```


获取循环任务的重复模式。

--------------------

可以是 `RecurrencePattern`([getRecurrencePattern()](../../com.aspose/tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose/tasks/recurringtaskinfo\#setRecurrencePattern-int-)) 枚举的其中一个值。

**Returns:**
int - 循环任务的重复模式。
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


获取出现开始的日期。

**Returns:**
java.util.Date - 事件开始的日期。
### getTask() {#getTask--}
```
public final Task getTask()
```


获取此实例的父任务，属于 [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) 类。

**Returns:**
[Task](../../com.aspose.tasks/task) - the parent task of this instance of [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) class.
### getUseEndDate() {#getUseEndDate--}
```
public final boolean getUseEndDate()
```


获取一个值，指示循环任务是使用结束日期还是出现次数。

**Returns:**
boolean - 指示是否为循环任务使用结束日期或出现次数的值。
### getWeeklyDays() {#getWeeklyDays--}
```
public final int getWeeklyDays()
```


获取每周循环模式中使用的天集合。

--------------------

**Returns:**
int - 用于每周重复模式的天集合。
### getWeeklyRepetitions() {#getWeeklyRepetitions--}
```
public final int getWeeklyRepetitions()
```


获取每周循环模式的重复次数。

**Returns:**
int - 每周重复模式的重复次数。
### getYearlyDate() {#getYearlyDate--}
```
public final Date getYearlyDate()
```


获取每年循环模式的日期。

**Returns:**
java.util.Date - 年度重复模式的日期。
### getYearlyOrdinalDay() {#getYearlyOrdinalDay--}
```
public final int getYearlyOrdinalDay()
```


在使用序数日时，获取每年循环模式的工作日。

--------------------

可以是 [DayOfWeek](../../com.aspose.tasks/dayofweek) 枚举的一个值。

**Returns:**
int - 使用序数日时的年度重复模式的工作日。
### getYearlyOrdinalMonth() {#getYearlyOrdinalMonth--}
```
public final int getYearlyOrdinalMonth()
```


在使用序数日时，获取每年循环模式的月份。

--------------------

可以是 [Month](../../com.aspose/tasks/month) 枚举的其中一个值。

**Returns:**
int - 使用序数日时的年度重复模式的月份。
### getYearlyOrdinalNumber() {#getYearlyOrdinalNumber--}
```
public final int getYearlyOrdinalNumber()
```


获取每年循环模式的序数。

--------------------

可以是 [OrdinalNumber](../../com.aspose.tasks/ordinalnumber) 枚举的一个值。

**Returns:**
int - 年度重复模式的序数。
### getYearlyUseOrdinalDay() {#getYearlyUseOrdinalDay--}
```
public final boolean getYearlyUseOrdinalDay()
```


获取一个值，指示是否在每年循环模式中使用序数日。

**Returns:**
boolean - 指示是否在年度重复模式中使用序数日的值。
### setDailyRepetitions(int value) {#setDailyRepetitions-int-}
```
public final void setDailyRepetitions(int value)
```


设置每日循环模式的重复次数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 每日重复模式的重复次数。 |

### setDailyUseWorkdays(boolean value) {#setDailyUseWorkdays-boolean-}
```
public final void setDailyUseWorkdays(boolean value)
```


设置一个值，指示是否在每日循环模式中使用工作日。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示是否在每日重复模式中使用工作日的值。 |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


设置循环任务一次出现的持续时间。

--------------------

`Duration` 类的实例（[getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-))。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | 循环任务一次出现的持续时间。 |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


设置出现结束的日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 事件结束的日期。 |

### setMonthlyDay(int value) {#setMonthlyDay-int-}
```
public final void setMonthlyDay(int value)
```


设置每月循环模式的天数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 月度重复模式的天数。 |

### setMonthlyOrdinalDay(int value) {#setMonthlyOrdinalDay-int-}
```
public final void setMonthlyOrdinalDay(int value)
```


在使用序数日时，设置每月重复模式的某一天。

--------------------

可以是 [DayOfWeek](../../com.aspose.tasks/dayofweek) 枚举的一个值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 使用序数日时的月度重复模式的天。 |

### setMonthlyOrdinalNumber(int value) {#setMonthlyOrdinalNumber-int-}
```
public final void setMonthlyOrdinalNumber(int value)
```


设置每月重复模式的序数号。

--------------------

可以是 [OrdinalNumber](../../com.aspose.tasks/ordinalnumber) 枚举的一个值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 月度重复模式的序数。 |

### setMonthlyOrdinalRepetitions(int value) {#setMonthlyOrdinalRepetitions-int-}
```
public final void setMonthlyOrdinalRepetitions(int value)
```


在使用序数日时，设置每月重复模式的重复次数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 使用序数日时的月度重复模式的重复次数。 |

### setMonthlyRepetitions(int value) {#setMonthlyRepetitions-int-}
```
public final void setMonthlyRepetitions(int value)
```


设置每月重复模式的重复次数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 月度重复模式的重复次数。 |

### setMonthlyUseOrdinalDay(boolean value) {#setMonthlyUseOrdinalDay-boolean-}
```
public final void setMonthlyUseOrdinalDay(boolean value)
```


设置一个值，指示是否在每月重复模式中使用序数日。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示是否在月度重复模式中使用序数日的值。 |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


设置循环任务的出现次数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 重复任务的出现次数。 |

### setRecurrencePattern(int value) {#setRecurrencePattern-int-}
```
public final void setRecurrencePattern(int value)
```


设置循环任务的重复模式。

--------------------

可以是 `RecurrencePattern`([getRecurrencePattern()](../../com.aspose/tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose/tasks/recurringtaskinfo\#setRecurrencePattern-int-)) 枚举的其中一个值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 重复任务的重复模式。 |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


设置出现开始的日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 出现开始的日期。 |

### setUseEndDate(boolean value) {#setUseEndDate-boolean-}
```
public final void setUseEndDate(boolean value)
```


设置一个值，指示是否在循环任务中使用结束日期或出现次数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示是否为重复任务使用结束日期或出现次数的值。 |

### setWeeklyDays(int value) {#setWeeklyDays-int-}
```
public final void setWeeklyDays(int value)
```


设置每周重复模式中使用的天集合。

--------------------

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 在每周重复模式中使用的天集合。 |

### setWeeklyRepetitions(int value) {#setWeeklyRepetitions-int-}
```
public final void setWeeklyRepetitions(int value)
```


设置每周重复模式的重复次数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 每周重复模式的重复次数。 |

### setYearlyDate(Date value) {#setYearlyDate-java.util.Date-}
```
public final void setYearlyDate(Date value)
```


设置每年重复模式的日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 年度重复模式的日期。 |

### setYearlyOrdinalDay(int value) {#setYearlyOrdinalDay-int-}
```
public final void setYearlyOrdinalDay(int value)
```


在使用序数日时，设置每年重复模式的工作日。

--------------------

可以是 [DayOfWeek](../../com.aspose.tasks/dayofweek) 枚举的一个值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 使用序数日时，年度重复模式的工作日。 |

### setYearlyOrdinalMonth(int value) {#setYearlyOrdinalMonth-int-}
```
public final void setYearlyOrdinalMonth(int value)
```


在使用序数日时，设置每年重复模式的月份。

--------------------

可以是 [Month](../../com.aspose/tasks/month) 枚举的其中一个值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 使用序数日时，年度重复模式的月份。 |

### setYearlyOrdinalNumber(int value) {#setYearlyOrdinalNumber-int-}
```
public final void setYearlyOrdinalNumber(int value)
```


设置每年重复模式的序数号。

--------------------

可以是 [OrdinalNumber](../../com.aspose.tasks/ordinalnumber) 枚举的一个值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 年度重复模式的序数。 |

### setYearlyUseOrdinalDay(boolean value) {#setYearlyUseOrdinalDay-boolean-}
```
public final void setYearlyUseOrdinalDay(boolean value)
```


设置一个值，指示是否在每年重复模式中使用序数日。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示是否在年度重复模式中使用序数日的值。 |

