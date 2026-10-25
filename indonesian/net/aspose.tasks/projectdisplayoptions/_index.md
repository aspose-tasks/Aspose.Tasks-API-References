---
title: "Kelas ProjectDisplayOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.ProjectDisplayOptions. Mewakili opsi tampilan untuk sebuah instance proyek"
type: docs
weight: 1450
url: /id/net/aspose.tasks/projectdisplayoptions/
---
## ProjectDisplayOptions class

Mewakili opsi tampilan untuk instance proyek.

```csharp
public class ProjectDisplayOptions
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [ProjectDisplayOptions](projectdisplayoptions/)() | Menginisialisasi instance baru dari kelas `ProjectDisplayOptions`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [AddSpaceBeforeLabel](../../aspose.tasks/projectdisplayoptions/addspacebeforelabel/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah akan menambahkan spasi sebelum nilai angka dan singkatan waktu (1 wk dibandingkan dengan 1wk). |
| [DayLabel](../../aspose.tasks/projectdisplayoptions/daylabel/) { get; set; } | Mendapatkan atau mengatur cara label hari ditampilkan. |
| [HourLabel](../../aspose.tasks/projectdisplayoptions/hourlabel/) { get; set; } | Mendapatkan atau mengatur cara label jam ditampilkan. |
| [MinuteLabel](../../aspose.tasks/projectdisplayoptions/minutelabel/) { get; set; } | Mendapatkan atau mengatur cara label menit ditampilkan. |
| [MonthLabel](../../aspose.tasks/projectdisplayoptions/monthlabel/) { get; set; } | Mendapatkan atau mengatur cara label bulan ditampilkan. |
| [ShowProjectSummaryTask](../../aspose.tasks/projectdisplayoptions/showprojectsummarytask/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah akan menampilkan informasi ringkasan tentang seluruh proyek pada satu baris dengan bilah tugas ringkasan sendiri di bagian atas tampilan Gantt Chart. |
| [ShowTaskScheduleSuggestions](../../aspose.tasks/projectdisplayoptions/showtaskschedulesuggestions/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah akan menampilkan saran ketika Project mengidentifikasi kemungkinan konflik penjadwalan dengan tugas yang dijadwalkan secara manual. Opsi ini tersedia untuk versi Project 2010 dan yang lebih baru. |
| [ShowTaskScheduleWarnings](../../aspose.tasks/projectdisplayoptions/showtaskschedulewarnings/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah menampilkan peringatan ketika Project mengidentifikasi kemungkinan konflik penjadwalan dengan tugas yang dijadwalkan secara manual. Opsi ini tersedia untuk versi Project 2010 dan yang lebih baru. |
| [UnderlineHyperlinks](../../aspose.tasks/projectdisplayoptions/underlinehyperlinks/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah menggarisbawahi tautan. |
| [WeekLabel](../../aspose.tasks/projectdisplayoptions/weeklabel/) { get; set; } | Mendapatkan atau mengatur cara tampilan label minggu. |
| [YearLabel](../../aspose.tasks/projectdisplayoptions/yearlabel/) { get; set; } | Mendapatkan atau mengatur cara tampilan label tahun. |

## Contoh

Menampilkan cara menggunakan opsi tampilan proyek.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// Mengatur nilai yang menunjukkan apakah menampilkan peringatan ketika Project mengidentifikasi kemungkinan konflik penjadwalan dengan tugas yang dijadwalkan secara manual.
// Opsi ini tersedia untuk versi Project 2010 dan yang lebih baru.
project.DisplayOptions.ShowTaskScheduleWarnings = false;

// nilai yang menunjukkan apakah menambahkan spasi sebelum nilai angka dan singkatan waktu (1 wk dibandingkan dengan 1wk)
project.DisplayOptions.AddSpaceBeforeLabel = true;

// atur bagaimana label menit ditampilkan
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.Min;

// atur bagaimana label jam ditampilkan
project.DisplayOptions.HourLabel = HourLabelDisplay.Hr;

// atur cara tampilan label hari
project.DisplayOptions.DayLabel = DayLabelDisplay.Dy;

// atur cara tampilan label minggu
project.DisplayOptions.WeekLabel = WeekLabelDisplay.Week;

// atur bagaimana label bulan ditampilkan
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mon;

// atur bagaimana label tahun ditampilkan
project.DisplayOptions.YearLabel = YearLabelDisplay.Year;

// atur nilai yang menunjukkan apakah menampilkan informasi ringkasan tentang seluruh proyek dalam satu baris dengan batang tugas ringkasan sendiri di bagian atas tampilan Gantt Chart.
project.DisplayOptions.ShowProjectSummaryTask = true;

// atur nilai yang menunjukkan apakah menampilkan saran ketika Project mengidentifikasi kemungkinan konflik penjadwalan dengan tugas yang dijadwalkan secara manual.
project.DisplayOptions.ShowTaskScheduleSuggestions = true;

// atur nilai yang menunjukkan apakah menggarisbawahi tautan.
project.DisplayOptions.UnderlineHyperlinks = true;

project.Save(OutDir + "WorkWithProjectDisplayOptions.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


