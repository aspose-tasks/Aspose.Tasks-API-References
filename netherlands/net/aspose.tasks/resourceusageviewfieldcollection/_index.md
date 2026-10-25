---
title: "Klasse ResourceUsageViewFieldCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.ResourceUsageViewFieldCollection klasse. Vertegenwoordigt een collectie van ResourceUsageViewField-waarden."
type: docs
weight: 1830
url: /nl/net/aspose.tasks/resourceusageviewfieldcollection/
---
## ResourceUsageViewFieldCollection class

Vertegenwoordigt een collectie van [`ResourceUsageViewField`](../resourceusageviewfield/) waarden.

```csharp
public class ResourceUsageViewFieldCollection : IList<ResourceUsageViewField>
```

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/resourceusageviewfieldcollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [ToList](../../aspose.tasks/resourceusageviewfieldcollection/tolist/)() | Converteert de instantie van de `ResourceUsageViewFieldCollection` klasse naar een lijst die de instanties van de [`ResourceUsageViewField`](../resourceusageviewfield/) klasse bevat. |

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

* enum [ResourceUsageViewField](../resourceusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


