---
title: "Task.ExternalId"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Task. Obtient ou définit une valeur de ExternalId"
type: docs
weight: 410
url: /fr/net/aspose.tasks/task/externalid/
---
## Task.ExternalId property

Obtient ou définit une valeur de ExternalId.

```csharp
public int ExternalId { get; set; }
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


