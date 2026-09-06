---
title: "Calendar.GetNextWorkingDayStart"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Calendar 方法。计算指定日期的下一个工作日开始时间"
type: docs
weight: 180
url: /zh/net/aspose.tasks/calendar/getnextworkingdaystart/
---
## Calendar.GetNextWorkingDayStart method

计算指定日期的下一个工作日开始时间。

```csharp
public DateTime GetNextWorkingDayStart(DateTime date)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 日期 | DateTime | 用于获取下一个工作日开始时间的日期。 |

### 返回值

下一个工作日开始的 DateTime。

## 示例

展示如何使用日历获取下一个工作日的开始时间。

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// 获取下一个工作日的开始时间（跳过周末）
var nextWorkingDayStart = calendar.GetNextWorkingDayStart(new DateTime(2020, 4, 10, 13, 0, 0));

// 2020年4月13日 上午9:00 将被打印
Console.WriteLine(nextWorkingDayStart);
```

### 另见

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


