---
title: "ResourceUsageViewFieldCollection.GetEnumerator"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ResourceUsageViewFieldCollection. Retourne un énumérateur pour cette collection"
type: docs
weight: 10
url: /fr/net/aspose.tasks/resourceusageviewfieldcollection/getenumerator/
---
## ResourceUsageViewFieldCollection.GetEnumerator method

Renvoie un énumérateur pour cette collection.

```csharp
public IEnumerator<ResourceUsageViewField> GetEnumerator()
```

### Valeur de retour

un énumérateur pour cette collection.

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


