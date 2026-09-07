---
title: "Kelas RiskAnalysisSettings"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.RiskAnalysis.RiskAnalysisSettings kelas. Menentukan pengaturan untuk melakukan analisis risiko."
type: docs
weight: 1880
url: /id/net/aspose.tasks.riskanalysis/riskanalysissettings/
---
## RiskAnalysisSettings class

Menentukan pengaturan untuk melakukan analisis risiko.

```csharp
public class RiskAnalysisSettings
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [RiskAnalysisSettings](riskanalysissettings/)() | Menginisialisasi instance baru dari kelas `RiskAnalysisSettings`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [IterationsCount](../../aspose.tasks.riskanalysis/riskanalysissettings/iterationscount/) { get; set; } | Mendapatkan atau mengatur jumlah iterasi yang digunakan dalam simulasi Monte Carlo. Nilai default adalah 100. |
| [Patterns](../../aspose.tasks.riskanalysis/riskanalysissettings/patterns/) { get; } | Mendapatkan koleksi yang berisi instance dari kelas [`RiskPattern`](../riskpattern/). |

## Contoh

Menampilkan cara menyiapkan pengaturan analisis risiko untuk simulasi Monte-Carlo.

```csharp
var riskAnalysisSettings = new RiskAnalysisSettings();

// Atur jumlah iterasi untuk simulasi Monte Carlo (nilai default adalah 100).
riskAnalysisSettings.IterationsCount = 200;

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// Inisialisasi pola risiko
var pattern = new RiskPattern(task);

// Pilih tipe distribusi untuk generator angka acak guna menghasilkan nilai yang mungkin (hanya dua tipe yang saat ini didukung, yaitu normal dan uniform)
// Untuk detail lebih lanjut lihat di sini: https://en.wikipedia.org/wiki/Normal_distribution)
pattern.Distribution = ProbabilityDistributionType.Normal;

// Atur persentase durasi tugas yang paling mungkin yang dapat terjadi dalam skenario proyek terbaik
// Nilai default adalah 75, yang berarti bahwa jika durasi tugas yang diperkirakan adalah 4 hari maka durasi optimis akan menjadi 3 hari
pattern.Optimistic = 70;

// Atur persentase durasi tugas yang paling mungkin yang dapat terjadi dalam skenario proyek terburuk
// Nilai default adalah 125, yang berarti bahwa jika durasi tugas yang diperkirakan adalah 4 hari maka durasi pesimis akan menjadi 5 hari.
pattern.Pessimistic = 130;

// Atur tingkat kepercayaan yang sesuai dengan persentase waktu nilai aktual berada di antara perkiraan optimis dan pesimis.
// Anda dapat menganggapnya sebagai nilai deviasi standar: semakin tidak pasti perkiraan Anda, semakin besar nilai deviasi standar yang digunakan dalam generator angka acak.
pattern.ConfidenceLevel = ConfidenceLevel.CL75;

riskAnalysisSettings.Patterns.Add(pattern);

var analyzer = new RiskAnalyzer(riskAnalysisSettings);
var analysisResult = analyzer.Analyze(project);
var rootEarlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Expected value: {0}", rootEarlyFinish.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", rootEarlyFinish.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", rootEarlyFinish.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", rootEarlyFinish.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", rootEarlyFinish.GetPercentile(90));
Console.WriteLine("Minimum: {0}", rootEarlyFinish.Minimum);
Console.WriteLine("Maximum: {0}", rootEarlyFinish.Maximum);

analysisResult.SaveReport(OutDir + "AnalysisReport_out.pdf");
```

### Lihat Juga

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


