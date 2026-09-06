---
title: "ResourceUsageView.FieldCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ResourceUsageView. Obtient l'objet ResourceUsageViewFieldCollection de ce ResourceUsageView"
type: docs
weight: 10
url: /fr/net/aspose.tasks/resourceusageview/fieldcollection/
---
## ResourceUsageView.FieldCollection property

Obtient l'objet [`ResourceUsageViewFieldCollection`](../../resourceusageviewfieldcollection/) de ce ResourceUsageView.

```csharp
public ResourceUsageViewFieldCollection FieldCollection { get; }
```

## Exemples

Montre comment lire les champs d’affichage d’utilisation des ressources.

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### Voir aussi

* class [ResourceUsageViewFieldCollection](../../resourceusageviewfieldcollection/)
* class [ResourceUsageView](../)
* namespace [Aspose.Tasks](../../resourceusageview/)
* assembly [Aspose.Tasks](../../../)


