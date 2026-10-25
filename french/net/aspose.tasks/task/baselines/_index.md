---
title: "Task.Baselines"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Task. Obtient ou définit la collection des valeurs de base du task"
type: docs
weight: 130
url: /fr/net/aspose.tasks/task/baselines/
---
## Task.Baselines property

Obtient ou définit la collection des valeurs de référence de la tâche.

```csharp
public TaskBaselineCollection Baselines { get; set; }
```

## Exemples

Montre comment lire les baselines du task.

```csharp
var project = new Project();

// définir une baseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// Afficher la durée de la ligne de base de la tâche
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration is 1 day: {0}", baseline.Duration.ToString().Equals("1 day"));
    Console.WriteLine("BaselineStart is same as Task Start: {0}", baseline.Start.Equals(task.Get(Tsk.Start)));
    Console.WriteLine("BaselineFinish is same as Task Finish: {0}", baseline.Finish.Equals(task.Get(Tsk.Finish)));
}
```

### Voir aussi

* class [TaskBaselineCollection](../../taskbaselinecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


