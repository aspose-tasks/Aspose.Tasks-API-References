---
title: "ResourceUsageViewFieldCollection.ToList"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ResourceUsageViewFieldCollection. Convertit l'instance de la classe ResourceUsageViewFieldCollection en une liste contenant les instances de la classe ResourceUsageViewField"
type: docs
weight: 20
url: /fr/net/aspose.tasks/resourceusageviewfieldcollection/tolist/
---
## ResourceUsageViewFieldCollection.ToList method

Convertit l'instance de la classe [`ResourceUsageViewFieldCollection`](../) en une liste contenant les instances de la classe [`ResourceUsageViewField`](../../resourceusageviewfield/).

```csharp
public IList<ResourceUsageViewField> ToList()
```

### Valeur de retour

L'instance de la classe [`ResourceUsageViewFieldCollection`](../) convertie en liste contenant les instances de la classe [`ResourceUsageViewField`](../../resourceusageviewfield/).

## Exemples

Montre comment travailler avec la collection de champs d'une instance ResourceUsageView.

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// on peut transformer la collection en une liste de ResourceUsageViewField
IList<ResourceUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### Voir aussi

* enum [ResourceUsageViewField](../../resourceusageviewfield/)
* class [ResourceUsageViewFieldCollection](../)
* namespace [Aspose.Tasks](../../resourceusageviewfieldcollection/)
* assembly [Aspose.Tasks](../../../)


