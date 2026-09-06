---
title: "Tsk.FixedCost"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Affiche toute dépense de tâche non liée aux ressources"
type: docs
weight: 430
url: /fr/net/aspose.tasks/tsk/fixedcost/
---
## Tsk.FixedCost field

Affiche toute dépense de tâche non liée à une ressource.

```csharp
public static readonly Key<double, TaskKey> FixedCost;
```

## Exemples

Montre comment lire les coûts des tâches.

```csharp
var project = new Project();

// Ajouter une tâche et définir le coût
var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Cost, 800);

// Afficher les propriétés liées au coût de la tâche
Console.WriteLine(task.Get(Tsk.RemainingCost));
Console.WriteLine(task.Get(Tsk.FixedCost));
Console.WriteLine(task.Get(Tsk.CostVariance));
Console.WriteLine(project.RootTask.Get(Tsk.Cost));
Console.WriteLine(project.RootTask.Get(Tsk.FixedCost));
Console.WriteLine(project.RootTask.Get(Tsk.RemainingCost));
Console.WriteLine(project.RootTask.Get(Tsk.CostVariance));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


