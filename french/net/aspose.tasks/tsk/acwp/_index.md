---
title: "Tsk.ACWP"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Coûts engagés pour le travail déjà effectué sur une tâche jusqu'à la date d'état du projet ou à la date d'aujourd'hui."
type: docs
weight: 110
url: /fr/net/aspose.tasks/tsk/acwp/
---
## Tsk.ACWP field

Coûts engagés pour le travail déjà effectué sur une tâche, jusqu'à la date d'état du projet ou à la date d'aujourd'hui.

```csharp
public static readonly Key<double, TaskKey> ACWP;
```

## Exemples

Montre comment lire les valeurs de coût des tâches.

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

foreach (var task in collector.Tasks)
{
    Console.WriteLine("Cost: " + task.Get(Tsk.Cost));
    Console.WriteLine("ACWP: " + task.Get(Tsk.ACWP));
    Console.WriteLine("BCWP: " + task.Get(Tsk.BCWP));
    Console.WriteLine("BCWS: " + task.Get(Tsk.BCWS));

    // CV = BCWP - ACWP
    Console.WriteLine("CV: " + task.Get(Tsk.CV));
    Console.WriteLine();
}
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


