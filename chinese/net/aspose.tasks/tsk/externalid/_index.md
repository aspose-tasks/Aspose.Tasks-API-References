---
title: "Tsk.ExternalId"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。如果任务是外部任务，则包含该任务的外部 ID"
type: docs
weight: 360
url: /zh/net/aspose.tasks/tsk/externalid/
---
## Tsk.ExternalId field

如果任务是外部任务，则包含该任务的外部 ID。

```csharp
public static readonly Key<int, TaskKey> ExternalId;
```

## 示例

展示如何识别跨项目任务。

```csharp
var project = new Project(DataDir + "External.mpp");
var externalTask = project.RootTask.Children.GetByUid(1);

// 显示外部项目中任务的 ID
Console.WriteLine(externalTask.Get(Tsk.Id).ToString());

// 显示原始项目中任务的 ID
Console.WriteLine(externalTask.Get(Tsk.ExternalId).ToString());
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

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


