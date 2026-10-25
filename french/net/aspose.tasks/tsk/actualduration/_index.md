---
title: "Tsk.ActualDuration"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. L’intervalle du temps de travail réel d’une tâche basé sur la durée planifiée et le travail restant actuel ou le pourcentage d’avancement."
type: docs
weight: 30
url: /fr/net/aspose.tasks/tsk/actualduration/
---
## Tsk.ActualDuration field

La durée du temps de travail réel pour une tâche, basée sur la durée planifiée et le travail restant actuel ou le pourcentage d'achèvement.

```csharp
public static readonly Key<Duration, TaskKey> ActualDuration;
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
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


