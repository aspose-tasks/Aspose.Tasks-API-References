---
title: "Kelas RiskItemStatistics"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.RiskAnalysis.RiskItemStatistics class. Mewakili sebuah item yang menyimpan data statistik untuk tugas proyek yang dianalisis"
type: docs
weight: 1900
url: /id/net/aspose.tasks.riskanalysis/riskitemstatistics/
---
## RiskItemStatistics class

Mewakili item yang menyimpan data statistik untuk tugas proyek yang dianalisis.

```csharp
public class RiskItemStatistics
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [ExpectedValue](../../aspose.tasks.riskanalysis/riskitemstatistics/expectedvalue/) { get; } | Mendapatkan nilai harapan dari item risiko. |
| [ItemType](../../aspose.tasks.riskanalysis/riskitemstatistics/itemtype/) { get; } | Mendapatkan sebuah instance dari enumerasi [`RiskItemType`](../riskitemtype/). |
| [Maximum](../../aspose.tasks.riskanalysis/riskitemstatistics/maximum/) { get; } | Mendapatkan nilai maksimum yang dihasilkan selama simulasi Monte Carlo. |
| [Minimum](../../aspose.tasks.riskanalysis/riskitemstatistics/minimum/) { get; } | Mendapatkan nilai minimum yang dihasilkan selama simulasi Monte Carlo. |
| [StandardDeviation](../../aspose.tasks.riskanalysis/riskitemstatistics/standarddeviation/) { get; } | Mendapatkan deviasi standar dari item risiko. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [GetPercentile](../../aspose.tasks.riskanalysis/riskitemstatistics/getpercentile/)(int) | Mendapatkan nilai di bawah mana persentase tertentu dari sampel yang dihasilkan berada. |
| override [ToString](../../aspose.tasks.riskanalysis/riskitemstatistics/tostring/)() | Mengembalikan representasi string singkat dari sebuah item risiko. Detail tepat dari representasi tersebut tidak ditentukan dan dapat berubah. |

## Contoh

Menampilkan cara menghitung statistik risiko.

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

// Analisis risiko proyek
var analyzer = new RiskAnalyzer(settings);
var analysisResult = analyzer.Analyze(project);
var statistics = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Short statistic: " + statistics);
Console.WriteLine();
Console.WriteLine("Statistic details: ");
Console.WriteLine("Item Type: {0}", statistics.ItemType);
Console.WriteLine("Expected value: {0}", statistics.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", statistics.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", statistics.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", statistics.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", statistics.GetPercentile(90));
Console.WriteLine("Minimum: {0}", statistics.Minimum);
Console.WriteLine("Maximum: {0}", statistics.Maximum);
```

### Lihat Juga

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


