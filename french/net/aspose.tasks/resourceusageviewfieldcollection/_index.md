---
title: "Classe ResourceUsageViewFieldCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.ResourceUsageViewFieldCollection. Représente une collection de valeurs ResourceUsageViewField"
type: docs
weight: 1830
url: /fr/net/aspose.tasks/resourceusageviewfieldcollection/
---
## ResourceUsageViewFieldCollection class

Représente une collection de valeurs [`ResourceUsageViewField`](../resourceusageviewfield/).

```csharp
public class ResourceUsageViewFieldCollection : IList<ResourceUsageViewField>
```

## Méthodes

| Nom | Description |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/resourceusageviewfieldcollection/getenumerator/)() | Renvoie un énumérateur pour cette collection. |
| [ToList](../../aspose.tasks/resourceusageviewfieldcollection/tolist/)() | Convertit l'instance de la classe `ResourceUsageViewFieldCollection` en une liste contenant les instances de la classe [`ResourceUsageViewField`](../resourceusageviewfield/). |

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

* enum [ResourceUsageViewField](../resourceusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


