---
title: "SplitPartCollection.GetEnumerator"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode SplitPartCollection. Mengembalikan enumerator untuk koleksi ini"
type: docs
weight: 30
url: /id/net/aspose.tasks/splitpartcollection/getenumerator/
---
## SplitPartCollection.GetEnumerator method

Mengembalikan enumerator untuk koleksi ini.

```csharp
public IEnumerator<SplitPart> GetEnumerator()
```

### Nilai Kembali

enumerator untuk koleksi ini.

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


