---
title: "TaskUsageViewFieldCollection.ToList"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode TaskUsageViewFieldCollection. Retourne une liste qui contient tous les éléments de cette collection"
type: docs
weight: 20
url: /fr/net/aspose.tasks/taskusageviewfieldcollection/tolist/
---
## TaskUsageViewFieldCollection.ToList method

Renvoie une liste qui contient tous les éléments de cette collection.

```csharp
public IList<TaskUsageViewField> ToList()
```

### Valeur de retour

retourne une liste qui contient tous les éléments de cette collection.

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

* enum [TaskUsageViewField](../../taskusageviewfield/)
* class [TaskUsageViewFieldCollection](../)
* namespace [Aspose.Tasks](../../taskusageviewfieldcollection/)
* assembly [Aspose.Tasks](../../../)


