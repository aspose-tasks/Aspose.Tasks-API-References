---
title: "Kelas RiskPattern"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.RiskAnalysis.RiskPattern class. Mewakili pola risiko untuk sebuah tugas proyek"
type: docs
weight: 1930
url: /id/net/aspose.tasks.riskanalysis/riskpattern/
---
## RiskPattern class

Mewakili pola risiko untuk tugas proyek.

```csharp
public class RiskPattern
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [RiskPattern](riskpattern/)(Task) | Menginisialisasi sebuah instance baru dari kelas `RiskPattern`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [ConfidenceLevel](../../aspose.tasks.riskanalysis/riskpattern/confidencelevel/) { get; set; } | Mendapatkan atau mengatur tingkat kepercayaan yang sesuai dengan persentase waktu nilai yang dihasilkan sebenarnya akan berada dalam perkiraan optimis dan pesimis. Nilai default adalah CL99. |
| [Distribution](../../aspose.tasks.riskanalysis/riskpattern/distribution/) { get; set; } | Mendapatkan atau mengatur distribusi probabilitas yang digunakan dalam simulasi Monte Carlo. Nilai default adalah ProbabilityDistributionType.Normal. |
| [Optimistic](../../aspose.tasks.riskanalysis/riskpattern/optimistic/) { get; set; } | Mendapatkan atau mengatur persentase durasi tugas yang paling mungkin yang dapat terjadi dalam skenario proyek terbaik. Nilai default adalah 75, yang berarti bahwa jika durasi tugas yang diperkirakan adalah 4 hari maka durasi optimis akan menjadi 3 hari. |
| [Pessimistic](../../aspose.tasks.riskanalysis/riskpattern/pessimistic/) { get; set; } | Mendapatkan atau mengatur persentase durasi tugas yang paling mungkin yang dapat terjadi dalam skenario proyek terburuk. Nilai default adalah 125, yang berarti bahwa jika durasi tugas yang diperkirakan adalah 4 hari maka durasi pesimis akan menjadi 5 hari. |
| [Task](../../aspose.tasks.riskanalysis/riskpattern/task/) { get; } | Mendapatkan tugas proyek yang diterapkan pola risiko ini. |

## Contoh

Menampilkan cara mendefinisikan pengaturan simulasi risiko.

```csharp
var settings = new RiskAnalysisSettings();
settings.IterationsCount = 200;

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

settings.Patterns.Add(pattern);

var analyzer = new RiskAnalyzer(settings);
var analysisResult = analyzer.Analyze(project);
var earlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Expected value: {0}", earlyFinish.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", earlyFinish.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", earlyFinish.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", earlyFinish.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", earlyFinish.GetPercentile(90));
Console.WriteLine("Minimum: {0}", earlyFinish.Minimum);
Console.WriteLine("Maximum: {0}", earlyFinish.Maximum);

analysisResult.SaveReport(OutDir + "AnalysisReport_out.pdf");
```

### Lihat Juga

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


