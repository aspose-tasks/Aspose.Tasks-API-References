---
title: "Kelas RiskItemStatisticsCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.RiskAnalysis.RiskItemStatisticsCollection. Mewakili koleksi yang berisi instance dari kelas RiskItemStatistics"
type: docs
weight: 1910
url: /id/net/aspose.tasks.riskanalysis/riskitemstatisticscollection/
---
## RiskItemStatisticsCollection class

Mewakili koleksi yang berisi instance dari kelas [`RiskItemStatistics`](../riskitemstatistics/).

```csharp
public class RiskItemStatisticsCollection : IDictionary<Task, RiskItemStatistics>, 
    IEnumerable<RiskItemStatistics>
```

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Get](../../aspose.tasks.riskanalysis/riskitemstatisticscollection/get/)(Task) | Mengembalikan sebuah instance dari kelas [`RiskItemStatistics`](../riskitemstatistics/) yang terdapat dalam koleksi ini dan terkait dengan objek Task yang ditentukan; null jika item tidak ditemukan. |
| [GetEnumerator](../../aspose.tasks.riskanalysis/riskitemstatisticscollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |

## Contoh

Menampilkan cara bekerja dengan koleksi statistik risiko.

```csharp
var settings = new RiskAnalysisSettings
{
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// Inisialisasi pola risiko
var pattern = new RiskPattern(task)
{
    // Pilih tipe distribusi untuk generator angka acak guna menghasilkan nilai yang mungkin (hanya dua tipe yang saat ini didukung, yaitu normal dan uniform)
    // Untuk detail lebih lanjut lihat di sini: https://en.wikipedia.org/wiki/Normal_distribution)
    Distribution = ProbabilityDistributionType.Normal,

    // Atur persentase durasi tugas yang paling mungkin yang dapat terjadi dalam skenario proyek terbaik
    // Nilai default adalah 75, yang berarti bahwa jika durasi tugas yang diperkirakan adalah 4 hari maka durasi optimis akan menjadi 3 hari
    Optimistic = 70,

    // Atur persentase durasi tugas yang paling mungkin yang dapat terjadi dalam skenario proyek terburuk
    // Nilai default adalah 125, yang berarti bahwa jika durasi tugas yang diperkirakan adalah 4 hari maka durasi pesimis akan menjadi 5 hari.
    Pessimistic = 130,

    // Atur tingkat kepercayaan yang sesuai dengan persentase waktu nilai aktual berada di antara perkiraan optimis dan pesimis.
    // Anda dapat menganggapnya sebagai nilai deviasi standar: semakin tidak pasti perkiraan Anda, semakin besar nilai deviasi standar yang digunakan dalam generator angka acak.
    ConfidenceLevel = ConfidenceLevel.CL75
};
settings.Patterns.Add(pattern);

var analyzer = new RiskAnalyzer(settings);
var analysisResult = analyzer.Analyze(project);

// iterasi semua item statistik
var statistics = analysisResult.GetRiskItems(RiskItemType.EarlyFinish);

foreach (var statistic in statistics)
{
    Console.WriteLine("Short statistic: " + statistic);
    Console.WriteLine();
    Console.WriteLine("Statistic details: ");
    Console.WriteLine("Item Type: {0}", statistic.ItemType);
    Console.WriteLine("Expected value: {0}", statistic.ExpectedValue);
    Console.WriteLine("StandardDeviation: {0}", statistic.StandardDeviation);
    Console.WriteLine("10% Percentile: {0}", statistic.GetPercentile(10));
    Console.WriteLine("50% Percentile: {0}", statistic.GetPercentile(50));
    Console.WriteLine("90% Percentile: {0}", statistic.GetPercentile(90));
    Console.WriteLine("Minimum: {0}", statistic.Minimum);
    Console.WriteLine("Maximum: {0}", statistic.Maximum);
}

// atau dapatkan statistik tertentu
var itemStatistics = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Print the specific statistic: ");
Console.WriteLine("Expected value: {0}", itemStatistics.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", itemStatistics.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", itemStatistics.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", itemStatistics.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", itemStatistics.GetPercentile(90));
Console.WriteLine("Minimum: {0}", itemStatistics.Minimum);
Console.WriteLine("Maximum: {0}", itemStatistics.Maximum);
```

### Lihat Juga

* class [Task](../../aspose.tasks/task/)
* class [RiskItemStatistics](../riskitemstatistics/)
* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


