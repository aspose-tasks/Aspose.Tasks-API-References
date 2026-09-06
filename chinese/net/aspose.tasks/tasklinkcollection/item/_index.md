---
title: "TaskLinkCollection.Item"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TaskLinkCollection 属性。返回或设置指定索引处的元素"
type: docs
weight: 20
url: /zh/net/aspose.tasks/tasklinkcollection/item/
---
## TaskLinkCollection indexer

返回或设置指定索引处的元素。

```csharp
public TaskLink this[int index] { get; set; }
```

| 参数 | 描述 |
| --- | --- |
| index | 要获取或设置的元素的零基索引。 |

### 返回值

指定索引处的元素。

## 示例

展示如何使用任务链接集合。

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// 获取任务
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// 链接任务
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// 打印任务之间的链接
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// 通过索引访问编辑链接
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// 移除所有任务链接
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### 另见

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


