---
title: "Tsk.OvertimeWork"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Le montant des heures supplémentaires prévues à être effectuées par toutes les ressources assignées à une tâche"
type: docs
weight: 870
url: /fr/net/aspose.tasks/tsk/overtimework/
---
## Tsk.OvertimeWork field

Le montant des heures supplémentaires prévu pour être effectué par toutes les ressources assignées à une tâche.

```csharp
public static readonly Key<Duration, TaskKey> OvertimeWork;
```

## Exemples

Montre comment lire les heures supplémentaires des tâches.

```csharp
var project = new Project(DataDir + "TaskOvertimes.mpp");

// Lire les heures supplémentaires et le pourcentage d'achèvement des tâches
foreach (var task in project.RootTask.Children)
{
    Console.WriteLine(task.Get(Tsk.OvertimeCost));
    Console.WriteLine(task.Get(Tsk.OvertimeWork));
    Console.WriteLine(task.Get(Tsk.PercentComplete));
    Console.WriteLine(task.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(task.Get(Tsk.PhysicalPercentComplete));

    // Définir le pourcentage d'achèvement
    task.Set(Tsk.PercentComplete, 100);
}
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


