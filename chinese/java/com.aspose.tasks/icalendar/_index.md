---
title: "ICalendar"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示可用于各种日期和持续时间计算的日历抽象。"
type: docs
weight: 376
url: /zh/java/com.aspose.tasks/icalendar/
---
```
public interface ICalendar
```

表示可用于各种日期和持续时间计算的日历抽象。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getFinishDateByStartAndWork(Date start, Duration work)](#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-) | 根据日历计算指定工作时间量耗尽时的日期。 |
| [getFinishDateByStartAndWork(Date start, double work)](#getFinishDateByStartAndWork-java.util.Date-double-) | 根据日历计算指定工作时间量耗尽时的日期。 |
| [getNextWorkingDayStart(Date date)](#getNextWorkingDayStart-java.util.Date-) | 计算指定日期的下一个工作日开始时间。 |
| [getPreviousWorkingDayEnd(Date date)](#getPreviousWorkingDayEnd-java.util.Date-) | 计算从指定日期起的前一个工作日的结束时间。 |
| [getStartDateFromFinishAndDuration(Date finish, Duration duration)](#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-) | 根据指定的结束日期和持续时间返回开始日期。 |
| [getStartDateFromFinishAndDuration(Date finish, double duration)](#getStartDateFromFinishAndDuration-java.util.Date-double-) | 根据指定的结束日期和持续时间返回开始日期。 |
| [getTaskFinishDateFromDuration(Task task, double duration)](#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-) | 根据任务的开始日期、拆分部分和工作持续时间计算任务的完成日期和时间。 |
| [getWorkStart(Date date)](#getWorkStart-java.util.Date-) | 从指定的日期和时间开始计算下一个工作时间的开始。 |
| [getWorkingHours(Date dt)](#getWorkingHours-java.util.Date-) | 返回指定日期的工作小时数。 |
| [getWorkingHours(Date start, Date finish)](#getWorkingHours-java.util.Date-java.util.Date-) | 返回 WorkUnit - 指定日期时间间隔的工作小时的开始、结束和持续时间。 |
| [getWorkingHoursTimeSpan(Date start, Date finish)](#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-) | 返回指定日期之间的工作小时数。 |
| [getWorkingTimes(Date dt)](#getWorkingTimes-java.util.Date-) | 返回 [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) 用于指定日期的工作时间。 |
| [isDayWorking(Date dt)](#isDayWorking-java.util.Date-) | 根据日历确定指定的日期是否为工作日。 |
| [isEmpty()](#isEmpty--) | 返回日历是否未定义工作时间。 |
### getFinishDateByStartAndWork(Date start, Duration work) {#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getFinishDateByStartAndWork(Date start, Duration work)
```


根据日历计算指定工作时间量耗尽时的日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 开始 | java.util.Date | 开始日期。 |
| work | [Duration](../../com.aspose.tasks/duration) | 工作持续时间。 |

**Returns:**
java.util.Date - 结束日期。
### getFinishDateByStartAndWork(Date start, double work) {#getFinishDateByStartAndWork-java.util.Date-double-}
```
public abstract Date getFinishDateByStartAndWork(Date start, double work)
```


根据日历计算指定工作时间量耗尽时的日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 开始 | java.util.Date | 开始日期。 |
| 工作 | double | 工作持续时间。 |

**Returns:**
java.util.Date - 结束日期。
### getNextWorkingDayStart(Date date) {#getNextWorkingDayStart-java.util.Date-}
```
public abstract Date getNextWorkingDayStart(Date date)
```


计算指定日期的下一个工作日开始时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 日期 | java.util.Date | 用于获取下一个工作日开始的日期。 |

**Returns:**
java.util.Date - 下一个工作日开始的 System.DateTime。
### getPreviousWorkingDayEnd(Date date) {#getPreviousWorkingDayEnd-java.util.Date-}
```
public abstract Date getPreviousWorkingDayEnd(Date date)
```


计算从指定日期起的前一个工作日的结束时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 日期 | java.util.Date | 用于计算前一个工作日结束的日期。 |

**Returns:**
java.util.Date - 前一个工作日结束的时间
### getStartDateFromFinishAndDuration(Date finish, Duration duration) {#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, Duration duration)
```


根据指定的结束日期和持续时间返回开始日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 完成 | java.util.Date | 指定的完成日期。 |
| duration | [Duration](../../com.aspose.tasks/duration) | 指定的持续时间。 |

**Returns:**
java.util.Date - 计算得到的开始日期。
### getStartDateFromFinishAndDuration(Date finish, double duration) {#getStartDateFromFinishAndDuration-java.util.Date-double-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, double duration)
```


根据指定的结束日期和持续时间返回开始日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 完成 | java.util.Date | 指定的完成日期。 |
| 持续时间 | double | 指定的持续时间。 |

**Returns:**
java.util.Date - 计算得到的开始日期。
### getTaskFinishDateFromDuration(Task task, double duration) {#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-}
```
public abstract Date getTaskFinishDateFromDuration(Task task, double duration)
```


根据任务的开始日期、拆分部分和工作持续时间计算任务的完成日期和时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 用于计算完成日期的任务。 |
|  | 持续时间 | double | 要计算的持续时间。 |

如果任务是汇总、为空或其开始日期未设置，则返回 DateTime.MinValue。 |

**Returns:**
java.util.Date - 给定开始日期和持续时间的任务完成日期。
### getWorkStart(Date date) {#getWorkStart-java.util.Date-}
```
public abstract Date getWorkStart(Date date)
```


从指定的日期和时间开始计算下一个工作时间的开始。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 日期 | java.util.Date | 日期和时间。 |

**Returns:**
java.util.Date - 最近的工作时间开始。
### getWorkingHours(Date dt) {#getWorkingHours-java.util.Date-}
```
public abstract double getWorkingHours(Date dt)
```


返回指定日期的工作小时数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dt | java.util.Date | 用于获取工作小时数的日期。 |

**Returns:**
double - 指定日期的工作小时数。
### getWorkingHours(Date start, Date finish) {#getWorkingHours-java.util.Date-java.util.Date-}
```
public abstract WorkUnit getWorkingHours(Date start, Date finish)
```


返回 WorkUnit - 指定日期时间间隔的工作小时的开始、结束和持续时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 开始 | java.util.Date | 区间的开始日期。 |
| 完成 | java.util.Date | 区间的结束日期。 |

**Returns:**
[WorkUnit](../../com.aspose.tasks/workunit) - Instance of [WorkUnit](../../com.aspose.tasks/workunit) class containing Start, Finish and Duration of working hours.
### getWorkingHoursTimeSpan(Date start, Date finish) {#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-}
```
public abstract double getWorkingHoursTimeSpan(Date start, Date finish)
```


返回指定日期之间的工作小时数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 开始 | java.util.Date | 区间的开始日期。 |
| 完成 | java.util.Date | 区间的结束日期。 |

**Returns:**
double - 根据日历实例的工作小时数。
### getWorkingTimes(Date dt) {#getWorkingTimes-java.util.Date-}
```
public abstract WorkingTimeCollection getWorkingTimes(Date dt)
```


返回 [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) 用于指定日期的工作时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dt | java.util.Date | 用于获取工作时间的日期。 |

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - Collection of [WorkingTime](../../com.aspose.tasks/workingtime) instances.
### isDayWorking(Date dt) {#isDayWorking-java.util.Date-}
```
public abstract boolean isDayWorking(Date dt)
```


根据日历确定指定的日期是否为工作日。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dt | java.util.Date | 用于检查该日是否为工作日的日期。 |

**Returns:**
boolean - 如果该日是工作日则为 True。
### isEmpty() {#isEmpty--}
```
public abstract boolean isEmpty()
```


返回日历是否未定义工作时间。

**Returns:**
布尔值 - 如果日历未定义工作时间，则为 True。
