---
title: "Tsk.ExternalId"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. Als een taak een externe taak is, bevat deze de externe Id van de taak"
type: docs
weight: 360
url: /nl/net/aspose.tasks/tsk/externalid/
---
## Tsk.ExternalId field

Als een taak een externe taak is, bevat deze de externe ID van de taak.

```csharp
public static readonly Key<int, TaskKey> ExternalId;
```

## Voorbeelden

Toont hoe cross-projecttaken te identificeren.

```csharp
var project = new Project(DataDir + "External.mpp");
var externalTask = project.RootTask.Children.GetByUid(1);

// Toon ID van de taak in het externe project
Console.WriteLine(externalTask.Get(Tsk.Id).ToString());

// Toon ID van de taak in het oorspronkelijke project
Console.WriteLine(externalTask.Get(Tsk.ExternalId).ToString());
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

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


