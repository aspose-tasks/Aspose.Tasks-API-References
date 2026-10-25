---
title: "Aspose::Tasks::Calendar 类"
linktitle: "日历"
articleTitle: "日历"
second_title: "Aspose.Tasks for C++"
description: "表示项目中使用的日历。"
type: docs
weight: 10
url: /zh/cpp/aspose.tasks/calendar/
---

## Calendar class

**Inherits:** Aspose::Tasks::ICalendar

表示项目中使用的日历。

如何从头创建简单日历。

```cpp
[C#]
// 创建空日历
Calendar calendar = new Calendar("New calendar");
// 添加默认工作日（每天 8 小时，从 9:00 到 17:00）
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

```cpp
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

日历用于定义标准工作时间和非工作时间。项目必须拥有一个基础日历。任务和资源可以拥有基于基础日历的非基础日历。

## 方法

| 表示 ResourceAssignment 对象的属性。 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| [Delete](./delete/) | 从项目中移除日历。 |
| [Equals](./equals/) | 返回一个值，指示此实例是否等于指定的对象。 |
| [get_BaseCalendar](./get_basecalendar/) | 获取此日历所依赖的基础日历。仅在该日历不是基础日历时适用。 |
| [get_Exceptions](./get_exceptions/) | 获取 CalendarExceptionCollection 对象。与日历关联的例外集合。 |
| [get_Guid](./get_guid/) | 获取日历的 Guid。 |
| [get_IsBaseCalendar](./get_isbasecalendar/) | 获取指示日历是否为基础日历的值。 |
| [get_IsBaselineCalendar](./get_isbaselinecalendar/) | 获取指示日历是否为基线日历的值。 |
| [get_Name](./get_name/) | 获取日历的名称。 |
| [get_Uid](./get_uid/) | 获取日历的唯一标识符。 |
| [get_WeekDays](./get_weekdays/) | 获取此日历的 WeekDaysCollection。定义日历的工作日集合。 |
| [get_WorkWeeks](./get_workweeks/) | 获取 WorkWeekCollections 对象。与日历关联的工作周集合。 |
| [GetFinishDateByStartAndWork (2 overloads)](./getfinishdatebystartandwork/) | 根据日历计算指定工作时间量结束的日期。 |
| [GetHashCode](./gethashcode/) | 返回类实例的哈希码。 |
| [GetIntersectionCalendar](./getintersectioncalendar/) | 获取 ICalendar 实例，可用于计算两个日历工作时间表交集的计算。 |
| [GetNextWorkingDayStart](./getnextworkingdaystart/) | 计算指定日期的下一个工作日开始时间。 |
| [GetPreviousWorkingDayEnd](./getpreviousworkingdayend/) | 根据指定日期计算前一个工作日的结束时间。 |
| [GetStartDateFromFinishAndDuration (2 overloads)](./getstartdatefromfinishandduration/) | 根据指定的结束日期和持续时间返回开始日期。 |
| [GetTaskFinishDateFromDuration](./gettaskfinishdatefromduration/) | 根据任务的开始日期、拆分部分和工作持续时间计算任务的完成日期和时间。 |
| [GetWorkingHours (2 overloads)](./getworkinghours/) | 返回指定日期的工作小时数。 |
| [GetWorkingHoursTimeSpan](./getworkinghourstimespan/) | 返回指定日期之间的工作小时数。 |
| [GetWorkingTimes](./getworkingtimes/) | 返回指定日期的 WorkingTimeCollection 工作时间集合。 |
| [GetWorkStart](./getworkstart/) | 从指定的日期和时间开始计算下一个工作时间的开始。 |
| [IsDayWorking](./isdayworking/) | 确定指定的日期是否为日历中的工作日。 |
| [IsEmpty](./isempty/) | 返回日历是否未定义工作时间。 |
| [Make24HourCalendar](./make24hourcalendar/) | 将给定的日历设为 24 小时日历。24 小时日历是指每周的每一天都以全天候工作时间运行的日历。 |
| [MakeNightShiftCalendar](./makenightshiftcalendar/) | 将给定的日历设为夜班日历。 |
| [MakeStandardCalendar](./makestandardcalendar/) | 创建默认标准日历。 |
| [set_BaseCalendar](./set_basecalendar/) | 设置此日历所依赖的基础日历。仅在该日历不是基础日历时适用。 |
| [set_IsBaselineCalendar](./set_isbaselinecalendar/) | 设置指示日历是否为基线日历的值。 |
| [set_Name](./set_name/) | 设置日历的名称。 |
| [set_Uid](./set_uid/) | 设置日历的唯一标识符。 |

