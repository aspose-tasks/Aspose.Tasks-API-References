---
title: "Enum ReportType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.Visualization.ReportType enum. Jenis laporan grafis proyek"
type: docs
weight: 3330
url: /id/net/aspose.tasks.visualization/reporttype/
---
## ReportType enumeration

Tipe laporan grafis proyek.

```csharp
public enum ReportType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| ProjectOverview | `0` | Menampilkan tanggal mulai dan selesai proyek, persentase durasi yang selesai, persentase penyelesaian untuk tugas tingkat atas, dan tonggak yang akan datang. |
| CostOverview | `1` | Menampilkan tanggal mulai dan selesai proyek, biaya terjadwal dan sisa biaya saat ini, % Selesai, dan nilai biaya untuk tugas tingkat atas. |
| WorkOverview | `2` | Menampilkan baseline, aktual, dan pekerjaan yang tersisa untuk setiap tugas tingkat atas serta pekerjaan untuk sumber daya kerja. |
| ResourceOverview | `3` | Menampilkan baseline, aktual, dan pekerjaan yang tersisa per sumber daya. |
| ResourceCostOverview | `4` | Menampilkan baseline, aktual, dan biaya yang tersisa per sumber daya. |
| CriticalTasks | `5` | Menampilkan tugas proyek yang kritis. |
| LateTasks | `6` | Menampilkan tugas proyek yang terlambat. |
| Milestones | `7` | Menampilkan tonggak yang terlambat, yang akan datang, dan yang selesai. |
| UpcomingTask | `8` | Menampilkan tugas yang jatuh tempo selama minggu ini dan tugas yang dimulai selama minggu ini. |
| CostOverruns | `9` | Menampilkan variasi biaya per tugas dan sumber daya. |
| TaskCostOverview | `10` | Menampilkan baseline, aktual, dan biaya yang tersisa dari semua tugas tingkat atas. |
| OverallocatedResources | `11` | Menampilkan jumlah jam kerja yang tersisa untuk sumber daya yang terlalu dialokasikan. |
| SlippingTasks | `12` | Menampilkan tugas yang dijadwalkan selesai setelah tanggal selesai baseline mereka (baseline harus diatur). |
| BestPracticeAnalyzer | `13` | Menampilkan tugas tanpa pekerjaan aktual, tugas yang tidak ditugaskan, tugas dengan durasi kurang dari 8 jam, dan ringkasan yang ditugaskan dengan sumber daya. |
| Burndown | `14` | Termasuk diagram work burndown dan task burndown. Diagram work burndown menunjukkan berapa banyak pekerjaan yang telah selesai, berapa banyak yang dijadwalkan selesai sebelum tanggal selesai proyek, dan perkiraan baseline berapa banyak pekerjaan yang akan selesai pada titik ini dalam proyek. Diagram task burndown menunjukkan jumlah tugas yang selesai, jumlah yang tersisa, dan perkiraan baseline berapa banyak yang akan selesai pada titik ini dalam proyek. |
| CashFlow | `15` | Menampilkan biaya dan biaya kumulatif per kuartal untuk semua tugas tingkat atas. |

## Contoh

Menampilkan cara menyimpan laporan burndown proyek dalam format PDF ke aliran yang ditentukan.

```csharp
var project = new Project(DataDir + @"Homemoveplan.mpp");
using (var stream = new FileStream(OutDir + "Burndown_out.pdf", FileMode.Create))
{
    project.SaveReport(stream, ReportType.Burndown);
}
```

### Lihat Juga

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


