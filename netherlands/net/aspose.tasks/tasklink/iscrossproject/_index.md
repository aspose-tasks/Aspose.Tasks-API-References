---
title: "TaskLink.IsCrossProject"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TaskLink-eigenschap. Haalt een waarde op of stelt een waarde in die aangeeft of een voorganger deel uitmaakt van een ander project"
type: docs
weight: 20
url: /nl/net/aspose.tasks/tasklink/iscrossproject/
---
## TaskLink.IsCrossProject property

Haalt een waarde op of stelt deze in die aangeeft of een voorganger deel uitmaakt van een ander project.

```csharp
public bool IsCrossProject { get; set; }
```

## Voorbeelden

Toont hoe cross-projecttaaklinks te vinden.

```csharp
var project = new Project(DataDir + "GetCrossProjectTaskLinks.mpp");

// Controleer cross-projecttaaklinks
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Task Link: " + taskLink.ToString());
    if (taskLink.IsCrossProject)
    {
        Console.WriteLine(taskLink.CrossProjectName);
    }
}
```

Toont hoe een cross-projecttaaklink te maken - link naar een taak in een ander (extern) project.

```csharp
Project project = new Project();
var summary = project.RootTask.Children.Add("Summary Task");

// Om een link naar een taak uit een ander project te maken, moeten we
// de duplicaat (of "externe") taak in het huidige project.

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

### Zie ook

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


