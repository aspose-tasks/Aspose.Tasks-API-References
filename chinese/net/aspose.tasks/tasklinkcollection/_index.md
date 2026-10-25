---
title: "类 TaskLinkCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.TaskLinkCollection 类。表示 Task 对象的集合"
type: docs
weight: 2420
url: /zh/net/aspose.tasks/tasklinkcollection/
---
## TaskLinkCollection class

表示一个 [`Task`](../task/) 对象的集合。

```csharp
public class TaskLinkCollection : IList<TaskLink>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/tasklinkcollection/count/) { get; } | 获取此 `TaskLinkCollection` 对象中包含的对象数量。 |
| [Item](../../aspose.tasks/tasklinkcollection/item/) { get; set; } | 返回或设置指定索引处的元素。 |
| [ParentProject](../../aspose.tasks/tasklinkcollection/parentproject/) { get; } | 获取 ResourceAssignmentCollection 对象的父项目。此对象的父 [`Project`](../project/)。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_3)(TaskLink) | 这是 ICollection 的 Add 方法的存根实现，只会抛出 NotSupportedException。 |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add)(Task, Task) | 返回已添加到 TaskLinkCollection 对象的 Finish-Start [`TaskLink`](../tasklink/) 实例。 |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_1)(Task, Task, TaskLinkType) | 返回已添加到 TaskLinkCollection 对象的 [`TaskLink`](../tasklink/) 实例。 |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_2)(Task, Task, TaskLinkType, Duration) | 返回已添加到 TaskLinkCollection 对象的 [`TaskLink`](../tasklink/) 实例。 |
| [GetEnumerator](../../aspose.tasks/tasklinkcollection/getenumerator/)() | 返回此集合的枚举器。 |
| [Remove](../../aspose.tasks/tasklinkcollection/remove/)(TaskLink) | 从项目中移除任务链接。 |
| [ToList](../../aspose.tasks/tasklinkcollection/tolist/)() | 将 TaskLinkCollection 对象转换为 [`TaskLink`](../tasklink/) 对象的列表。 |

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

* class [TaskLink](../tasklink/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


