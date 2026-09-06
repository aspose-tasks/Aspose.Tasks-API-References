---
title: "Task.Status"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Task 属性。获取任务状态"
type: docs
weight: 1160
url: /zh/net/aspose.tasks/task/status/
---
## Task.Status property

获取任务状态。

```csharp
public TaskStatus Status { get; }
```

## 示例

展示如何获取任务的状态。

```csharp
var project = new Project(DataDir + "TaskPercentageCompletion.mpp");

// 应设置项目的状态日期，因为状态计算使用状态日期。
project.StatusDate = new DateTime(2010, 7, 9, 15, 0, 0);
foreach (var task in project.EnumerateAllChildTasks())
{
    Console.WriteLine("{0} - {1}", task.Name, task.Status);
}
```

### 另见

* enum [TaskStatus](../../taskstatus/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


