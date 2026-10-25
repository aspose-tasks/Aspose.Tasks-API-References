---
title: "Enum RiskItemType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.RiskAnalysis.RiskItemType enum. Menentukan bidang tugas yang informasi statistiknya dikumpulkan selama analisis risiko."
type: docs
weight: 1920
url: /id/net/aspose.tasks.riskanalysis/riskitemtype/
---
## RiskItemType enumeration

Menentukan bidang tugas yang informasi statistiknya dikumpulkan selama analisis risiko.

```csharp
public enum RiskItemType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Start | `0` | Mulai Tugas. |
| Finish | `1` | Selesai Tugas. |
| EarlyStart | `2` | Mulai Awal Tugas. |
| EarlyFinish | `3` | Selesai Awal Tugas. |
| LateStart | `4` | Mulai Terlambat Tugas. |
| LateFinish | `5` | Selesai Terlambat Tugas. |

## Contoh

Menampilkan cara menghitung statistik risiko dan menyimpannya sebagai laporan PDF.

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

// simpan analisis sebagai laporan ke file dengan jalur file
analysisResult.SaveReport(OutDir + "AnalysisResult_out.pdf");

// atau simpan analisis ke aliran
using (var stream = new FileStream(OutDir + "AnalysisResult_out1.pdf", FileMode.Create))
{
    analysisResult.SaveReport(stream);
}
```

### Lihat Juga

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


