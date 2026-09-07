---
title: "SplitPartCollection.Item"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "SplitPartCollection property. Retrieves a tasks split part at the given index"
type: docs
weight: 20
url: /id/net/aspose.tasks/splitpartcollection/item/
---
## SplitPartCollection indexer

Mengambil bagian split tugas pada indeks yang diberikan.

```csharp
public SplitPart this[int index] { get; set; }
```

| Parameter | Deskripsi |
| --- | --- |
| index | The part index. |

### Nilai Kembali

a split part.

## Catatan

The index is zero-based. Returns null if the index is outside array's boundaries.

## Contoh

Menampilkan cara bekerja dengan koleksi bagian split.

```csharp
var project = new Project(DataDir + "Splits.mpp");

var task = project.RootTask.Children.GetById(1);

// iterasi atas bagian split
Console.WriteLine("Iterate over split parts");
Console.WriteLine("Split parts count:" + task.SplitParts.Count);
foreach (var splitPart in task.SplitParts)
{
    Console.WriteLine("Start: " + splitPart.Start);
    Console.WriteLine("Finish: " + splitPart.Finish);
}

// dapatkan bagian berdasarkan indeks
var split = task.SplitParts[0];
Console.WriteLine("Split start: " + split.Start);

// lakukan beberapa pekerjaan dengan bagian split pertama dari tugas
```

### Lihat Juga

* class [SplitPart](../../splitpart/)
* class [SplitPartCollection](../)
* namespace [Aspose.Tasks](../../splitpartcollection/)
* assembly [Aspose.Tasks](../../../)


