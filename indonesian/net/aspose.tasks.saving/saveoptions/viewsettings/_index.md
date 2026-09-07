---
title: "SaveOptions.ViewSettings"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti SaveOptions. Mendapatkan atau mengatur sebuah view View untuk dirender. Anda dapat menggunakan opsi ini untuk secara eksplisit menentukan view mana yang harus disimpan ke format PDF, HTML, atau Image. Jika properti ini diatur, properti PresentationFormat diabaikan saat proyek disimpan. View harus berasal dari salah satu layar berikut: Screen Gantt TaskSheet TaskUsage ResourceSheet ResourceUsage."
type: docs
weight: 240
url: /id/net/aspose.tasks.saving/saveoptions/viewsettings/
---
## SaveOptions.ViewSettings property

Mendapatkan atau mengatur sebuah view ([`View`](../view/)) untuk dirender. Anda dapat menggunakan opsi ini untuk secara eksplisit menentukan view mana yang harus disimpan ke format PDF, HTML, atau Image. Jika properti ini diatur, properti [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) diabaikan saat proyek disimpan. View harus berasal dari salah satu layar berikut (([`Screen`](../../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage).

```csharp
public View ViewSettings { get; set; }
```

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | Ketika metode set dipanggil dan instance kelas View dengan nilai Screen yang tidak didukung diberikan. |

## Contoh

Menampilkan cara menggunakan 'SaveOptions.ViewSettings' untuk menentukan view yang harus dirender ke PDF.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);
Console.WriteLine("Page size specified in view settings: " + view.PageInfo.PageSettings.PaperSize);
Console.WriteLine("Page orientation: {0}", view.PageInfo.PageSettings.IsPortrait ? "Portrait" : "Landscape");

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.DefinedInView;
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

project.Save(OutDir + "SaveToPdfUsingSpecificView_out.pdf", saveOptions);
```

### Lihat Juga

* class [View](../../../aspose.tasks/view/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


