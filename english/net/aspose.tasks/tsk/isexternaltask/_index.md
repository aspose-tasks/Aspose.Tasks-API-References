---
title: Tsk.IsExternalTask
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Determines whether a task is external
type: docs
weight: 600
url: /net/aspose.tasks/tsk/isexternaltask/
---
## Tsk.IsExternalTask field

Determines whether a task is external.

```csharp
public static readonly Key<bool, TaskKey> IsExternalTask;
```

## Examples

Shows how to read/write Tsk.IsExternalTask property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsExternalTask, true);

Console.WriteLine("Is External Task: " + task.Get(Tsk.IsExternalTask));
```

Shows how to create cross project task link - link to task in another (external) project.

```csharp
Project project = new Project();
var summary = project.RootTask.Children.Add("Summary Task");

// In order to create a link to a task from another project we should create
// its duplicate (or "external") task in the current project.

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

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


