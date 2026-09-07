---
title: "ProjectDisplayOptions.ShowTaskScheduleWarnings"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ProjectDisplayOptions. Mendapatkan atau mengatur nilai yang menunjukkan apakah menampilkan peringatan ketika Project mengidentifikasi kemungkinan konflik penjadwalan dengan tugas yang dijadwalkan secara manual. Opsi ini tersedia untuk versi Project 2010 dan yang lebih baru."
type: docs
weight: 90
url: /id/net/aspose.tasks/projectdisplayoptions/showtaskschedulewarnings/
---
## ProjectDisplayOptions.ShowTaskScheduleWarnings property

Mendapatkan atau mengatur nilai yang menunjukkan apakah menampilkan peringatan ketika Project mengidentifikasi kemungkinan konflik penjadwalan dengan tugas yang dijadwalkan secara manual. Opsi ini tersedia untuk versi Project 2010 dan yang lebih baru.

```csharp
public bool ShowTaskScheduleWarnings { get; set; }
```

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

* class [ProjectDisplayOptions](../)
* namespace [Aspose.Tasks](../../projectdisplayoptions/)
* assembly [Aspose.Tasks](../../../)


