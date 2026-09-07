---
title: "Kelas SplitPartCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.SplitPartCollection. Koleksi yang mewakili bagian-bagian dari sebuah tugas."
type: docs
weight: 2300
url: /id/net/aspose.tasks/splitpartcollection/
---
## SplitPartCollection class

Koleksi yang mewakili bagian-bagian dari sebuah tugas.

```csharp
public class SplitPartCollection : IList<SplitPart>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../aspose.tasks/splitpartcollection/count/) { get; } | Mendapatkan jumlah bagian dalam koleksi. |
| [Item](../../aspose.tasks/splitpartcollection/item/) { get; set; } | Mengambil bagian split tugas pada indeks yang diberikan. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/splitpartcollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [ToArray](../../aspose.tasks/splitpartcollection/toarray/)() | Menyalin semua bagian dari koleksi ke array baru. |

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

* class [SplitPart](../splitpart/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


