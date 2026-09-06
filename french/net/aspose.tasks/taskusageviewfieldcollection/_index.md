---
title: "Classe TaskUsageViewFieldCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.TaskUsageViewFieldCollection. Représente une collection de valeurs TaskUsageViewField."
type: docs
weight: 2500
url: /fr/net/aspose.tasks/taskusageviewfieldcollection/
---
## TaskUsageViewFieldCollection class

Représente une collection de valeurs [`TaskUsageViewField`](../taskusageviewfield/).

```csharp
public class TaskUsageViewFieldCollection : IList<TaskUsageViewField>
```

## Méthodes

| Nom | Description |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/taskusageviewfieldcollection/getenumerator/)() | Renvoie un énumérateur pour cette collection. |
| [ToList](../../aspose.tasks/taskusageviewfieldcollection/tolist/)() | Renvoie une liste qui contient tous les éléments de cette collection. |

## Exemples

Montre comment travailler avec la collection de champs d'une instance TaskUsageView.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// On peut transformer la collection en une liste de TaskUsageViewField.
IList<TaskUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### Voir aussi

* enum [TaskUsageViewField](../taskusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


