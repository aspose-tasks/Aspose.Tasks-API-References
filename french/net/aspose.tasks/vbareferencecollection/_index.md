---
title: "Classe VbaReferenceCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.VbaReferenceCollection. Représente une collection d'objets VbaReference"
type: docs
weight: 2880
url: /fr/net/aspose.tasks/vbareferencecollection/
---
## VbaReferenceCollection class

Représente une collection d'objets [`VbaReference`](../vbareference/).

```csharp
public class VbaReferenceCollection : ReadOnlyCollectionBase<VbaReference>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.tasks/readonlycollectionbase-1/count/) { get; } |  |
| [Item](../../aspose.tasks/readonlycollectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.tasks/readonlycollectionbase-1/add/)(VbaReference) |  |
| [GetEnumerator](../../aspose.tasks/readonlycollectionbase-1/getenumerator/)() |  |
| [ToList](../../aspose.tasks/readonlycollectionbase-1/tolist/)() |  |

## Exemples

Montre comment travailler avec une collection de références VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Reference count " + project.VbaProject.References.Count);

foreach (var reference in project.VbaProject.References)
{
    Console.WriteLine("Identifier: " + reference.LibIdentifier);
    Console.WriteLine("Name: " + reference.Name);
}
```

### Voir aussi

* class [ReadOnlyCollectionBase&lt;T&gt;](../readonlycollectionbase-1/)
* class [VbaReference](../vbareference/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


