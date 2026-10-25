---
title: "TaskLink.PredTask"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TaskLink 属性。获取或设置前置任务"
type: docs
weight: 70
url: /zh/net/aspose.tasks/tasklink/predtask/
---
## TaskLink.PredTask property

获取或设置前置任务。

```csharp
public Task PredTask { get; set; }
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

* class [Task](../../task/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


