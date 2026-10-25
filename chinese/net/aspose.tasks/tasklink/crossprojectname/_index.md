---
title: "TaskLink.CrossProjectName"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TaskLink 属性。获取或设置外部前置项目"
type: docs
weight: 10
url: /zh/net/aspose.tasks/tasklink/crossprojectname/
---
## TaskLink.CrossProjectName property

获取或设置外部前置项目。

```csharp
public string CrossProjectName { get; set; }
```

## 示例

展示如何查找跨项目任务链接。

```csharp
var project = new Project(DataDir + "GetCrossProjectTaskLinks.mpp");

// 检查跨项目任务链接
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Task Link: " + taskLink.ToString());
    if (taskLink.IsCrossProject)
    {
        Console.WriteLine(taskLink.CrossProjectName);
    }
}
```

展示如何创建跨项目任务链接——链接到另一个（外部）项目中的任务。

```csharp
Project project = new Project();
var summary = project.RootTask.Children.Add("Summary Task");

// 为了创建指向另一个项目中任务的链接，我们应当创建
// 该任务的副本（或“外部”）任务于当前项目中。

Task t2 = summary.Children.Add("External Task");
t2.Set(Tsk.ExternalTaskProject, "ExternalProject.mpp"); // here we set path to external project's MPP file.
t2.Set(Tsk.ExternalId, 1); // Set External task's Id.
t2.Set(Tsk.ExternalUid, 2); // External task's Unique Id should be set.
t2.Set(Tsk.IsExternalTask, true);
t2.Set(Tsk.IsManual, new NullableBool(false));
t2.Set(Tsk.IsSummary, false);

Task t = summary.Children.Add("Task");
TaskLink link = project.TaskLinks.Add(t2, t);
link.IsCrossProject = true;
link.LinkType = TaskLinkType.FinishToStart;
link.CrossProjectName = "ExternalProject.mpp\\\\1"; // <- here external task's Id is used.
```

### 另见

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


