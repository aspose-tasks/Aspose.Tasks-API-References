---
title: "类 Calendar"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Calendar 类。表示项目中使用的日历"
type: docs
weight: 230
url: /zh/net/aspose.tasks/calendar/
---
## Calendar class

表示项目中使用的日历。

```csharp
public class Calendar : ICalendar
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar/) { get; set; } | 获取或设置此日历所依赖的基础日历。仅在该日历不是基础日历时适用。 |
| [Exceptions](../../aspose.tasks/calendar/exceptions/) { get; } | 获取 CalendarExceptionCollection 对象。与该日历关联的异常集合。 |
| [Guid](../../aspose.tasks/calendar/guid/) { get; } | 获取日历的 Guid。 |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar/) { get; } | 获取一个值，指示该日历是否为基础日历。 |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar/) { get; set; } | 获取或设置一个值，指示该日历是否为基线日历。 |
| [Name](../../aspose.tasks/calendar/name/) { get; set; } | 获取或设置日历的名称。 |
| [PrimaveraProperties](../../aspose.tasks/calendar/primaveraproperties/) { get; } | 获取一个对象，包含从 Primavera 格式读取的日历的 Primavera 特定属性。 |
| [Uid](../../aspose.tasks/calendar/uid/) { get; set; } | 获取或设置日历的唯一标识符。 |
| [WeekDays](../../aspose.tasks/calendar/weekdays/) { get; } | 获取此日历的 WeekDaysCollection。定义该日历的工作日集合。 |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks/) { get; } | 获取 WorkWeekCollections 对象。与该日历关联的工作周集合。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar/)(Calendar) | 将给定的 Calendar 设置为 24 小时日历。24 小时日历是一种日历，其中一周的每一天都以全天候工作时间运行。 |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar/)(Calendar) | 将给定的日历设为夜班日历。 |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar/)(Calendar) | 创建默认的标准日历。 |
| [Delete](../../aspose.tasks/calendar/delete/)() | 从项目中移除日历。 |
| override [Equals](../../aspose.tasks/calendar/equals/)(object) | 返回一个值，指示此实例是否等于指定的对象。 |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | 根据日历计算指定工作时间量过去后的日期。 |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | 根据日历计算指定工作时间量过去后的日期。 |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode/)() | 返回类实例的哈希码。 |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart/)(DateTime) | 计算指定日期的下一个工作日开始时间。 |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend/)(DateTime) | 计算指定日期之前的工作日结束时间。 |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | 根据指定的结束日期和持续时间返回开始日期。 |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | 根据指定的结束日期和持续时间返回开始日期。 |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | 根据任务的开始日期、拆分部分和工作持续时间计算任务的完成日期和时间。 |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours_1)(DateTime) | 返回指定日期的工作小时数。 |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | 返回 WorkUnit —— 指定日期时间区间的工作时间的开始、结束和持续时间。 |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/calendar/getworkinghourstimespan/)(DateTime, DateTime) | 返回指定日期之间的工作小时数。 |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes/)(DateTime) | 返回指定日期的工作时间的 [`WorkingTimeCollection`](../workingtimecollection/)。 |
| [GetWorkStart](../../aspose.tasks/calendar/getworkstart/)(DateTime) | 计算从指定日期和时间开始的下一个工作时间的开始。 |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking/)(DateTime) | 确定指定日期是否为日历中的工作日。 |
| virtual [IsEmpty](../../aspose.tasks/calendar/isempty/)() | 返回日历是否未定义工作时间。 |
| static [GetIntersectionCalendar](../../aspose.tasks/calendar/getintersectioncalendar/)(Calendar, Calendar) | 获取 [`ICalendar`](../icalendar/) 实例，可用于对两个日历的工作时间表交集进行计算。 |

## 备注

日历用于定义标准工作时间和非工作时间。项目必须拥有一个基础日历。任务和资源可以拥有基于基础日历的非基础日历。

## 示例

如何从头创建简单日历。

```csharp
[C#]
// 创建空日历
Calendar calendar = new Calendar("New calendar");
// 添加默认工作日（每天 8 小时，上午 9:00 至下午 5:00）
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// 创建新的工作日
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// 设置工作时间。仅 DateTime 的时间部分重要。
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
' create empty calendar
Dim calendar As Calendar =  New Calendar("New calendar")
' adds default working days (8 working hours from 9:00 to 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' create new new working day
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' Sets working time. Only time part of DateTime is important
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
' adds weekend
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

展示如何定义新日历、向其添加工作日并为这些天定义工作时间。

```csharp
var project = new Project();

// 定义日历
var calendar = project.Calendars.Add("Calendar1");

// 添加从周一到周四的工作日，使用默认时间安排
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// 将周五设为短工作日
var weekDay = new WeekDay(DayType.Friday);

// 设置工作时间。仅 DateTime 的时间部分重要。
var workingTime = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 16);
weekDay.WorkingTimes.Add(workingTime);
weekDay.WorkingTimes.Add(workingTime2);
weekDay.DayWorking = true;
calendar.WeekDays.Add(weekDay);

// 正在处理项目……
```

### 另见

* interface [ICalendar](../icalendar/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


