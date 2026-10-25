---
title: "PageViewSettings.PrintNotes"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti PageViewSettings. Mendapatkan atau mengatur nilai yang menunjukkan apakah mencetak catatan"
type: docs
weight: 70
url: /id/net/aspose.tasks.visualization/pageviewsettings/printnotes/
---
## PageViewSettings.PrintNotes property

Mendapatkan atau mengatur nilai yang menunjukkan apakah catatan harus dicetak.

```csharp
public bool PrintNotes { get; set; }
```

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

* class [PageViewSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pageviewsettings/)
* assembly [Aspose.Tasks](../../../)


