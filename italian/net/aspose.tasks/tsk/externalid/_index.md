---
title: "Tsk.ExternalId"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Se un'attività è esterna contiene l'ID esterno dell'attività"
type: docs
weight: 360
url: /it/net/aspose.tasks/tsk/externalid/
---
## Tsk.ExternalId field

Se un'attività è un'attività esterna contiene l'ID esterno dell'attività.

```csharp
public static readonly Key<int, TaskKey> ExternalId;
```

## Esempi

Mostra come identificare le attività cross‑project.

```csharp
var project = new Project(DataDir + "External.mpp");
var externalTask = project.RootTask.Children.GetByUid(1);

// Mostra l'ID dell'attività nel progetto esterno
Console.WriteLine(externalTask.Get(Tsk.Id).ToString());

// Mostra l'ID dell'attività nel progetto originale
Console.WriteLine(externalTask.Get(Tsk.ExternalId).ToString());
```

Mostra come creare un collegamento di attività cross‑project – collegamento a un'attività in un altro progetto (esterno).

```csharp
Project project = new Project();
var summary = project.RootTask.Children.Add("Summary Task");

// Per creare un collegamento a un'attività da un altro progetto dobbiamo creare
// il suo duplicato (o "esterno") nel progetto corrente.

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

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


