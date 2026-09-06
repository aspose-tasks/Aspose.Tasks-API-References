---
title: "TaskUsageViewFieldCollection.GetEnumerator"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode TaskUsageViewFieldCollection. Retourne un énumérateur pour cette collection"
type: docs
weight: 10
url: /fr/net/aspose.tasks/taskusageviewfieldcollection/getenumerator/
---
## TaskUsageViewFieldCollection.GetEnumerator method

Renvoie un énumérateur pour cette collection.

```csharp
public IEnumerator<TaskUsageViewField> GetEnumerator()
```

### Valeur de retour

un énumérateur pour cette collection.

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


