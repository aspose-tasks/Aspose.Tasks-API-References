---
title: "Klasse VbaReferenceCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.VbaReferenceCollection klasse. Vertegenwoordigt een collectie van VbaReference-objecten"
type: docs
weight: 2880
url: /nl/net/aspose.tasks/vbareferencecollection/
---
## VbaReferenceCollection class

Vertegenwoordigt een collectie van [`VbaReference`](../vbareference/) objecten.

```csharp
public class VbaReferenceCollection : ReadOnlyCollectionBase<VbaReference>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/readonlycollectionbase-1/count/) { get; } |  |
| [Item](../../aspose.tasks/readonlycollectionbase-1/item/) { get; set; } |  |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/readonlycollectionbase-1/add/)(VbaReference) |  |
| [GetEnumerator](../../aspose.tasks/readonlycollectionbase-1/getenumerator/)() |  |
| [ToList](../../aspose.tasks/readonlycollectionbase-1/tolist/)() |  |

## Voorbeelden

Toont hoe te werken met VBA-referentiecollectie.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Reference count " + project.VbaProject.References.Count);

foreach (var reference in project.VbaProject.References)
{
    Console.WriteLine("Identifier: " + reference.LibIdentifier);
    Console.WriteLine("Name: " + reference.Name);
}
```

### Zie ook

* class [ReadOnlyCollectionBase&lt;T&gt;](../readonlycollectionbase-1/)
* class [VbaReference](../vbareference/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


