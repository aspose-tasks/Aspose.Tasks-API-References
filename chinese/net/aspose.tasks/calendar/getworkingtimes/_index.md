---
title: "Calendar.GetWorkingTimes"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Calendar 方法。返回指定日期的 WorkingTimeCollection 工作时间"
type: docs
weight: 240
url: /zh/net/aspose.tasks/calendar/getworkingtimes/
---
## Calendar.GetWorkingTimes method

返回指定日期的 [`WorkingTimeCollection`](../../workingtimecollection/) 工作时间集合。

```csharp
public WorkingTimeCollection GetWorkingTimes(DateTime dt)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dt | DateTime | 获取工作时间的日期。 |

### 返回值

[`WorkingTime`](../../workingtime/) 实例的集合。

## 示例

展示如何获取特定日期的工作时间。

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// 获取特定日期的工作时间
var workingTimes = calendar.GetWorkingTimes(new DateTime(2020, 4, 8, 8, 0, 0));

// 将打印 16 小时
foreach (var workingTime in workingTimes)
{
    Console.WriteLine("From: " + workingTime.From);
    Console.WriteLine("To: " + workingTime.To);
}
```

### 另见

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


