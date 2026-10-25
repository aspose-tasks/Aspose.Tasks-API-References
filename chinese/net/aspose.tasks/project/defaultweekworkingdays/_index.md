---
title: "Project.DefaultWeekWorkingDays"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 属性。获取 WeekDayCollection 类的实例，该实例表示项目默认工作周的工作日和工作时间的集合"
type: docs
weight: 370
url: /zh/net/aspose.tasks/project/defaultweekworkingdays/
---
## Project.DefaultWeekWorkingDays property

获取 [`WeekDayCollection`](../../weekdaycollection/) 类的实例，该实例表示项目默认工作周的工作日和工作时间的集合。

```csharp
public WeekDayCollection DefaultWeekWorkingDays { get; }
```

### 返回值

[`WeekDayCollection`](../../weekdaycollection/) 类的实例，其中包含一系列 [`WeekDay`](../../weekday/) 对象。

## 备注

该数据仅存在于 mpp 文件中（不在 xml 中）。

## 示例

展示如何获取默认工作周的工作日。

```csharp
var project = new Project(DataDir + "Project2003.mpp");
foreach (var weekDay in project.DefaultWeekWorkingDays)
{
    Console.WriteLine("From: " + weekDay.FromDate);
    Console.WriteLine("From: " + weekDay.ToDate);
    Console.WriteLine("Day type: " + weekDay.DayType);
    Console.WriteLine("Is day working: " + weekDay.DayWorking);
}
```

### 另见

* class [WeekDayCollection](../../weekdaycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


