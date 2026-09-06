---
title: "Enum TaskLinkType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Enum Aspose.Tasks.TaskLinkType. Spécifie le type de dépendance des tâches"
type: docs
weight: 2440
url: /fr/net/aspose.tasks/tasklinktype/
---
## TaskLinkType enumeration

Spécifie le type de dépendance des tâches.

```csharp
public enum TaskLinkType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| FinishToFinish | `0` | Relation Fin-Fin |
| FinishToStart | `1` | Relation Fin-Début |
| StartToFinish | `2` | Relation Début-Fin |
| StartToStart | `3` | Relation Début-Début |

## Exemples

Montre comment obtenir/définir un type de lien d'un lien de tâche.

```csharp
var project = new Project();

// Ajouter de nouvelles tâches
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// Lier des tâches avec le type de lien défini sur Start to Start
var newLink = project.TaskLinks.Add(pred, succ);
newLink.LinkType = TaskLinkType.StartToStart;

foreach (var link in project.TaskLinks)
{
    Console.WriteLine("Task Link Type: " + link.LinkType.ToString());
}
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


