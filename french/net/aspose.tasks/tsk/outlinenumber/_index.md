---
title: "Tsk.OutlineNumber"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Le nombre qui représente la position d’une tâche dans la structure hiérarchique du plan"
type: docs
weight: 850
url: /fr/net/aspose.tasks/tsk/outlinenumber/
---
## Tsk.OutlineNumber field

Le numéro qui représente la position d’une tâche dans la structure hiérarchique du contour.

```csharp
public static readonly Key<string, TaskKey> OutlineNumber;
```

## Exemples

Montre comment lire les propriétés de contour de tâche.

```csharp
var project = new Project(DataDir + "TaskOutlineProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analyser toutes les tâches collectées
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Level : " + task.Get(Tsk.OutlineLevel));
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Number : " + task.Get(Tsk.OutlineNumber));
}
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


