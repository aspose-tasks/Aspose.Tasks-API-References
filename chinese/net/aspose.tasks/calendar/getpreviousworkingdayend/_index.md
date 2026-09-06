---
title: "Calendar.GetPreviousWorkingDayEnd"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Calendar 方法。计算指定日期之前的工作日结束时间。"
type: docs
weight: 190
url: /zh/net/aspose.tasks/calendar/getpreviousworkingdayend/
---
## Calendar.GetPreviousWorkingDayEnd method

计算指定日期之前的工作日结束时间。

```csharp
public DateTime GetPreviousWorkingDayEnd(DateTime date)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 日期 | DateTime | 用于计算前一个工作日结束时间的日期。 |

### 返回值

前一个工作日的结束时间。

## 示例

展示如何使用 Calendar 获取前一个工作日结束时间。

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// 获取前一个工作日结束时间
var previousWorkingDayEnd = calendar.GetPreviousWorkingDayEnd(new DateTime(2020, 4, 10, 13, 0, 0));

// 2020年4月9日 18:00 将被打印。
Console.WriteLine(previousWorkingDayEnd);
```

### 另见

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


