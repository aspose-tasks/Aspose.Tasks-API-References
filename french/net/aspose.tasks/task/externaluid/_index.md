---
title: "Task.ExternalUid"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Task. Obtient ou définit l'identifiant unique des tâches externes lorsque la tâche est externe"
type: docs
weight: 430
url: /fr/net/aspose.tasks/task/externaluid/
---
## Task.ExternalUid property

Obtient ou définit l'identifiant unique de la tâche externe lorsque la tâche est externe.

```csharp
public int ExternalUid { get; set; }
```

## Exemples

Montre comment créer un lien de tâche inter‑projet – lien vers une tâche dans un autre projet (externe).

```csharp
Project project = new Project();
var summary = project.RootTask.Children.Add("Summary Task");

// Afin de créer un lien vers une tâche d'un autre projet, nous devons créer
// son double (ou "external") tâche dans le projet actuel.

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

### Voir aussi

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


