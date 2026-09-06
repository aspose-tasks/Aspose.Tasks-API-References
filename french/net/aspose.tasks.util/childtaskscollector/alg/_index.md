---
title: "ChildTasksCollector.Alg"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ChildTasksCollector. Traite l'objet spécifié"
type: docs
weight: 30
url: /fr/net/aspose.tasks.util/childtaskscollector/alg/
---
## ChildTasksCollector.Alg method

Traite l'objet spécifié.

```csharp
public override void Alg(Task el, int level)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| el | Tâche | Objet à traiter. |
| niveau | Int32 | Niveau du nœud d'arbre. |

## Exemples

Montre comment itérer sur toutes les tâches d'un projet sous forme de liste simple.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analyser toutes les tâches collectées
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### Voir aussi

* class [Task](../../../aspose.tasks/task/)
* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


