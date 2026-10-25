---
title: "TaskBaseline.CompareTo"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode TaskBaseline. Implémentation de l'interface IComparable. Compare cette instance à l'objet Baseline spécifié"
type: docs
weight: 90
url: /fr/net/aspose.tasks/taskbaseline/compareto/
---
## TaskBaseline.CompareTo method

Implémentation de l'interface IComparable. Compare cette instance à l'objet Baseline spécifié.

```csharp
public int CompareTo(TaskBaseline other)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| autre | TaskBaseline | l'objet Baseline spécifié avec lequel comparer cette instance. |

### Valeur de retour

renvoie -1 si cette instance est inférieure à l'objet spécifié, 1 si cette instance est supérieure à l'objet spécifié ; sinon renvoie 0

## Exemples

Montre comment vérifier l'égalité des baselines.

```csharp
var project = new Project();

// création de TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// afficher la durée de la baseline de la tâche
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// L'égalité des baselines est vérifiée par rapport aux valeurs de la baseline.
Console.WriteLine("Baseline Number 1: " + baseline1.BaselineNumber);
Console.WriteLine("Baseline Number 2: " + baseline2.BaselineNumber);
Console.WriteLine("Are baselines equal: " + baseline1.Equals(baseline2));
```

### Voir aussi

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


