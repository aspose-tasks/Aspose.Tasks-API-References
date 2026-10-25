---
title: "TaskLink.LagFormat"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TaskLink 属性。获取或设置用于表示时滞的格式"
type: docs
weight: 30
url: /zh/net/aspose.tasks/tasklink/lagformat/
---
## TaskLink.LagFormat property

获取或设置用于表示延迟格式的格式。

```csharp
public TimeUnitType LagFormat { get; set; }
```

## 示例

展示如何读取项目任务链接。

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

// 显示前置任务和后续任务的名称
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Predecessor: " + taskLink.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor: " + taskLink.SuccTask.Get(Tsk.Name));
    Console.WriteLine("Lag Format: " + taskLink.LagFormat);
    Console.WriteLine("Link Lag: " + taskLink.LinkLag);
    Console.WriteLine();
}
```

### 另见

* enum [TimeUnitType](../../timeunittype/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


