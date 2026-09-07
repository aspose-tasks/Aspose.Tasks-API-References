---
title: "Kelas PageViewSettings"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Visualization.PageViewSettings. Mewakili pengaturan pencetakan untuk tampilan proyek"
type: docs
weight: 3260
url: /id/net/aspose.tasks.visualization/pageviewsettings/
---
## PageViewSettings class

Mewakili pengaturan pencetakan untuk tampilan proyek.

```csharp
public class PageViewSettings
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [PageViewSettings](pageviewsettings/)() | Konstruktor default. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [FirstColumnsCount](../../aspose.tasks.visualization/pageviewsettings/firstcolumnscount/) { get; set; } | Mendapatkan atau mengatur jumlah kolom pertama yang akan dicetak pada semua halaman. |
| [FitTimescaleToEndOfPage](../../aspose.tasks.visualization/pageviewsettings/fittimescaletoendofpage/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah skala waktu harus disesuaikan hingga akhir halaman saat mencetak. |
| [PrintAllSheetColumns](../../aspose.tasks.visualization/pageviewsettings/printallsheetcolumns/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah semua kolom lembar tampilan harus dicetak. |
| [PrintBlankPages](../../aspose.tasks.visualization/pageviewsettings/printblankpages/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah halaman kosong tampilan harus dicetak. |
| [PrintFirstColumnsCountOnAllPages](../../aspose.tasks.visualization/pageviewsettings/printfirstcolumnscountonallpages/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah jumlah kolom pertama tertentu harus dicetak pada semua halaman. |
| [PrintNotes](../../aspose.tasks.visualization/pageviewsettings/printnotes/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah catatan harus dicetak. |

## Contoh

Menampilkan cara mencetak catatan tugas, sumber daya, dan penugasan pada halaman terpisah.

```csharp
var project = new Project(DataDir + "Input.mpp");

// atur jumlah kolom pertama yang akan dicetak pada semua halaman
project.DefaultView.PageInfo.PageViewSettings.FirstColumnsCount = 2;

// atur nilai yang menunjukkan apakah catatan harus dicetak.
project.DefaultView.PageInfo.PageViewSettings.PrintNotes = true;

// atur nilai yang menunjukkan apakah skala waktu harus disesuaikan hingga akhir halaman saat mencetak.
project.DefaultView.PageInfo.PageViewSettings.FitTimescaleToEndOfPage = true;

// atur nilai yang menunjukkan apakah semua kolom lembar tampilan harus dicetak
project.DefaultView.PageInfo.PageViewSettings.PrintAllSheetColumns = true;

// atur nilai yang menunjukkan apakah halaman kosong tampilan harus dicetak
project.DefaultView.PageInfo.PageViewSettings.PrintBlankPages = false;

// atur nilai yang menunjukkan apakah mencetak sejumlah kolom pertama yang ditentukan pada semua halaman
project.DefaultView.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

project.Save(OutDir + "ProjectWithComments_out.pdf", SaveFileFormat.Pdf);
```

### Lihat Juga

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


