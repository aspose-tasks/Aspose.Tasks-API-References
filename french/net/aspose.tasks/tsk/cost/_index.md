---
title: "Tsk.Cost"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Le coût total prévu ou programmé pour une tâche, basé sur les coûts déjà engagés pour le travail effectué par les ressources assignées aux tâches, ainsi que sur les coûts prévus pour le travail restant"
type: docs
weight: 230
url: /fr/net/aspose.tasks/tsk/cost/
---
## Tsk.Cost field

Le coût total prévu ou projeté pour une tâche, basé sur les coûts déjà engagés pour le travail effectué par les ressources affectées aux tâches, en plus des coûts prévus pour le travail restant.

```csharp
public static readonly Key<decimal, TaskKey> Cost;
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


