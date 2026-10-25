---
title: "Tsk.OvertimeCost"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Le coût total des heures supplémentaires pour une tâche pour une ressource sur toutes les tâches assignées ou pour une affectation de ressource"
type: docs
weight: 860
url: /fr/net/aspose.tasks/tsk/overtimecost/
---
## Tsk.OvertimeCost field

Le coût total des heures supplémentaires pour une tâche, pour une ressource sur toutes les tâches assignées, ou pour une affectation de ressource.

```csharp
public static readonly Key<decimal, TaskKey> OvertimeCost;
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
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


