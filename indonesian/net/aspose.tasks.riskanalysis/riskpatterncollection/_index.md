---
title: "Kelas RiskPatternCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.RiskAnalysis.RiskPatternCollection class. Mewakili koleksi yang berisi instance kelas RiskPattern"
type: docs
weight: 1940
url: /id/net/aspose.tasks.riskanalysis/riskpatterncollection/
---
## RiskPatternCollection class

Mewakili koleksi yang berisi instance kelas [`RiskPattern`](../riskpattern/).

```csharp
public class RiskPatternCollection : ICollection<RiskPattern>, IDictionary<Task, RiskPattern>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../aspose.tasks.riskanalysis/riskpatterncollection/count/) { get; } | Mendapatkan jumlah elemen yang terdapat dalam koleksi ini. |
| [IsReadOnly](../../aspose.tasks.riskanalysis/riskpatterncollection/isreadonly/) { get; } | Mendapatkan nilai yang menunjukkan apakah koleksi ini hanya-baca; jika tidak, false. |
| [Item](../../aspose.tasks.riskanalysis/riskpatterncollection/item/) { get; } | Mendapatkan instance kelas [`RiskPattern`](../riskpattern/) untuk tugas yang ditentukan. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Add](../../aspose.tasks.riskanalysis/riskpatterncollection/add/)(RiskPattern) | Menambahkan instance kelas [`RiskPattern`](../riskpattern/) ke koleksi ini. |
| [Clear](../../aspose.tasks.riskanalysis/riskpatterncollection/clear/)() | Menghapus semua item dari koleksi ini. |
| [Contains](../../aspose.tasks.riskanalysis/riskpatterncollection/contains/)(RiskPattern) | Mengembalikan true jika item yang ditentukan ditemukan dalam koleksi ini; jika tidak, false. |
| [CopyTo](../../aspose.tasks.riskanalysis/riskpatterncollection/copyto/)(RiskPattern[], int) | Menyalin elemen-elemen koleksi ini ke array yang ditentukan, mulai dari indeks array yang ditentukan. |
| [GetEnumerator](../../aspose.tasks.riskanalysis/riskpatterncollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [Remove](../../aspose.tasks.riskanalysis/riskpatterncollection/remove/)(RiskPattern) | Menghapus kemunculan pertama dari objek tertentu dari koleksi ini. |

## Contoh

Menampilkan cara bekerja dengan koleksi pola risiko.

```csharp
var settings = new RiskAnalysisSettings
{
    // Atur jumlah iterasi untuk simulasi Monte Carlo (nilai default adalah 100).
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task1 = project.RootTask.Children.GetById(17);
var task2 = project.RootTask.Children.GetById(18);

// selama RiskPatternCollection tidak bersifat read-only
Console.WriteLine("Is pattern collection read-only?: " + settings.Patterns.IsReadOnly);

// bisa menambahkan pola baru 
var pattern1 = new RiskPattern(task1)
{
    Distribution = ProbabilityDistributionType.Normal,
    Optimistic = 60,
    Pessimistic = 140,
    ConfidenceLevel = ConfidenceLevel.CL75
};
var pattern2 = new RiskPattern(task2)
{
    Distribution = ProbabilityDistributionType.Normal,
    Optimistic = 70,
    Pessimistic = 130,
    ConfidenceLevel = ConfidenceLevel.CL75
};

settings.Patterns.Add(pattern1);
settings.Patterns.Add(pattern2);

// mengiterasi pola yang ditambahkan
Console.WriteLine("Patterns count: " + settings.Patterns.Count);
foreach (var pattern in settings.Patterns)
{
    Console.WriteLine("Task: " + pattern.Task);
    Console.WriteLine("Distribution: " + pattern.Distribution);
    Console.WriteLine("Optimistic: " + pattern.Optimistic);
    Console.WriteLine("Pessimistic: " + pattern.Pessimistic);
    Console.WriteLine("Confidence Level: " + pattern.ConfidenceLevel);
    Console.WriteLine();
}

// mengedit pola dalam koleksi dengan menggunakan akses indeks
settings.Patterns[task1].Optimistic = 70;
settings.Patterns[task1].Pessimistic = 140;

// memeriksa pola setelah pengeditan
Console.WriteLine("Print edited patterns: ");
foreach (var pattern in settings.Patterns)
{
    Console.WriteLine("Task: " + pattern.Task);
    Console.WriteLine("Distribution: " + pattern.Distribution);
    Console.WriteLine("Optimistic: " + pattern.Optimistic);
    Console.WriteLine("Pessimistic: " + pattern.Pessimistic);
    Console.WriteLine("Confidence Level: " + pattern.ConfidenceLevel);
    Console.WriteLine();
}

// kita dapat menghapus pola
Console.WriteLine("Removing the first pattern...");
settings.Patterns.Remove(pattern1);

// memeriksa bahwa pola tidak ada dalam koleksi
Console.WriteLine("Is collection contains the first pattern?: " + settings.Patterns.Contains(pattern1));

// seseorang dapat membersihkan koleksi dengan dua cara

// menyalin pola ke dalam array dan menghapusnya satu per satu
var patterns = new RiskPattern[settings.Patterns.Count];
settings.Patterns.CopyTo(patterns, 0);
foreach (var pattern in patterns)
{
    settings.Patterns.Remove(pattern);
}

// atau dapat mengosongkan koleksi pola sepenuhnya
settings.Patterns.Clear();
```

### Lihat Juga

* class [RiskPattern](../riskpattern/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


