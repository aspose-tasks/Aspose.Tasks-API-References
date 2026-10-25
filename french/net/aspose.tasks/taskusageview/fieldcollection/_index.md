---
title: "TaskUsageView.FieldCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété TaskUsageView. Obtient l'objet TaskUsageViewFieldCollection de ce TaskUsageView"
type: docs
weight: 10
url: /fr/net/aspose.tasks/taskusageview/fieldcollection/
---
## TaskUsageView.FieldCollection property

Obtient l'objet [`TaskUsageViewFieldCollection`](../../taskusageviewfieldcollection/) de ce TaskUsageView.

```csharp
public TaskUsageViewFieldCollection FieldCollection { get; }
```

## Exemples

Montre comment lire les champs de la vue d'utilisation des tâches.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### Voir aussi

* class [TaskUsageViewFieldCollection](../../taskusageviewfieldcollection/)
* class [TaskUsageView](../)
* namespace [Aspose.Tasks](../../taskusageview/)
* assembly [Aspose.Tasks](../../../)


