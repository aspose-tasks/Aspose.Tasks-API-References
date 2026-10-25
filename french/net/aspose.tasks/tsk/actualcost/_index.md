---
title: "Tsk.ActualCost"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Coûts engagés pour le travail déjà effectué par les ressources sur leurs tâches ainsi que tout autre coût enregistré associé à la tâche"
type: docs
weight: 20
url: /fr/net/aspose.tasks/tsk/actualcost/
---
## Tsk.ActualCost field

Coûts engagés pour le travail déjà effectué par les ressources sur leurs tâches, ainsi que tout autre coût enregistré associé à la tâche.

```csharp
public static readonly Key<decimal, TaskKey> ActualCost;
```

## Exemples

Montre comment lire les propriétés réelles de la tâche.

```csharp
var project = new Project(DataDir + "ActualTaskProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analyser toutes les tâches collectées
foreach (var task in collector.Tasks)
{
    Console.WriteLine("Task Name : " + task.Get(Tsk.Name));
    Console.WriteLine("Actual Start: " + task.Get(Tsk.ActualStart).ToLongDateString());
    Console.WriteLine("Actual Finish: " + task.Get(Tsk.ActualFinish).ToLongDateString());
    Console.WriteLine("Actual Duration: " + task.Get(Tsk.ActualDuration).TimeSpan.Hours);
    Console.WriteLine("Actual Cost: " + task.Get(Tsk.ActualCost));
}
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


