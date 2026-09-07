---
title: "SaveOptions.IsPortrait"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti SaveOptions. Mendapatkan atau mengatur nilai yang menunjukkan apakah orientasi halaman adalah potret, mengembalikan false jika orientasi halaman adalah lanskap."
type: docs
weight: 70
url: /id/net/aspose.tasks.saving/saveoptions/isportrait/
---
## SaveOptions.IsPortrait property

Mendapatkan atau mengatur nilai yang menunjukkan apakah orientasi halaman potret; mengembalikan false jika orientasi halaman lanskap.

```csharp
public bool IsPortrait { get; set; }
```

## Catatan

Tidak berlaku ketika SaveOptions.PageSize == Visualization.PageSize.DefinedInView. Dalam kasus ini View.PageInfo.PageSettings.IsPortrait digunakan sebagai gantinya. Tidak berlaku ketika SaveOptions.CustomPageSize diatur.

## Contoh

Menampilkan cara menentukan ukuran halaman dan orientasi menggunakan pengaturan View atau menggunakan SaveOptions.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

saveOptions.PageSize = PageSize.DefinedInView;

// Dalam kasus ini ukuran halaman dan orientasi diterapkan dari properti view.PageInfo.PageSettings.PaperSize dan view.PageInfo.PageSettings.IsPortrait.
project.Save(OutDir + "WorkWithIsPortrait_out1.pdf", saveOptions);

saveOptions.PageSize = PageSize.A4;
saveOptions.IsPortrait = true;

// Dalam kasus ini ukuran halaman dan orientasi diterapkan dari properti SaveOptions.
project.Save(OutDir + "WorkWithIsPortrait_out2.pdf", saveOptions);

saveOptions.CustomPageSize = new SizeF(400, 600);

// Dalam kasus ini ukuran halaman diterapkan dari SaveOptions.CustomPageSize. Properti IsPortrait tidak dipertimbangkan.
project.Save(OutDir + "WorkWithIsPortrait_out3.pdf", saveOptions);
```

### Lihat Juga

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


