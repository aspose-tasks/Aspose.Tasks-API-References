---
title: "类 TaskLink"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.TaskLink 类。表示前置链接"
type: docs
weight: 2410
url: /zh/net/aspose.tasks/tasklink/
---
## TaskLink class

表示前置链接。

```csharp
public sealed class TaskLink : IEquatable<TaskLink>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [CrossProjectName](../../aspose.tasks/tasklink/crossprojectname/) { get; set; } | 获取或设置外部前置项目。 |
| [IsCrossProject](../../aspose.tasks/tasklink/iscrossproject/) { get; set; } | 获取或设置一个值，指示前置任务是否属于另一个项目。 |
| [LagFormat](../../aspose.tasks/tasklink/lagformat/) { get; set; } | 获取或设置用于表示延迟格式的格式。 |
| [LinkLag](../../aspose.tasks/tasklink/linklag/) { get; set; } | 获取或设置以十分之一分钟或百分比表示的延迟。 |
| [LinkLagTimeSpan](../../aspose.tasks/tasklink/linklagtimespan/) { get; set; } | 获取或设置延迟持续时间，取决于 LagFormat。 |
| [LinkType](../../aspose.tasks/tasklink/linktype/) { get; set; } | 获取或设置链接的类型。 |
| [PredTask](../../aspose.tasks/tasklink/predtask/) { get; set; } | 获取或设置前置任务。 |
| [SuccTask](../../aspose.tasks/tasklink/succtask/) { get; set; } | 获取或设置后续任务。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [Equals](../../aspose.tasks/tasklink/equals/#equals_1)(object) | 返回一个值，指示此实例是否等于指定的对象。 |
| [Equals](../../aspose.tasks/tasklink/equals/#equals)(TaskLink) | 返回一个值，指示此实例是否等于指定的对象。 |
| override [GetHashCode](../../aspose.tasks/tasklink/gethashcode/)() | 返回 `TaskLink` 类实例的哈希码值。 |
| override [ToString](../../aspose.tasks/tasklink/tostring/)() | 返回 TaskLink 的字符串表示。表示的具体细节未指定，且可能会更改。 |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


