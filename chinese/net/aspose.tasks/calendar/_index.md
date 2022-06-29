---
title: Calendar
second_title: Aspose.Tasks for .NET API 参考
description: 表示项目中使用的日历
type: docs
weight: 220
url: /zh/net/aspose.tasks/calendar/
---
## Calendar class

表示项目中使用的日历。

```csharp
public class Calendar
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar) { get; set; } | 获取或设置此日历所依赖的基准日历。 仅当日历不是基准日历时才适用。 读/写[`Calendar`](../calendar)。 |
| [Exceptions](../../aspose.tasks/calendar/exceptions) { get; } | 获取 CalendarExceptionCollection 对象。 与日历关联的异常集合。 |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar) { get; } | 获取指示日历是否为基准日历的值。 只读Boolean。 |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar) { get; set; } | 获取或设置一个指示日历是否为基线日历的值。 读/写Boolean。 |
| [Name](../../aspose.tasks/calendar/name) { get; set; } | 获取或设置日历的名称。 读/写String。 |
| [ParentProject](../../aspose.tasks/calendar/parentproject) { get; } | 获取此日历的父项目。 |
| [Uid](../../aspose.tasks/calendar/uid) { get; set; } | 获取或设置日历的唯一标识符。 读/写Int32。 |
| [WeekDays](../../aspose.tasks/calendar/weekdays) { get; } | 获取此日历的 WeekDaysCollection。 定义日历的工作日集合。 |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks) { get; } | 获取 WorkWeekCollections 对象。 与日历关联的工作周集合。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar)(Calendar) | 使给定的日历成为 24 小时日历。 24Hours Calendar 是一种日历，其中一周中的每一天都在全天候工作。 |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar)(Calendar) | 将给定日历设为夜班日历。 |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar)(Calendar) | 创建默认标准日历。 |
| [Delete](../../aspose.tasks/calendar/delete)() | 从项目中删除日历。 |
| override [Equals](../../aspose.tasks/calendar/equals)(object) | 返回一个值，指示此实例是否等于指定对象。 |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork#getfinishdatebystartandwork)(DateTime, Duration) | 根据日历计算将经过指定工作时间的日期。 |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | 根据日历计算将经过指定工作时间的日期。 |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode)() | 返回[`Calendar`](../calendar)类实例的哈希码。 |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart)(DateTime) | 从日期开始计算下一个工作日。 |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend)(DateTime) | 从指定日期计算上一个工作日期结束。 |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration#getstartdatefromfinishandduration)(DateTime, Duration) | 根据指定的 FinishDate 和 Duration 返回 StartDate。 |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | 根据指定的 FinishDate 和 Duration 返回 StartDate。 |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration)(Task, TimeSpan) | 从开始日期、拆分部分和持续时间计算任务完成日期和时间。 |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours#getworkinghours_1)(DateTime) | 返回该日期的工作小时数。 |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours#getworkinghours)(DateTime, DateTime) | 返回指定日期的工作时间。 |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes)(DateTime) | 返回[`WorkingTimeCollection`](../workingtimecollection)的工作时间。 |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking)(DateTime) | 判断当天是否为工作日。 |

### 评论

日历用于定义标准工作时间和非工作时间。 项目必须有一个基准日历。任务和资源可以有 它们自己的基于基准日历的非基准日历。

### 例子

如何从头开始创建简单的日历。

```csharp
[C#]
// 创建空日历
Calendar calendar = new Calendar("New calendar");
// 添加默认工作日（从 9:00 到 17:00 的 8 个工作小时）
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// 创建新的新工作日
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// 设置工作时间。只有 DateTime 的时间部分很重要
    WorkingTime wt1 = new WorkingTime();
    wt1.FromTime = new DateTime(1, 1, 1, 6, 0, 0, 0);
    wt1.ToTime = new DateTime(1, 1, 1, 12, 0, 0, 0);
    WorkingTime wt2 = new WorkingTime();
    wt2.FromTime = new DateTime(1, 1, 1, 14, 0, 0, 0);
    wt2.ToTime = new DateTime(1, 1, 1, 18, 0, 0, 0);
    myWeekDay.WorkingTimes.Add(wt1);
    myWeekDay.WorkingTimes.Add(wt2);
    myWeekDay.DayWorking = true;
calendar.Days.Add(myWeekDay);
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
// 添加周末
calendar.Days.Add(new WeekDay(DayType.Saturday));
calendar.Days.Add(new WeekDay(DayType.Sunday));
```

```csharp
[VB]
'创建空日历
Dim calendar As Calendar =  New Calendar("New calendar")
'添加默认工作日（从 9:00 到 17:00 的 8 个工作小时）
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
'创建新的新工作日
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
'设置工作时间。只有 DateTime 的时间部分很重要
    Dim wt1 As WorkingTime =  New WorkingTime()
    wt1.FromTime = New DateTime(1, 1, 1, 6, 0, 0, 0)
    wt1.ToTime = New DateTime(1, 1, 1, 12, 0, 0, 0)
    Dim wt2 As WorkingTime =  New WorkingTime()
    wt2.FromTime = New DateTime(1, 1, 1, 14, 0, 0, 0)
    wt2.ToTime = New DateTime(1, 1, 1, 18, 0, 0, 0)
    myWeekDay.WorkingTimes.Add(wt1)
    myWeekDay.WorkingTimes.Add(wt2)
    myWeekDay.DayWorking = True
calendar.Days.Add(myWeekDay)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday))
'增加周末
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

### 也可以看看

* 命名空间 [Aspose.Tasks](../../aspose.tasks)
* 部件 [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
