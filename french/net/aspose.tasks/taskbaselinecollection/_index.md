---
title: "Classe TaskBaselineCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.TaskBaselineCollection classe. Représente une collection d'objets TaskBaseline"
type: docs
weight: 2380
url: /fr/net/aspose.tasks/taskbaselinecollection/
---
## TaskBaselineCollection class

Représente une collection d'objets [`TaskBaseline`](../taskbaseline/).

```csharp
public class TaskBaselineCollection : IList<TaskBaseline>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.tasks/taskbaselinecollection/count/) { get; } | Obtient le nombre d'objets contenus dans cet objet TaskBaselineCollection. |
| [Item](../../aspose.tasks/taskbaselinecollection/item/) { get; set; } | Renvoie l'élément à l'index spécifié. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.tasks/taskbaselinecollection/add/)(TaskBaseline) | Ceci est l'implémentation factice de la méthode Add de ICollection, qui ne lance que NotSupportedException |
| [GetEnumerator](../../aspose.tasks/taskbaselinecollection/getenumerator/)() | Renvoie un énumérateur pour cette collection. |
| [Remove](../../aspose.tasks/taskbaselinecollection/remove/)(TaskBaseline) | Supprime la ligne de base de cette collection. |
| [ToList](../../aspose.tasks/taskbaselinecollection/tolist/)() | Convertit l'objet TaskBaselineCollection en une liste d'objets [`TaskBaseline`](../taskbaseline/). |

## Exemples

Montre comment travailler avec des collections de lignes de base de tâches.

```csharp
var project = new Project();

// créer des lignes de base de projet
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// imprimer les lignes de base de tâches
Console.WriteLine("Count of task baselines: " + task.Baselines.Count);
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration: {0}", baseline.Duration);
    Console.WriteLine("Baseline start: {0}", baseline.Start);
    Console.WriteLine("Baseline finish: {0}", baseline.Finish);
}

// effaçons toutes les lignes de base
List<TaskBaseline> baselines = task.Baselines.ToList();
for (var i = 0; i < baselines.Count; i++)
{
    task.Baselines.Remove(baselines[i]);
}
```

### Voir aussi

* class [TaskBaseline](../taskbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


