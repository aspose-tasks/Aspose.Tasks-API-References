---
title: "Klasse VbaModuleAttributeCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.VbaModuleAttributeCollection‑klasse. Vertegenwoordigt een collectie van VbaModuleAttribute‑objecten"
type: docs
weight: 2830
url: /nl/net/aspose.tasks/vbamoduleattributecollection/
---
## VbaModuleAttributeCollection class

Vertegenwoordigt een collectie van [`VbaModuleAttribute`](../vbamoduleattribute/) objecten.

```csharp
public class VbaModuleAttributeCollection : ReadOnlyCollectionBase<VbaModuleAttribute>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/readonlycollectionbase-1/count/) { get; } |  |
| [Item](../../aspose.tasks/readonlycollectionbase-1/item/) { get; set; } |  |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/readonlycollectionbase-1/add/)(VbaModuleAttribute) |  |
| [GetEnumerator](../../aspose.tasks/readonlycollectionbase-1/getenumerator/)() |  |
| [ToList](../../aspose.tasks/readonlycollectionbase-1/tolist/)() |  |

## Voorbeelden

Toont hoe te itereren over de attribuutcollectie van een VBA‑module.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("Attribute Name: " + attribute.Key);
        Console.WriteLine("Attribute Value: " + attribute.Value);
    }
}
```

### Zie ook

* class [ReadOnlyCollectionBase&lt;T&gt;](../readonlycollectionbase-1/)
* class [VbaModuleAttribute](../vbamoduleattribute/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


