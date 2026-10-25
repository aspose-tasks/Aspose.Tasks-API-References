---
title: "Enum TimescaleFitBehavior"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.Visualization.TimescaleFitBehavior. Mewakili perilaku yang digunakan untuk menyelaraskan area skala waktu dengan lebar halaman."
type: docs
weight: 3440
url: /id/net/aspose.tasks.visualization/timescalefitbehavior/
---
## TimescaleFitBehavior enumeration

Mewakili perilaku yang digunakan untuk menyelaraskan area skala waktu dengan lebar halaman.

```csharp
public enum TimescaleFitBehavior
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| DefinedInView | `0` | Bagian kalender dirender sesuai dengan properti View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage dari Tampilan yang dirender. |
| NoScaleToEndDate | `1` | Bagian kalender dirender tepat hingga EndDate, meskipun ada ruang kosong pada halaman. |
| NoScaleToEndOfPage | `2` | Bagian kalender dirender hingga akhir (sisi kanan) halaman terakhir. Dengan demikian tanggal yang dirender terakhir dapat melampaui EndDate. |
| ScaleToEndOfPage | `3` | Mesin rendering akan mencoba menyelaraskan tanggal sehingga EndDate selaras dengan akhir (sisi kanan) halaman terakhir. Sesuai dengan opsi "Page Setup \\ View \\ Fit timescale to end of page" pada MS Project yang diaktifkan. |

## Contoh

Menampilkan cara menggunakan TimescaleFitBehavior agar skala waktu diagram Gantt menyesuaikan hingga akhir halaman terakhir.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.DefaultView as GanttChartView;

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.A4;
saveOptions.StartDate = project.StartDate;
saveOptions.EndDate = project.FinishDate;
saveOptions.ViewSettings = view;
saveOptions.TimescaleFitBehavior = TimescaleFitBehavior.ScaleToEndOfPage;

project.Save(OutDir + "WorkWithPageSizeDefinedInView_out.pdf", saveOptions);
```

### Lihat Juga

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


