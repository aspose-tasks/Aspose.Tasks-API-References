---
title: "TaskLinkCollection.ToList"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TaskLinkCollection 方法。将 TaskLinkCollection 对象转换为 TaskLink 对象的列表"
type: docs
weight: 70
url: /zh/net/aspose.tasks/tasklinkcollection/tolist/
---
## TaskLinkCollection.ToList method

将 TaskLinkCollection 对象转换为 [`TaskLink`](../../tasklink/) 对象的列表。

```csharp
public List<TaskLink> ToList()
```

### 返回值

[`TaskLink`](../../tasklink/) 对象的列表。

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


