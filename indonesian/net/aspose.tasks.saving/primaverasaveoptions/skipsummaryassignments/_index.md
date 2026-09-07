---
title: "PrimaveraSaveOptions.SkipSummaryAssignments"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti PrimaveraSaveOptions. Mendapatkan atau mengatur nilai yang menunjukkan apakah penugasan sumber daya ke tugas rangkuman harus dilewati selama ekspor"
type: docs
weight: 60
url: /id/net/aspose.tasks.saving/primaverasaveoptions/skipsummaryassignments/
---
## PrimaveraSaveOptions.SkipSummaryAssignments property

Mendapatkan atau mengatur nilai yang menunjukkan apakah penugasan sumber daya ke tugas rangkuman harus dilewati selama ekspor.

```csharp
public bool SkipSummaryAssignments { get; set; }
```

## Catatan

Perangkat lunak Primavera tidak mendukung penugasan sumber daya ke tugas ringkasan (WBS). Oleh karena itu, ekspor penugasan semacam itu dapat menghasilkan file yang tidak valid menurut model Primavera. Jika true, penugasan ke tugas ringkasan akan dilewati selama ekspor. Jika false (nilai default), sebuah pengecualian akan dilemparkan jika penugasan ke tugas ringkasan ditemukan selama ekspor.

## Contoh

Menampilkan cara menggunakan flag SkipSummaryAssignments.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var resource = project.Resources.Add("Resource");

var summaryTask = project.RootTask.Children.Add("Summary");
summaryTask.Children.Add("Task");

// Primavera tidak mendukung penugasan sumber daya ke tugas ringkasan.
// Jadi mengekspor penugasan semacam itu ke format Primavera dapat menghasilkan file yang tidak dapat diimpor ke Primavera.
var assignment = project.ResourceAssignments.Add(summaryTask, resource);

var options = new PrimaveraXmlSaveOptions();
options.SkipSummaryAssignments = true;
project.Save(OutDir + "UseSkipSummaryAssignments_out.xml", options);
```

### Lihat Juga

* class [PrimaveraSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaverasaveoptions/)
* assembly [Aspose.Tasks](../../../)


