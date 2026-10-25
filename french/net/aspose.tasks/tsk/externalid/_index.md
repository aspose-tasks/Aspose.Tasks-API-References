---
title: "Tsk.ExternalId"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Si une tâche est une tâche externe, elle contient l'Id externe de la tâche"
type: docs
weight: 360
url: /fr/net/aspose.tasks/tsk/externalid/
---
## Tsk.ExternalId field

Si une tâche est une tâche externe, elle contient l'ID externe de la tâche.

```csharp
public static readonly Key<int, TaskKey> ExternalId;
```

## Exemples

Montre comment identifier les tâches inter‑projets.

```csharp
var project = new Project(DataDir + "External.mpp");
var externalTask = project.RootTask.Children.GetByUid(1);

// Afficher l'ID de la tâche dans le projet externe
Console.WriteLine(externalTask.Get(Tsk.Id).ToString());

// Afficher l'ID de la tâche dans le projet original
Console.WriteLine(externalTask.Get(Tsk.ExternalId).ToString());
```

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

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


