---
title: "Tsk.Priority"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Le niveau d'importance attribué à une tâche, qui indique à quel point une tâche ou une affectation peut être retardée ou divisée lors du nivellement des ressources."
type: docs
weight: 930
url: /fr/net/aspose.tasks/tsk/priority/
---
## Tsk.Priority field

Le niveau d’importance attribué à une tâche, qui indique à son tour dans quelle mesure une tâche ou une affectation peut être retardée ou divisée lors du nivellement des ressources.

```csharp
public static readonly Key<int, TaskKey> Priority;
```

## Exemples

Montre comment lire la priorité d'une tâche.

```csharp
var project = new Project(DataDir + "TaskPriority.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Afficher les priorités pour toutes les tâches
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Priority : " + task.Get(Tsk.Priority));
}
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


