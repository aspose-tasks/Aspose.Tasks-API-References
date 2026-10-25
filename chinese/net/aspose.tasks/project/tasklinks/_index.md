---
title: "Project.TaskLinks"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 属性。获取 TaskLinkCollection 对象。"
type: docs
weight: 930
url: /zh/net/aspose.tasks/project/tasklinks/
---
## Project.TaskLinks property

获取 [`TaskLinkCollection`](../../tasklinkcollection/) 对象。

```csharp
public TaskLinkCollection TaskLinks { get; }
```

## 示例

展示如何创建任务链接。

```csharp
var project = new Project();

// 添加新任务
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// 链接任务
project.TaskLinks.Add(pred, succ);

foreach (var link in project.TaskLinks)
{
    Console.WriteLine("Predecessor Task: " + link.PredTask);
    Console.WriteLine("Successor Task: " + link.SuccTask);
    Console.WriteLine("LagFormat: " + link.LagFormat);
    Console.WriteLine("LinkType: " + link.LinkType);
    Console.WriteLine("LinkLag: " + link.LinkLag);
    Console.WriteLine("CrossProjectName: " + link.CrossProjectName);
    Console.WriteLine("IsCrossProject: " + link.IsCrossProject);
}
```

### 另见

* class [TaskLinkCollection](../../tasklinkcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


