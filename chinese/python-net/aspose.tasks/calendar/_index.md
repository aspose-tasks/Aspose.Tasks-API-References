---
title: "Calendar"
second_title: "适用于 Python via .NET 的 Aspose.Tasks API 参考"
description: 
type: docs
weight: 140
url: /zh/python-net/aspose.tasks/calendar/
---

## Calendar class

表示项目中使用的日历。

Calendar 类型公开以下成员：
## 属性
| 名称 | 描述 |
| :- | :- |
| name | 获取或设置日历的名称。 |
| uid | 获取或设置日历的唯一标识符。 |
| week_days | 获取此日历的 WeekDaysCollection。<br/>            定义日历的工作日集合。 |
| exceptions | 获取 CalendarExceptionCollection 对象。<br/>            与日历关联的例外集合。 |
| work_weeks | 获取 WorkWeekCollections 对象。<br/>            与日历关联的工作周集合。 |
| is_base_calendar | 获取一个值，指示该日历是否为基础日历。 |
| base_calendar | 获取或设置此日历所依赖的基础日历。<br/>            仅在该日历不是基础日历时适用。 |
| is_baseline_calendar | 获取或设置一个值，指示该日历是否为基线日历。 |
| guid | 获取日历的 Guid。 |
| Primavera 属性 | 获取一个对象，其中包含从 Primavera 格式读取的日历的 Primavera 特定属性。 |
## Methods
| 名称 | 描述 |
| :- | :- |
| get_start_date_from_finish_and_duration(finish, duration) | 根据指定的结束日期和持续时间返回开始日期。 |
| get_start_date_from_finish_and_duration(finish, duration) | 根据指定的结束日期和持续时间返回开始日期。 |
| get_working_hours(start, finish) | 返回 WorkUnit - 指定日期时间间隔的工作时间的开始、结束和持续时间。 |
| get_working_hours(dt) | 返回 WorkUnit - 指定日期时间间隔的工作时间的开始、结束和持续时间。 |
| get_finish_date_by_start_and_work(start, work) | 根据日历计算指定工作时间量过去后的日期。 |
| get_finish_date_by_start_and_work(start, work) | 根据日历计算指定工作时间量过去后的日期。 |
| get_intersection_calendar(calendar1, calendar2) | 获取 [ICalendar](/tasks/python-net/aspose.tasks/icalendar/) 实例，可用于对两个日历的工作计划交集进行计算。 |
| make_standard_calendar(calendar) | 创建默认的标准日历。 |
| make_24_hour_calendar(calendar) | 将给定的日历设为 24 小时日历。<br/>            24 小时日历是指每周的每一天都以全天候工作时间运行的日历。 |
| make_night_shift_calendar(calendar) | 将给定的日历设为夜班日历。 |
| delete() | 从项目中移除日历。 |
| is_day_working(dt) | 确定指定日期是否为工作日（根据日历）。 |
| get_working_hours_time_span(start, finish) | 返回指定日期之间的工作小时数。 |
| get_task_finish_date_from_duration(task, duration) | 根据任务的开始日期、拆分部分和工作时长计算任务的完成日期和时间。 |
| get_working_times(dt) | 返回指定日期的工作时间集合 [WorkingTimeCollection](/tasks/python-net/aspose.tasks/workingtimecollection/)。 |
| get_previous_working_day_end(date) | 根据指定日期计算前一个工作日的结束时间。 |
| get_next_working_day_start(date) | 计算指定日期的下一个工作日的开始时间。 |
| get_work_start(date) | 从指定的日期和时间开始计算下一个工作时间的开始。 |
| is_empty() | 返回日历是否未定义工作时间。 |

### 另见

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

