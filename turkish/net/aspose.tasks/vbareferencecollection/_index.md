---
title: "Sınıf VbaReferenceCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.VbaReferenceCollection sınıfı. VbaReference nesnelerinin bir koleksiyonunu temsil eder"
type: docs
weight: 2880
url: /tr/net/aspose.tasks/vbareferencecollection/
---
## VbaReferenceCollection class

[`VbaReference`](../vbareference/) nesnelerinin bir koleksiyonunu temsil eder.

```csharp
public class VbaReferenceCollection : ReadOnlyCollectionBase<VbaReference>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/readonlycollectionbase-1/count/) { get; } |  |
| [Item](../../aspose.tasks/readonlycollectionbase-1/item/) { get; set; } |  |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/readonlycollectionbase-1/add/)(VbaReference) |  |
| [GetEnumerator](../../aspose.tasks/readonlycollectionbase-1/getenumerator/)() |  |
| [ToList](../../aspose.tasks/readonlycollectionbase-1/tolist/)() |  |

## Örnekler

VBA referans koleksiyonuyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Reference count " + project.VbaProject.References.Count);

foreach (var reference in project.VbaProject.References)
{
    Console.WriteLine("Identifier: " + reference.LibIdentifier);
    Console.WriteLine("Name: " + reference.Name);
}
```

### Ayrıca Bakınız

* class [ReadOnlyCollectionBase&lt;T&gt;](../readonlycollectionbase-1/)
* class [VbaReference](../vbareference/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


