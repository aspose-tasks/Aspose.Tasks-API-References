---
title: "Project.GetPredecessors"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 方法。返回指定任务的前置任务链接集合"
type: docs
weight: 1120
url: /zh/net/aspose.tasks/project/getpredecessors/
---
## Project.GetPredecessors method

返回指定任务的前置任务链接集合。

```csharp
public TaskLinkCollection GetPredecessors(Task task)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 任务 | 任务 | 要获取前置任务的任务。 |

### 返回值

前置任务的列表 [`TaskLink`](../../tasklink/)。

## 示例

展示如何获取特定任务的前置任务。

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");
var task = project.RootTask.Children.GetById(10);

var predecessors = project.GetPredecessors(task);

// 显示前置任务和后续任务的名称
foreach (var predecessor in predecessors)
{
    Console.WriteLine("Predecessor " + predecessor.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor " + predecessor.SuccTask.Get(Tsk.Name));
}
```

### 另见

* class [TaskLinkCollection](../../tasklinkcollection/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


