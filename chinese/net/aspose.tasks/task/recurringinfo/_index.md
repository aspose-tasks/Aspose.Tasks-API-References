---
title: "Task.RecurringInfo"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Task 属性。获取任务的 RecurringTaskInfo 类实例（如果任务是循环任务），如果任务不是循环任务则返回 null。RecurringTaskInfo 实例的信息仅在 mpp 文件格式中存在。"
type: docs
weight: 1030
url: /zh/net/aspose.tasks/task/recurringinfo/
---
## Task.RecurringInfo property

获取任务的 [`RecurringTaskInfo`](../../recurringtaskinfo/) 类实例（如果任务是循环任务）；如果任务不是循环任务则返回 null；[`RecurringTaskInfo`](../../recurringtaskinfo/) 实例的信息仅在 mpp 文件格式中存在。

```csharp
public RecurringTaskInfo RecurringInfo { get; }
```

## 示例

展示如何读取任务的循环信息。

```csharp
var project = new Project(DataDir + "TestRecurringTask2016.mpp");

var task = project.RootTask.Children.GetById(1);

Console.WriteLine("Recurrence Pattern: " + task.RecurringInfo.RecurrencePattern);
Console.WriteLine("Start Date: " + task.RecurringInfo.StartDate);
Console.WriteLine("End Date: " + task.RecurringInfo.EndDate);
Console.WriteLine("Duration: " + task.RecurringInfo.Duration);
Console.WriteLine("Occurrences: " + task.RecurringInfo.Occurrences);
Console.WriteLine("Weekly Days: " + task.RecurringInfo.WeeklyDays);
Console.WriteLine("WeeklyRepetitions: " + task.RecurringInfo.WeeklyRepetitions);
```

### 另见

* class [RecurringTaskInfo](../../recurringtaskinfo/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


