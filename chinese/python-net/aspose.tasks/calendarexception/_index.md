---
title: "CalendarException"
second_title: "适用于 Python via .NET 的 Aspose.Tasks API 参考"
description: 
type: docs
weight: 160
url: /zh/python-net/aspose.tasks/calendarexception/
---

## CalendarException class

表示日历中的例外时间段。

CalendarException 类型公开以下成员：
## 构造函数
| 名称 | 描述 |
| :- | :- |
| CalendarException() | 初始化一个新的 [CalendarException](/tasks/python-net/aspose.tasks/calendarexception/) 类实例。 |
## 属性
| 名称 | 描述 |
| :- | :- |
| entered_by_occurrences | 获取或设置一个值，指示是否通过输入出现次数来定义重复范围。<br/>            False 指定重复范围是通过输入结束日期来定义的。 |
| from_date | 获取或设置异常时间的开始。 |
| to_date | 获取或设置异常时间的结束。 |
| occurrences | 获取或设置日历异常有效的出现次数。 |
| name | 获取或设置异常的名称。 |
| type | 获取或设置异常类型。 |
| period | 获取或设置异常的重复周期。 |
| days_of_week | 获取此对象的 DayTypeCollection。<br/>            异常有效的星期几。 |
| month_item | 获取或设置安排异常重复的月份项。 |
| month_position | 获取或设置月份项在月份中的位置。 |
| month | 获取或设置安排异常重复的月份。 |
| month_day | 获取或设置安排异常重复的月份中的天。 |
| day_working | 获取或设置一个值，指示指定的日期或日期类型是否为工作日。 |
| working_times | 获取或设置 WorkingTimeCollection 对象。<br/>            定义工作日工作时间的工作时间集合。 |
| parent_calendar | 获取此对象的父日历。 |
## Methods
| 名称 | 描述 |
| :- | :- |
| delete() | 从父日历 CalendarExceptionCollection 对象中删除 Exception 实例。 |
| check_exception(dt) | 如果指定的 datetime 结构实例是异常日，则返回 true。 |
| get_working_time() | 返回日历例外的工作时间。 |
| get_exception_dates() | 返回日历例外适用的日期。 |

### 另见

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

