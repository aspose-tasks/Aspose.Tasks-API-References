---
title: "TaskBaselineCollection.GetEnumerator"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "TaskBaselineCollection méthode. Retourne un énumérateur pour cette collection"
type: docs
weight: 40
url: /fr/net/aspose.tasks/taskbaselinecollection/getenumerator/
---
## TaskBaselineCollection.GetEnumerator method

Renvoie un énumérateur pour cette collection.

```csharp
public IEnumerator<TaskBaseline> GetEnumerator()
```

### Valeur de retour

un énumérateur pour cette collection.

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


