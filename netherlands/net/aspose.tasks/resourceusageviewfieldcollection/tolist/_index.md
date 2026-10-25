---
title: "ResourceUsageViewFieldCollection.ToList"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ResourceUsageViewFieldCollection methode. Converteert de instantie van de ResourceUsageViewFieldCollection klasse naar een lijst die de instanties van de ResourceUsageViewField klasse bevat."
type: docs
weight: 20
url: /nl/net/aspose.tasks/resourceusageviewfieldcollection/tolist/
---
## ResourceUsageViewFieldCollection.ToList method

Converteert de instantie van de [`ResourceUsageViewFieldCollection`](../) klasse naar een lijst die de instanties van de [`ResourceUsageViewField`](../../resourceusageviewfield/) klasse bevat.

```csharp
public IList<ResourceUsageViewField> ToList()
```

### Retourwaarde

De instantie van de [`ResourceUsageViewFieldCollection`](../) klasse geconverteerd naar een lijst die de instanties van de [`ResourceUsageViewField`](../../resourceusageviewfield/) klasse bevat.

## Voorbeelden

Toont hoe te werken met de veldcollectie van een ResourceUsageView‑instantie.

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// men kan de collectie omzetten naar een lijst van ResourceUsageViewField.
IList<ResourceUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### Zie ook

* enum [ResourceUsageViewField](../../resourceusageviewfield/)
* class [ResourceUsageViewFieldCollection](../)
* namespace [Aspose.Tasks](../../resourceusageviewfieldcollection/)
* assembly [Aspose.Tasks](../../../)


