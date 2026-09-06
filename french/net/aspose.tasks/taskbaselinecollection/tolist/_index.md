---
title: "TaskBaselineCollection.ToList"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "TaskBaselineCollection méthode. Convertit l'objet TaskBaselineCollection en une liste d'objets TaskBaseline"
type: docs
weight: 60
url: /fr/net/aspose.tasks/taskbaselinecollection/tolist/
---
## TaskBaselineCollection.ToList method

Convertit l'objet TaskBaselineCollection en une liste d'objets [`TaskBaseline`](../../taskbaseline/).

```csharp
public List<TaskBaseline> ToList()
```

### Valeur de retour

Liste d'objets [`TaskBaseline`](../../taskbaseline/).

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

* class [TaskBaseline](../../taskbaseline/)
* class [TaskBaselineCollection](../)
* namespace [Aspose.Tasks](../../taskbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


