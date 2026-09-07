---
title: "Kelas VbaReferenceCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.VbaReferenceCollection. Mewakili koleksi objek VbaReference"
type: docs
weight: 2880
url: /id/net/aspose.tasks/vbareferencecollection/
---
## VbaReferenceCollection class

Mewakili koleksi objek [`VbaReference`](../vbareference/).

```csharp
public class VbaReferenceCollection : ReadOnlyCollectionBase<VbaReference>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../aspose.tasks/readonlycollectionbase-1/count/) { get; } |  |
| [Item](../../aspose.tasks/readonlycollectionbase-1/item/) { get; set; } |  |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Add](../../aspose.tasks/readonlycollectionbase-1/add/)(VbaReference) |  |
| [GetEnumerator](../../aspose.tasks/readonlycollectionbase-1/getenumerator/)() |  |
| [ToList](../../aspose.tasks/readonlycollectionbase-1/tolist/)() |  |

## Contoh

Menampilkan cara bekerja dengan koleksi referensi VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Reference count " + project.VbaProject.References.Count);

foreach (var reference in project.VbaProject.References)
{
    Console.WriteLine("Identifier: " + reference.LibIdentifier);
    Console.WriteLine("Name: " + reference.Name);
}
```

### Lihat Juga

* class [ReadOnlyCollectionBase&lt;T&gt;](../readonlycollectionbase-1/)
* class [VbaReference](../vbareference/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


