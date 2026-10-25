---
title: "Calendar.GetWorkingHours"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Calendar 方法。返回指定日期时间间隔的工作单元、开始、结束和工作时长。"
type: docs
weight: 220
url: /zh/net/aspose.tasks/calendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

返回 WorkUnit —— 指定日期时间区间的工作时间的开始、结束和持续时间。

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 开始 | DateTime | 区间的开始日期。 |
| 结束 | DateTime | 区间的结束日期。 |

### 返回值

[`WorkUnit`](../../workunit/) 类的实例，包含工作时间的开始、结束和持续时间。

## 示例

展示如何获取特定日期的工作时间。

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// 获取特定日期的工作时间
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

// 将打印 16 小时
Console.WriteLine(workUnit.WorkingHours);
```

### 另见

* class [WorkUnit](../../workunit/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

返回指定日期的工作小时数。

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dt | DateTime | 获取工作时间的日期。 |

### 返回值

指定日期的工作时间。

## 示例

展示如何获取特定日期的工作时间。

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// 获取特定日期的工作时间
var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 10));

// 将打印 8 小时
Console.WriteLine(workingHours.Hours);
```

### 另见

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


