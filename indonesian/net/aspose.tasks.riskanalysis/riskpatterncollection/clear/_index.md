---
title: "RiskPatternCollection.Clear"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode RiskPatternCollection. Menghapus semua item dari koleksi ini."
type: docs
weight: 50
url: /id/net/aspose.tasks.riskanalysis/riskpatterncollection/clear/
---
## RiskPatternCollection.Clear method

Menghapus semua item dari koleksi ini.

```csharp
public void Clear()
```

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

* class [RiskPatternCollection](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskpatterncollection/)
* assembly [Aspose.Tasks](../../../)


