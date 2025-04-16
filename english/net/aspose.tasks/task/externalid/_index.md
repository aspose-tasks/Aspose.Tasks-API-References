---
title: Task.ExternalId
second_title: Aspose.Tasks for .NET API Reference
description: Task property. Gets or sets a value of ExternalId
type: docs
weight: 410
url: /net/aspose.tasks/task/externalid/
---
## Task.ExternalId property

Gets or sets a value of ExternalId.

```csharp
public int ExternalId { get; set; }
```

## Examples

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

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


