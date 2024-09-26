---
title: TaskLink.IsCrossProject
second_title: Aspose.Tasks for .NET API Reference
description: TaskLink property. Gets or sets a value indicating whether a predecessor is part of another project
type: docs
weight: 20
url: /net/aspose.tasks/tasklink/iscrossproject/
---
## TaskLink.IsCrossProject property

Gets or sets a value indicating whether a predecessor is part of another project.

```csharp
public bool IsCrossProject { get; set; }
```

## Examples

Shows how to find cross project task links.

```csharp
var project = new Project(DataDir + "GetCrossProjectTaskLinks.mpp");

// Check cross project task links
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Task Link: " + taskLink.ToString());
    if (taskLink.IsCrossProject)
    {
        Console.WriteLine(taskLink.CrossProjectName);
    }
}
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

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


