---
title: "Tsk.BCWP"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. La valeur cumulative du pourcentage d’avancement des tâches multiplié par les coûts de référence phasés dans le temps"
type: docs
weight: 120
url: /fr/net/aspose.tasks/tsk/bcwp/
---
## Tsk.BCWP field

La valeur cumulative du pourcentage d'achèvement de la tâche multiplié par les coûts de base phasés dans le temps.

```csharp
public static readonly Key<double, TaskKey> BCWP;
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


