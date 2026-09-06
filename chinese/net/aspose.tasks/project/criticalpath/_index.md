---
title: "Project.CriticalPath"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 属性。获取一个集合，其中包含构成此项目关键路径的关键任务列表。这是一个 O(n) 操作，其中 n 是项目中的任务数量"
type: docs
weight: 180
url: /zh/net/aspose.tasks/project/criticalpath/
---
## Project.CriticalPath property

获取一个集合，其中包含构成此项目关键路径的关键任务列表。这是 O(n) 操作，其中 n 为项目中的任务数量。

```csharp
public TaskCollection CriticalPath { get; }
```

### 返回值

一个表示所有关键任务列表的集合。

## 示例

展示如何计算项目的关键路径。

```csharp
var project = new Project()
{
    CalculationMode = CalculationMode.Automatic
};

var subtask1 = project.RootTask.Children.Add("1");
var subtask2 = project.RootTask.Children.Add("2");
project.TaskLinks.Add(subtask1, subtask2, TaskLinkType.FinishToStart);

project.RootTask.Children.Add("3");

// 立即显示关键路径
foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id) + "  " + task.Get(Tsk.Name));
    Console.WriteLine(task.Get(Tsk.Start));
    Console.WriteLine(task.Get(Tsk.Finish) + "\n");
}
```

### 另见

* class [TaskCollection](../../taskcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


