---
title: "SplitPartCollection.Count"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti SplitPartCollection. Mengembalikan jumlah bagian dalam koleksi"
type: docs
weight: 10
url: /id/net/aspose.tasks/splitpartcollection/count/
---
## SplitPartCollection.Count property

Mendapatkan jumlah bagian dalam koleksi.

```csharp
public int Count { get; }
```

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

* class [SplitPartCollection](../)
* namespace [Aspose.Tasks](../../splitpartcollection/)
* assembly [Aspose.Tasks](../../../)


