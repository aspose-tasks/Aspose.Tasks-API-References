---
title: "TaskLink.LinkLag"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TaskLink 属性。获取或设置以十分之一分钟或百分比表示的时滞"
type: docs
weight: 40
url: /zh/net/aspose.tasks/tasklink/linklag/
---
## TaskLink.LinkLag property

获取或设置以十分之一分钟或百分比表示的延迟。

```csharp
public int LinkLag { get; set; }
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

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


