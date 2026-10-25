---
title: "RiskPattern.RiskPattern"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor RiskPattern. Menginisialisasi sebuah instance baru dari kelas RiskPattern."
type: docs
weight: 10
url: /id/net/aspose.tasks.riskanalysis/riskpattern/riskpattern/
---
## RiskPattern constructor

Menginisialisasi sebuah instance baru dari kelas [`RiskPattern`](../).

```csharp
public RiskPattern(Task task)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tugas | Tugas | tugas proyek yang ditentukan dimana risiko ini akan diterapkan dalam simulasi Monte Carlo. |

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

* class [Task](../../../aspose.tasks/task/)
* class [RiskPattern](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskpattern/)
* assembly [Aspose.Tasks](../../../)


