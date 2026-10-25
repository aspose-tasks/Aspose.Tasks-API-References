---
title: "Tsk.CV"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. La différence entre le coût de référence et le coût total d'une tâche. Cost Variance  Cost  Baseline Cost"
type: docs
weight: 260
url: /fr/net/aspose.tasks/tsk/cv/
---
## Tsk.CV field

La différence entre le coût de référence et le coût total pour une tâche. Écart de coût = Coût - Coût de référence

```csharp
public static readonly Key<double, TaskKey> CV;
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


