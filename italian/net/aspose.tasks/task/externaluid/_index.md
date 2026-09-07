---
title: "Task.ExternalUid"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Task. Ottiene o imposta l'identificatore univoco esterno del task quando il task è esterno"
type: docs
weight: 430
url: /it/net/aspose.tasks/task/externaluid/
---
## Task.ExternalUid property

Ottiene o imposta l'identificatore univoco del task esterno quando il task è esterno.

```csharp
public int ExternalUid { get; set; }
```

## Esempi

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

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


