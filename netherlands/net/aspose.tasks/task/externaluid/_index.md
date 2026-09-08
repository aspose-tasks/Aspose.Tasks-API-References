---
title: "Task.ExternalUid"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Task eigenschap. Haalt of stelt de unieke identifier van externe taken in wanneer de taak extern is"
type: docs
weight: 430
url: /nl/net/aspose.tasks/task/externaluid/
---
## Task.ExternalUid property

Haalt op of stelt de unieke identifier van de externe taak in wanneer de taak extern is.

```csharp
public int ExternalUid { get; set; }
```

## Voorbeelden

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

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


