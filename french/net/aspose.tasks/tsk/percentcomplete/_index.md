---
title: "Tsk.PercentComplete"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. L'état actuel d'une tâche exprimé en pourcentage de la durée de la tâche qui a été complétée"
type: docs
weight: 880
url: /fr/net/aspose.tasks/tsk/percentcomplete/
---
## Tsk.PercentComplete field

L’état actuel d’une tâche, exprimé en pourcentage de la durée de la tâche qui a été accomplie.

```csharp
public static readonly Key<int, TaskKey> PercentComplete;
```

## Exemples

Montre comment modifier la progression d'une tâche en mettant à jour le pourcentage d'achèvement de la tâche.

```csharp
var project = new Project();
Console.WriteLine("Project Calculation mode is Automatic: {0}", project.CalculationMode.Equals(CalculationMode.Automatic));

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(2));
task.Set(Tsk.PercentComplete, 50);

// Accéder aux tâches et afficher le pourcentage d'achèvement
foreach (var tsk in project.RootTask.Children)
{
    Console.WriteLine(tsk.Get(Tsk.PercentComplete));
    Console.WriteLine(tsk.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(tsk.Get(Tsk.PhysicalPercentComplete));
}
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


